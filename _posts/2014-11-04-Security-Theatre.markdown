---
layout: post
title:  Security Theatre 
date:   2014-11-04 
categories:  security tech MDM mobile MacOS 
---

# Security Theatre


There are many things in IT that are received knowledge, things that *everyone knows*.

One thing that *everyone knows* is that you have to manage employee's mobile devices to prevent unauthorised access to enterprise systems. My employer's choice of MDM agent is a bit intrusive for my personal tastes, so I opted not to install it on my personal iPad. The iPhone is the company's device, so it's their own choice what they want me to run on it.

Among other things, this agent is required to connect to the company Exchange server from mobile devices. You can't just add an Exchange account and log in with your AD credentials, you need this agent to be in place.

![](/images/unknown_filename.296.jpeg)

But why the focus on mobile devices?

When I upgraded my work and home Macs to Yosemite, I finally turned on the iCloud Keychain. I hadn't checked exactly what was syncing, and was surprised to see work calendar alerts turning up on my home Mac. My personal Mac had just grabbed my AD credentials out of iCloud and logged in to Exchange, without any challenge from the corporate side.

So how is that different from my iPad? Why is a Mac exempt from the roadblock? A Mac is arguably **less** secure than an iPad if it gets forgotten in a coffee shop or whatever - never mind a Windows machine. Why is "mobile" different? Just because?

Many enterprise IT people seem to lose their minds when it comes to mobile device management. I'm not necessarily arguing for just dropping the requirement, just for a sane evaluation of the risks and the responses that are required.

