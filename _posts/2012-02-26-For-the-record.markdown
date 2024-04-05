---
layout: post
title:  For the record 
date:   2012-02-26 
categories:  tech FreeBSD DNS
---

I've done all of this before, but that was a long time ago, and when it came to doing it again, I realised I had forgotten all of it and had to start over. Therefore, for the benefit of my future self and anyone who is trying to do the same thing, here is how to set up a FreeBSD box to act as a firewall and caching name server for its local network.

First things first, you need the hardware. I went with an Intel Atom CPU, because this box runs 24x7 and I wanted something that wouldn't eat too many watts. I sat that in a D525 micro-ATX board and put that in an Antec Mini-Skeleton case. If you haven't seen one, here's what it looks like:

![](/images/unknown_filename.146.jpeg)

The fan on the top is pretty quiet, and lights up blue if you want.

I added a second network interface because one of this machine's jobs is to act as firewall, and off we go.

I'm running FreeBSD because it is as close to a hassle-free OS as I know. It also lets me keep in practice at running a real, non quiche-eating OS, plus has the added benefit of freaking out anyone who asks to use my computer. Between FreeBSD and the keyboard with blank key-caps, most people bail out without even trying.

First things first, I need to get the server to talk to my ISP and to provide IP addresses to the local LAN. On FreeBSD, this is super easy. Just add the following to `rc.conf`:

```
     ifconfig_rl0=“DHCP"
     ifconfig_re0="inet 192.168.1.1 netmask 255.255.255.0 broadcast 192.168.1.255”
     dhcpd_enable=“YES"
     dhcpd_ifaces=“re0"
     pf_enable=“YES"
     pflog_enable=“YES"
     gateway_enable=“YES"
     named_enable=“YES"
     named_auto_forward=“yes"
     named_auto_forward_only="yes"
```

The first line instructs the `rl0` network interface to request its configuration via DHCP. The second line gives a fixed address to interface `re0`.

I wanted a firewall that would let me talk to the outside world, but would not allow any inbound traffic. Since my ISP NATs traffic unles you pay them lots, there is no downside to a complete lock-down. I went with pf, purely because it's hard to replicate in iptables the artistic intent of a pf rule that says `pass out quick on $cheap_gin`. The pf firewall is enabled by the `pf_enable=YES"` line in `rc.conf`, and configured with `pf.conf`. Here's my firewall setup:

```
     ext_if = “rl0"
     haus_if = “re0"
     haus_ips = "192.168.1.0/24”
     wifi_ips = "192.168.3.0/24”
     priv_nets = "{ 127.0.0.1/8, 192.168.0.0/16, 172.16.0.0/12, 10.0.0.0/8 }”
     table <firewall> const { self }
     set loginterface $ext_if
     set skip on lo0
     set skip on plip0
     #antispoof log for $ext_if inet

     scrub in all
     nat on $ext_if from $haus_if:network to any -> ($ext_if)

     block all
     block drop in quick from urpf-failed
     block drop in quick on $ext_if from $priv_nets to any
     block drop out quick on $ext_if from any to $priv_nets
     pass out on $ext_if proto tcp all modulate state flags S/SA
     pass out on $ext_if proto { udp icmp } all modulate state
     pass in on $haus_if from $haus_if:network to any keep state
     pass out on $haus_if from any to $haus_if:network keep state
```

Simples. I have my two interfaces, `rl0` and `re0`, respectively the one facing teh internets and the one facing the house LAN. Everything from the outside gets dropped, including anything spoofing an address which should be internal, and everying from the inside gets passed, whether to the outside or to another internal network.

Now everything in the house can talk to the internet. Next, DHCP and dynamic DNS. The DHCP server, dhcpd, is started with the `dhcpd_enable="YES"` line from `rc.conf`. This enables the server, and then `dhcpd_ifaces="re0"`, which forces it to listen only on the internal interface. Having dealt with rogue DHCP servers before, I don't want to be guilty of unleashing one. The DHCP server is then configured with `dhcpd.conf`:

```
     option domain-name "dashaus.lan”;
     option domain-name-servers 192.168.1.1;
     option subnet-mask 255.255.255.0;

     default-lease-time 600;
     max-lease-time 7200;
     authoritative;

     ddns-update-style interim;
     ddns-domainname "dashaus.lan”;
     ddns-rev-domainname "1.168.192.in-addr.arpa”;
     log-facility local7;
     update-static-leases on;
     do-forward-updates true;

     subnet 192.168.1.0 netmask 255.255.255.0 {
          range 192.168.1.2 192.168.1.200;
          option routers 192.168.1.1;
   	 }
```

The house domain is `dashaus.lan`, and this is the authoritative DHCP server for the domain. In addition, any device that gets an IP address from this server also gets its hostname resolvable under `dashaus.lan`. This is great for not having to remember which access point has 192.168.1.15, or where the NAS is now. Sure, I could do it with hosts files, but then I'd have to update those, and iOS doesn't do hosts files anyway, so this is better.

Of course this doesn't work alone - you also need a DNS server. I enabled it simply by adding `named_enable="YES"` to `rc.conf`.

And here is my `named.conf`:

