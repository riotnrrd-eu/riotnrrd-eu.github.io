---
layout: post
title:  Lowering the Barrier to Cloud 
date:   2014-12-15 
categories:  cloud 
---

The 451 Group might not have the name recognition of some of the bigger analyst firms, with their magic quadrants and what-not, but there is a lot of value in their approach to the business. In particular, they have the only "cloud economist" I know, in the person of [Dr Owen Rogers](https://451research.com/biography?eid=698 "Analyst Bios - 451 Research"). Dr Rogers actually did his PhD on the economics of cloud computing, so he knows what he is talking about. 

Dr Rogers also defies the stereotype of economists by being fun to talk to. He's also good on his personal blog - see [this recent post](http://cloud-economics.com/post/105016816894/my-wife-and-jevons-paradox "My wife and Jevon’s paradox" ) for instance. I'll let you read the setup yourself - it's worth it - but I just wanted to comment on the closing paragraph: 

> Moving to the cloud might make cost-savings. But actually, it might just mean you consume more IT resources than you might have otherwise. This isn’t a bad thing in itself - just make sure you’re prepared, and that this extra consumption is deriving something real in return. 

![](/images/unknown_filename.220.png)

This is something that I have seen in action time and time again - although not so much recently. Certainly in the early days of cloud computing, when it was still widely seen as "virtualisation 2.0", many people jumped in thinking that cloud would substantially lower the cost of IT, by keeping the volume constant - or even shrinking it by controlling virtualisation sprawl - while lowering costs. 

Unfortunately for people who built their business cases around this model, it didn't quite work out that way. Done right, cloud computing certainly lowers the *unit cost* of IT - the cost to deliver a certain quantum of IT service. Note that the unit here is not "a server", otherwise straight virtualisation would have been sufficient to deliver the expected benefits. People outside of IT cannot consume "a server* directly; they need a lot more to be done before it is useful to them: 

* Install and configure database
* Install and configure middleware
* Deploy application code
* Reserve storage
* Set up networking (routing, load balancer, firewall/NAT access, …)
* Security hardening
* Compliance checks 
* And so on and so forth 

Doing all of this in a pre-cloud way was **expensive**. Even if all the IT infrastructure was in-house, it was expensive in opportunity costs - all the other tasks that those various teams had on their plates - and in the simple time necessary to deliver all of those different parts. Worse, it wasn't just a one-off cost, but an *ongoing* cost. This is where another term from economics gets introduced: **technical debt**, or the future work that IT commits itself to in order to maintain what they deliver. 

All of this translated to a high barrier to access IT services. The only applications  (in the business sense, not the App Store sense) that could be implemented were ones that could clear the high hurdle of being able to justify not only the initial outlay and delay, but all the future maintenance costs. 

Cloud computing changes that equation by lowering the barrier to entry. The most expensive component of IT delivery, both in resources and in time, is *manual human action*. By automating that away, the unit cost of IT drops dramatically. 

This is where Jevons' Paradox comes in. Instead of lowering the *total* cost of IT, this reduction in the unit cost unlocks all sorts of applications that were previously unthinkable. The result is that instead of delivering the same amount of IT for less money, companies end up delivering *much more* IT for the same budget. 

How to ensure that this flowering of IT delivers business value? In yet another intersection of IT and economics, let us turn to the *Financial Times* and an article entitled "[Big service providers turn to the cloud](http://www.ft.com/cms/s/0/5e09386a-7563-11e4-a1a9-00144feabdc0.html?ftcamp=published_links%2Frss%2Freports_the-connected-business%2Ffeed%2F%2Fprod&siteedition=uk#axzz3LxLn8m2A "Big service providers turn to the cloud - FT.com")": 

> According to Forrester Research, technologies with a direct impact on a company’s business, such as customer relationship management services and analytics, eat up only about 20 per cent of IT spending. 

That is where the value of cloud computing comes from: the good old 80/20 rule. Done right, cloud computing acts on both parts of the rule, making it easy to increase the 20% of IT that actually delivers value - by lowering the barrier to entry - while automating or outsourcing the keep-the-lights-on activity that consumes the other 80% of the IT budget. 

So much for the dismal science!