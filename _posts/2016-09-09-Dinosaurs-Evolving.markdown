---
layout: post
title:  Dinosaurs Evolving 
date:   2016-09-09 
categories:  iPhone email 
---

Right now, basically the entire Internet is having a massive collective tantrum over the fact that [Apple dropped the headphone jack from the newest iPhone](https://www.buzzfeed.com/johnpaczkowski/inside-iphone-7-why-apple-killed-the-headphone-jack ). This, despite the fact that (in a very un-Apple move) the box includes *both* a Lightning-to-TRS audio jack adapter, *and* a pair of EarPods with a Lightning connector.

Speaking for myself, I already specced out the iPhone I want, but I’m just waiting to pick it up when I go to San Francisco next month. Some times, geo restrictions actually work in my favour, as even with SF sales tax, the US price is a couple of hundred Euros cheaper than my local price. EarPods don’t fit my ears (which also means the new AirPods are out), so I’ll use the adapter while I look for W1 wireless earphones that I like.

The hysteria over the whole thing reminded me of a situation that is the exact opposite, one where an “obsolete” standard keeps soldiering on, despite repeated attempts to kill it or just declare it dead by fiat.

I am of course referring to email[^1].

## A bit of history

To [recap](https://www.theguardian.com/technology/2016/mar/07/email-ray-tomlinson-history), everything started back in those tie-died days of 1965. This was not yet email as we know it, however; even the @-sign was not added until 1971, although for a while there things like [bang paths](http://www.catb.org/jargon/html/B/bang-path.html "bang path" ) were viable alternatives.

In those days the Internet in general and email specifically were still things that only academics and governments used. However, in September of 1993 - [the September that never ended](https://en.wikipedia.org/wiki/Eternal_September) - Arpanet was opened up to the public, becoming the Internet[^2]. It didn’t take long for the whole thing to degenerate into the wretched hive of scum and villainy that we know and love today.

![](/images/unknown_filename.99.jpeg)

So why did email survive the transition to the Internet, when many other protocols, including beloved ones like Usenet, withered and died? And why are people still trying to kill it now, with the likes of [Slack](https://slack.com ) or [Cisco Spark](https://www.ciscospark.com ) or Microsoft's [Yammer](https://products.office.com/yammer ) or Salesforce [Chatter](http://www.salesforce.com/chatter/overview/ ) or whatever?

The key thing about email is that it is extremely simple. If you want (and if you can still find an SMTP server that does not require authentication), you can still send email from the command line in just a couple of lines.

```
> telnet mail.domain.ext 25
Trying ???.???.???.???...
Connected to mail.domain.ext.
Escape character is '^]'.
220 mail.domain.ext ESMTP Sendmail ?version-number?; ?date+time+gmtoffset?
> HELO local.domain.name
250 mail.domain.ext Hello local.domain.name [loc.al.i.p], pleased to meet you
> MAIL FROM: mail@domain.ext
250 2.1.0 mail@domain.ext... Sender ok
> RCPT TO: mail@otherdomain.ext
250 2.1.0 mail@otherdomain.ext... Recipient ok
> DATA
> Subject: This is a subject
>
> This is the body of the email
> .
250 2.0.0 ???????? Message accepted for delivery
> QUIT
221 2.0.0 mail.domain.ext closing connection
Connection closed by foreign host. 
```

Try *that* with Chatter.

Of course nobody would do that except for a stunt - but this is what is going on in the background of every mail client you would actually *use* on a regular basis. The simplicity of this protocol means that anyone can implement their own tool, offering specific capabilities. Email clients can be arbitrarily simple or complex, and anyone can choose one that suits their own requirements.

## Email is email is email

One of the consequences of that simplicity is universality and flexibility. Anyone using email can communicate with anyone else, regardless of what client or server software they are using. Email is email is email.

In contrast, most would-be email killers are walled gardens, consisting of a service that is tightly integrated with its client app and does not allow third-party clients. This makes it much harder for innovation to happen, because there is only one provider, and they deliver only the functionality that they want and can build. If you want a feature to be added to Slack, you can’t build your own Slack client; you have to petition Slack to do it, and they choose whether to implement that feature or not.

Even now, more than fifty years into the age of email, there is constant experimentation, with new email clients popping up all the time. Right now I am using one called [Notion](https://notion.ai "Notion AI" ), which implements all sorts of gestures to triage your inbox. You can “star” messages, file them, and even snooze them so that they go away but come back to your inbox later. Even in the simplest clients, you still have the option to read something and then mark it as unread so that you don’t forget about it.

Try snoozing a notification from Facebook Messenger, or marking a WhatsApp message as unread to return to it later. Can’t be done.

You don’t need a fancy client, either. There are a ton of features built right into the protocol. Think of the concise power of the CC and BCC headers, or the simple “forward” action. With CC (“carbon copy”, a coelacanth term surviving from a previous age of office technology) you can make people aware of a conversation, while also making it clear that they are being informed but are not expected to take action. BCC (“blind carbon copy”) lets you send a message without making each participant aware of all of the others, so you can let your boss see the email you sent without the recipients seeing their name. BCC *should* also be used by anyone sending mass emails, to avoid disclosing the entire recipient list to every recipient, but people regularly forget - with hilarious consequences.

In contrast, chat systems are symmetrical. You can add people to a group chat, but it’s a flat hierarchy; no question of someone being informed as opposed to an active participant, or a silent observer. Forwarding a message with its context is also usually impossible. Sure, you can easily copy the text, but not the group participants and so on. Email’s simplicity make all of these features universal, independent of the generosity of one particular developer.

![](/images/unknown_filename.100.jpeg)

## Email just won’t die

Email is unkillable because it provides substantial utility, and it is easy for people to build additional value on top of a common standard. In other words, if it's a dinosaur, it's the sort that didn't get killed by an asteroid, but instead grew feathers and is still around today.

The old TRS audio jack has only ubiquity in its favour. It does not offer any particular functionality; the TRRRS extended spec that lets in-line remotes work is a horrible hack, and it’s kind of surprising that it works as well as it does.

Also, most iPhone users just use the EarPods they get with their device, so I would not have been surprised if, absent the media firestorm and rending of vestments, people would have just used the Lightning EarPods and not even have noticed the change.

And if you feel *that* strongly about it, use the adapter that Apple puts right in the box.

Who wants to bet that inside of two years, all the major Android manufactures offer phones with audio over Micro USB or something similar, instead of TRS? [Some](https://www.engadget.com/2016/04/20/leeco-le-2-pro-max-smartphones-china/#/ ) [vendors](http://motorola-blog.blogspot.it/2016/06/the-new-moto-z-family-with-moto-mods.html ) already do…

[^1]: Yes, I have given up on calling it “e-mail”, although I still think that is more correct.
[^2]: An internet, the Internet. Come at me.

