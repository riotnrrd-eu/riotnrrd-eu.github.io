---
layout: post
title:  Adventures in Screen Sharing 
date:   2014-10-31 
categories:  tech Apple MacOS 
---

# Adventures in Screen Sharing


I'm having an odd issue, and I wonder whether anyone else has seen anything like this. 

I have a headless Mac mini[^1], named "cooper" for reasons that should be obvious. The mini lives in a cupboard (not under the stairs), and its main job is to run iTunes and feed the AppleTV, as well as any other long-duration tasks. It also occasionally acts as a test bed for my projects, but those have been few and far between lately. *Surprise!* It turns out that having kids takes up a bunch of time that would otherwise be available for projects, and once they're in bed I'm usually too shattered to do anything very serious. 

Because it's headless, the main way I interact with it is via Share Screen from my MacBook Air. The problem is that the mini occasionally loses the ability to advertise itself as a Shared device in the Finder sidebar. 

![|157x42](/images/unknown_filename.7.png) 

In this screenshot, I only see the NAS. There should be another entry above that, like so: 

![|161x74](/images/unknown_filename.8.png) 

The thing is, the mini is still reachable via VNC - just not from the Finder, because the Finder in its wisdom only allows you to Share Screen from a machine that is visible under Shared. Using the "Connect to" menu action, or for that matter iSSH on the iPad, however, I can still VNC in and see that everything is running fine. 

The only fix to this issue that I have found is to reboot the mini. Since I can get in both via VNC and via SSH, this isn't a huge issue, because I can shut things down and make it a clean reboot, but it's still annoying. I haven't been able to figure out a cause, either; sometimes it happens while I'm connected via Share Screen if the Air goes to sleep, while at other times it happens if the mini is asleep - it wakes up but doesn't advertise itself in the Finder sidebar. 

Both the Air and the mini are running Yosemite. Any suggestions? 

*** 

**UPDATE**: Ars Technica did [publish](http://arstechnica.com/apple/2015/01/why-dns-in-os-x-10-10-is-broken-and-what-you-can-do-to-fix-it/ "Why DNS in OS X 10.10 is broken, and what you can do to fix it" ) a deeper investigation than I got into. It seems that the root of the problem is indeed in discovery, as I had surmised. With Yosemite, Apple switched from `mDNSResponder` to `discoveryd`, and it looks like the latter has some issues. 

That said, the Ars suggestion of restoring `mDNSResponder` seems insane to me. I guess I will just muddle through until Apple fixes `discoveryd`.

[^1]: Yes, that is the correct capitalisation, TYVM.

