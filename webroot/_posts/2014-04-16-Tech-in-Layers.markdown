---
layout: post
title:  Tech in Layers 
date:   2014-04-16 
categories:  tech industry pace-layering 
---

# Tech in Layers


*This post is the follow-up to the earlier post [Caveat Vendor]({% post_url 2014-04-11-Caveat-Vendor %}).*

It’s not easy being an enterprise IT buyer these days. Time was, the IBM sales rep would show up once a year, you would cover your eyes and sign the cheque, and that would be it for another year. Then things got complicated.

Nowadays there are dozens of vendors at each level of your stack, and more every day. Any hope of controlling the Cambrian explosion of technologies in the enterprise went out of the window with the advent of cloud computing. Large companies used to maintain an Office of Vendor Relations, or words to that effect. Their job was to try to keep the number of vendors the company dealt with to a minimum. The rationale was simple: if we have an existing enterprise licensing agreement with BigCo, introducing PluckyStartupCo just adds risk, not to mention complicating our contract negotiations. It doesn’t matter if PluckyStartupCo has better tech than BigCo, we get good enough tech from BigCo as part of our Enterprise Licensing Agreement (all hail the ELA!). On top of that we are pretty sure BigCo is going to be around for the long haul, while PluckyStartupCo is untested and will either go bust or get bought by someone else, either BigCo or one of their competitors. Job done, knock off at five on the dot.

The dependency of business on technology is too close for that approach to work any longer. The performance of IT ***is*** the performance of the business, to all intents and purposes. If you don’t believe me, try visiting an office when the power is down or the net connection has gone out. Not much business gets done without IT.

If companies effectively hobble themselves with antiquated approaches to procurement, they leave themselves wide open to being outmanoeuvred by their competitors. When the first non-tech companies built websites, plenty of their competitors thought it was a fad, but those early adopters stole a march on their slow-moving erstwhile peers.

All of this does not even count **shadow IT**. Famously, [Gartner predicted](http://www.gartner.com/newsroom/id/1862714 "Gartner Reveals Top Predictions for IT Organizations and Users for 2012 and Beyond") that “*By 2015, 35 percent of enterprise IT expenditures for most organizations will be managed outside the IT department's budget.*” People are bringing their own services, not just the techie example of devs[^1] spinning up servers in AWS, but business users - Muggles - using Dropbox, Basecamp, Google Hangouts and Docs, Slideshare, Prezi, and so on and on.

## What is a CIO or CTO to do?

First of all, don’t try to stop the train - you’ll just get run down. The only thing you can do is to jump on board and help drive it. Note that I said *help*: IT can no longer lead from high up an ivory tower. IT leaders need to engage with their business counterparts, or those business users will vote with their feet and go elsewhere for their IT services.

IT leaders can help the business by building a policy framework to encompass all of these various technologies. Most importantly, this framework has to be flexible and assume that new technologies will appear and gain adoption. Users won’t listen if you say “we’ll review doing a pilot of that cool new tech in six months, and if that goes well we can maybe roll it out a year from now”. By the time you’ve finished speaking, they’ve already signed up online and invited all their team-mates.

Fortunately, there is a technique that can be used to build these frameworks. It’s called *pace layering*, and was [introduced by Gartner](http://www.gartner.com/newsroom/id/1923014 "Gartner Says Adopting a Pace-Layered Application Strategy Can Accelerate Innovation") in 2012.

## Pace Layering

Pace layering divides IT into three layers:

+ **Systems of Record** — Established packaged applications or legacy homegrown systems that support core transaction processing and manage the organization's critical master data. The rate of change is low, because the processes are well-established and common to most organizations, and often are subject to regulatory requirements.

+ **Systems of Differentiation** — Applications that enable unique company processes or industry-specific capabilities. They have a medium life cycle (one to three years), but need to be reconfigured frequently to accommodate changing business practices or customer requirements.

+ **Systems of Innovation** — New applications that are built on an ad hoc basis to address new business requirements or opportunities. These are typically short life cycle projects (zero to 12 months) using departmental or outside resources and consumer-grade technologies.

The idea is that there are parts of the business where the emphasis is on absolute stability, reliability and predictability - the *Systems of Record*, which are basically the boring stuff that has to work but isn’t particularly interesting. Other areas need to move fast and respond with agility to changing conditions - the *Systems of Innovation*, the cool high-tech leading-edge stuff. In between there are the *Systems of Differentiation*, which are about what the company actually *does*. They need to move fast enough to be relevant, but still be reliable enough to use - often a tough balancing act. The layering looks like this:

![|1411x0](/images/153039.jpg)

If we overlay two common IT methodologies, we start to understand many of the ongoing arguments of the last few years, where it seems that practitioners are talking past each other:

![|1368x0](/images/153058.jpg)

DevOps, Agile, and so on are approaches that work well for Systems of Innovation. Here it is appropriate to "move fast and break stuff", to fail fast, to A/B test things on the live environment. Run with what works; the goal is speed and quickly figuring out the Next Big Thing.

ITIL is the opposite: it’s designed for a cautious approach to mature and predictable systems, with the ultimate goal of maintaining stability. Here, the absolute goal is *not breaking stuff*; the whole *moving fast* part is completely subordinate to that goal.

I hear a lot of complaints along the lines of “ITIL is a bottleneck on IT”, “ITIL is the anti-Agile”, and so on. In the same vein, ITIL sages throw up their hands in horror at some of what the new crowd are getting up to. The thing is, **they’re both right**.

Use ITIL where it’s appropriate, and be agile where *that* is appropriate. Try to figure out the demarcation points, the hand-offs, and where you can, by all means take the best of both worlds. You don’t want to have to wait for the weekly Change Advisory Board meeting to make a minor website change, but when something goes wrong, you’ll be thankful for having some sort of an audit trail in place.

## From operations to planning

So much for operations - but the same applies to planning. The Systems of Record might have a roadmap planned out years in advance, with little reason to deviate from it. The motto here is “**if it ain’t broke, DON’T TOUCH IT!**”. This is the part of the company where mainframes still lurk. Why? *Because they work*. It’s as simple as that.

On the other hand, the Systems of Innovation are where you want to let a thousand clouds bloom (to coin a phrase). Let people try all those wonderful services I mentioned earlier. The ones that are useful and safe will gradually get adopted further back from the bleeding edge. If something doesn’t make the cut, no matter - you didn’t bet the company on it.

To return to one of my pet arguments, the Systems of Record are virtualised, the Systems of Differentiation are on a private cloud, and the Systems of Innovation are in the public cloud. This way, the strengths of each model fit nicely with each layer’s requirements.

The problems arise if get your layers mixed up - but that’s outside the scope of this post.

[^1]: Not “debs", whatever autocorrect might think. Although the image is amusing.

