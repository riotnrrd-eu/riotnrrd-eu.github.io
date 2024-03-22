---
layout: post
title:  DevOps is killing us 
date:   2014-04-23 
categories:  devops tech 
---

# DevOps is killing us


I came across [this interesting article](http://www.paperplanes.de/2014/4/17/the-developer-is-dead.html "The Developer is Dead, Long Live the Developer" ) about the changes that DevOps brings to the developer role. Because of my sysadmin background, I had tended to focus on the Ops side of DevOps. I had simply not realised that developers might object to DevOps!

I knew sysadmins often didn’t like DevOps, of course. Generalising wildly, sysadmins are not happy with DevOps because it means they have to give non-sysadmins access to the systems. This is not just jealousy (although there is often some of that), but a very real awareness that incentives are not necessarily aligned. Developers want change, sysadmins want stability.

Actually, that point is important. Let me emphasise it some more.

# Developers want change, sysadmins want stability

Typical pre-DevOps scenario: developers code up an application, and it works. It passes all the testing: functional, performance, and user-acceptance. Now it’s time to deploy it in production - and suddenly the sysadmins are begin *difficult*, complaining about processes running as root and world-writable directories, or talking about maintenance windows for the deployment. Developers just want the code that they have spent all this time working on to get *out there*, and the sysadmins are in the way.

From the point of view of the sysadmins, it’s a bit different. They just got all the systems how they like them, and now developers are asking for the keys? Not only that, but their stuff is all messy, with processes running as root, world-writable directories, and goodness knows what. When the sysadmins point out these issues and propose reasonable corrections, the devs get all huffy, and before you know it, the meeting has turned into a [blamestorm](http://en.wiktionary.org/wiki/blamestorm "blamestorm - Wiktionary" ).

![](/images/unknown_filename.98.png)

The DevOps movement attempts to address this by getting developers more involved in operations, meaning instead of throwing their code over the proverbial wall between Dev and Ops, they have to support not just deployment but also support and maintenance of that code. In other words, developers have to start carrying pagers.

The default sysadmin assumption is that developers can’t wait to get the root password and go joy-riding in their carefully maintained datacenter - and because I have a sysadmin background, sell to sysadmins, and hang out with sysadmin types, I had unconsciously bought into that. However, now someone points it out, it does make sense that developers would not *want* to take up that pager…