```
     options {
          directory       "/etc/namedb/working”;
          pid-file        "/var/run/named/pid”;
          dump-file       "/var/dump/named_dump.db”;

          statistics-file "/var/stats/named.stats”;
          listen-on       { 127.0.0.1; 192.168.1.1; };

          disable-empty-zone "255.255.255.255.IN-ADDR.ARPA”;
          disable-empty-zone "0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.IP6.ARPA”;
          disable-empty-zone "1.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.0.IP6.ARPA”;

          include "/etc/namedb/auto_forward.conf”;
     };

     acl dashaus{
          192.168.1.0/24;
          127.0.0.1;
     };

     zone "." { type hint; file "/etc/namedb/named.root"; };
     zone "dashaus.lan” {
          type master;
          file "dashaus”;
          allow-update {
               dashaus;
          };
     };

     zone "1.168.192.in-addr.arpa” {
          type master;
          file "dashaus.rev”;
          allow-update {
               dashaus;
          };
     };
```

There's nothing particularly funky going on here. The acl directive specifies that only clients with an IP address in that subnet can update their DNS records. Here are the zone files:

```
     $ORIGIN .
     $TTL 86400      ; 1 day
     dashaus.lan             IN SOA  skeletor.dashaus.lan. root.skeletor.dashaus.lan. (
                                20011955   ; serial
                                3600       ; refresh (1 hour)
                                900        ; retry (15 minutes)
                                3600000    ; expire (5 weeks 6 days 16 hours)
                                3600       ; minimum (1 hour)
                                )
                        NS      skeletor.dashaus.lan.

     $ORIGIN dashaus.lan.
     $TTL 300        ; 5 minutes
     Apple-TV                A       192.168.1.11
                        TXT     “31da5805e31cba162785449fe301a035f2"
     beast                   A       192.168.1.5
                        TXT     “31140c046d012654084168c75af137a956"
     Claras-iPad             A       192.168.1.31
                        TXT     “31d7c4fd01cef4e2f76a201fdaa8a6e56c"
     dashaus-nas             A       192.168.1.4
                        TXT     “31d02895fbe37aebe514fc5f5bd685b703"
     demonic-iPad            A       192.168.1.14    
                        TXT     “31e907692c02809efc782ef4fd60568712"
     Demonic-iPhone          A       192.168.1.7
                        TXT     “312d530aa18c5c3f8da67f54b9a35a938d"
     HPB1251A                A       192.168.1.9    
                        TXT     "31a9b7ff798848034e2cf14e05aa6f7648”    
     $TTL 86400      ; 1 day
     skeletor                A       192.168.1.1
```

Skeletor is the server's name, for obvious case-related reasons. Here's the reverse file:

```
     $ORIGIN .
     $TTL 86400      ; 1 day
     1.168.192.in-addr.arpa  IN SOA  skeletor.dashaus.lan. root.skeletor.dashaus.lan. (
                                20011704   ; serial
                                3600       ; refresh (1 hour)
                                900        ; retry (15 minutes)
                                3600000    ; expire (5 weeks 6 days 16 hours)
                                3600       ; minimum (1 hour)
                                )
                        NS      skeletor.dashaus.lan.

     $ORIGIN 1.168.192.1.168.192.in-addr.arpa.
     $TTL 300        ; 5 minutes
     11                      PTR     Apple-TV.dashaus.lan.
     14                      PTR     demonic-iPad.dashaus.lan.
     31                      PTR     Claras-iPad.dashaus.lan.
     4                       PTR     dashaus-nas.dashaus.lan.
     5                       PTR     beast.dashaus.lan.
     7                       PTR     Demonic-iPhone.dashaus.lan.
     9                       PTR     HPB1251A.dashaus.lan.
```

This is from a running instance, so you can see the AppleTV, a couple of iPads, an iPhone, the NAS, Beast (my Windows box), and the printer, each with its own IP address. I assume the wifi APs aren't showing up because they haven't refreshed recently, but they're working so I am not going to mess with them!

Last step: as this stands, clients can recognize each other, but Skeletor itself can't resolve other local clients. This is inconvenient if you want to export an X session to yourself and can't remember your IP address. The problem is that the ISP-facing interface is configured via DHCP, so `resolv.conf` gets over-written every time dhclient refreshes - every 1800 seconds, or every half-hour.

The way to fix that is by writing `dhclient.conf`:

```
     interface “rl0”
     {
          prepend domain-name-servers 127.0.0.1;
          supersede domain-name "dashaus.lan”;
     }
```

This adds the local DNS server before the ones supplied by my ISP, and forces unqualified hostname searches to use the house domain instead of going to the internet.

Now if I could just get an X server running... Everything looks good, but actually starting X puts my monitor to sleep. This looks like a sync out of range issue, but I cannot figure out how to fix it. The really frustrating thing is that I cannot get back to a text console to try again, I actually have to reboot. Fortunately I can get in via SSH to pull logs and do a safe reboot, but it's still far from ideal. The X client is fine - if I fire up an X server somewhere else, I can export apps just fine, which is how I was able to [fail]({% post_url 2012-02-25-Adventures-in-Airplay %}) at configuring Totem.

Any X-on-FreeBSD gurus, hit me up!