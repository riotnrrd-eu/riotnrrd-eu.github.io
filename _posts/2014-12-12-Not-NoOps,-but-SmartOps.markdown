---
layout: post
title:  Not NoOps, but SmartOps 
date:   2014-12-12 
categories:  devops NoOps 
---

# Not NoOps, but SmartOps


### Or, **Don't work harder, work smarter**

I have always been irritated by some of the more extreme rhetoric around DevOps. I especially hate the way DevOps often gets simplified into blaming everything that went wrong in the past on the Ops team, and explicitly minimising their role in the future. At its extreme, this tendency is encapsulated by the *NoOps* movement.

This is why I was heartened to read [There is no such thing as NoOps](http://www.itskeptic.org/content/there-no-such-thing-noops-it-awful-word "There is no such thing as NoOps: it is an awful word | The IT Skeptic"), by the reliably acerbic IT Skeptic.

Annoyingly, in terms of the original terminology, I quite agree that we need to get rid of Ops. Back in the day, there was a distinction between [*admins*](http://en.wikipedia.org/wiki/System_administrator) and [*ops*](http://en.wikipedia.org/wiki/Computer_operator). The sysadmins were the senior people, who had deep skills and experience, and generally spent their time planning and analysing rather than executing. The operators were typically junior roles, often proto-sysadmins working through an apprenticeship.

Getting rid of ops in this meaning makes perfect sense. The major cause of outages is human error, and not necessarily the fairly obvious moment when the poor overworked ops realize one oh-no-second after hitting Enter that the login shell was not where they thought it was. What leads to these human-mediated outages is **complexity**, so the issue is the valid change that is made here but not there, or the upgrade that happened to one component but did not flow down to later stages of the lifecycle. These are the types of human error that can either cause failures on deployment, or those more subtle issues which only show up under load, or every second Thursday, or only when the customer's name has a Y in it.

There have been many attempts to reduce the incidence of these moments by enforcing policies, review, and procedures. However, by not eliminating the weakest link in the chain - the human one - none of these well-meaning attempts have succeeded. Instead of saying "it will work this time, really!", we should aim to to eliminate downtime and improve performance by removing every possible human intervention and hand-over, and instead allowing one single original design to propagate everywhere automatically.

So yes, we get rid of ops by automating their jobs - what I once heard a sysadmin friend describe to a colleague as "monkey-compatible tasks", basically low-value-added, tactical, hands-on-keyboard activity. However, that does ***not*** mean that there is no role for IT! It simply means that IT's role is no longer in execution, or in other words, as the bottleneck in every request.

### Standard requests should not require hands-on-keyboard intervention from IT.

This is what all these *WhateverOps* movements are about: preventing IT from becoming a bottleneck to other departments, whether the developers in the case of DevOps, or the GRC team in the case of SecOps that I keep banging on about lately, or whatever other variation you like.

IT still has a very important role to play, but it is not the *operator's* role, it is the *sysadmin's* role: to plan, to strategise, to have a deep understanding of the infrastructure. Ultimately, IT's role is to advise other teams on how best to achieve their goals, and to emplace and maintain the automation that lets them do that - much as sysadmins in the past would have worked to train their junior operators to deliver on requests.

The thing is, sysadmins themselves can't *wait* to rid themselves of scut work. Nothing would make them happier! But the state of the art today makes that difficult to achieve. DevOps et al are the friend of IT, not its enemy, at least when they're done right. Done wrong, they are [the developer's enemy too]({% post_url 2014-04-23-DevOps-is-killing-us %}).

In that sense, I say yes to NoOps - but let's not throw the baby out with the bathwater! Any developer trying to do completely without an IT team will soon find that they no longer have any time to develop, because they are so busy with all this extraneous activity, managing their infrastructure[^1], keeping it compliant, updating components, and all the thousand and one tasks IT performs to keep the lights on.

[^1]: No, Docker, "the cloud", or whatever fad comes next will not obviate this problem; there will always be some level of infrastructure that needs to be looked after. Even if it works completely lights-out in the normal way of things, someone will need to understand it well enough to fix it when (not if) it breaks. That person is IT, no matter which department they sit in.