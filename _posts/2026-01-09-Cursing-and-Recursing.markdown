---
layout: post
title:  Cursing and Recursing
date:   2026-01-09
categories: cloud AI
---

I've been paid to work in IT for nearly three decades, starting when I was still in high school. Once you have been around IT that long, you start to see patterns come around over and over. This pattern recognition has both good and bad aspects, as do most things in this fallen world of ours.

The big benefit is that I can often shortcut my way to the sense of something by spotting that "oh, it's similar to this other thing I have seen in the past". The big drawback is that I have to be on my guard that this doesn't turn me into (even more of) a curmudgeon, grumbling that there's nothing new and everything was already invented in back in nineteen-oatcake.

![A train speeding along the rails](/images/linus-mimietz-9Z3acH8gBps-unsplash.jpg)

With that said, I think that experience gives us a useful lens through which to analyse the current AI wave (bubble?), and that is the rise of cloud computing fifteen to twenty years ago (wow, I'm old). I was working on a cloud management product at the time, and I wrote a couple of blog posts which I think are still relevant.

I should point out right away that I am talking only of enterprise use of AI, hence the cloud computing comparison. I am not going to try to get into the mess that is consumer AI, with "nudify" apps, wholesale IP theft, or the extremely thorny topic of AI use in education, except to say that those are *applications* of the technology, not anything inherent in Large Language Models. The people building the tools own the outcomes, but the underlying models can still be useful elsewhere.

In the enterprise context, too, there are good and bad applications. If Alice uses GenAI to expand a two-line prompt into a professional-looking and well-formatted email to Bob, and he uses GenAI to summarise it (lossily) back down to two lines, what exactly is the point of the GenAI? This sort of thing is symptomatic of the early days of a technology adoption wave, and to me at least, it explains a lot of the current mismatch between investment (huge), adoption (unclear), and value (lagging).

However, lots of enterprise processes rely on working with large volumes of text, and that is where GenAI can be very useful. This is after all the big remaining opportunity for organisational automation: all of the processes that involved working with numbers have already been digitised by now.

# Time For Some Tall Tales

Back in 2013, I reminded everyone that *[All Software Sucks]({% post_url  2013-06-24-All-Software-Sucks %})*. I'm not going to quote the whole thing here; by all means click through if you're interested, but the gist is that I shared three war stories about enterprise cloud projects that completely failed at the **adoption** stage.

Cloud computing, together with mobile computing, turned the world of enterprise IT upside down. Instead of users meekly taking whatever they were handed by corporate IT departments, they were bringing iPhones to work and signing up for AWS accounts and SaaS tools. Suddenly, corporate IT departments found themselves scrambling to keep up with new expectations.

![The Earth from space](/images/nasa-Q1p7bh3SHj8-unsplash.jpg)

My pitch at the time was that this sort of "[shadow IT]({% post_url 2014-09-05-Enterprise-IT-Kill-Switch %})" was a sign of *unmet demand*. Before then, if corporate IT didn't deliver something, you simply couldn't have it. These days, we take it for granted that you can sign up to some SaaS tool in minutes and ask for forgiveness rather than permission.

AI follows a very similar user-driven adoption pattern. Once again, users are voting with their actions, and while corporate IT departments are cautiously evaluating alternatives and studying options, they already downloaded the app and are merrily using it. 

One aspect that is different this time around is that vendors are actively enabling this shadow adoption, as opposed to the tacit approval they showed during the early days of cloud. Copilots and assistants get enabled in software updates to major productivity suites and even operating systems, with no opt-out or central control for corporate IT. Companies are left scrambling to catch up and work out which of these emerging use cases are good, bad, or actively dangerous. It's all very well to [signal that you're all-in on AI]({% post_url 2014-06-18-Signalling %}), but you have to walk the walk too.

# What Have We Learned?

That's where those stories of failed cloud adoption projects are important: this time around, we can avoid making the same mistakes. Users are going to adopt whatever tools make their jobs easier and their working lives better. IT's role is to make sure that they are enabling as much as possible of that demand in a way that is safe and controlled.

![Code on a computer screen](/images/luca-bravo-XJXWbfSo2f0-unsplash.jpg)

The benefits of code-generating assistants, to take one example, are huge — to individual coders. It's pointless to try to ban these tools, especially when they are already embedded in popular development environments. But coding is only a relatively small portion of product development. Even if developers are seeing the mythical 10x productivity increases, if the rest of the release pipeline is not overhauled, all that has happened is the creation of a massive bottleneck which may actually cause negative overall impacts. 

Vice versa, my guess is that programmers fearing for their jobs may well be right to be nervous in the short term, but in the longer term, we will see many *more* jobs in software development. With the rise of cloud, it's true that traditional sysadmins have become an endangered breed — but there has been an explosion in SRE, DevOps, and other operational roles. The work simply happens at a different level of the stack. There will continue to be value in deep expertise that can drop down several levels of abstraction to debug problems or extract ultimate performance, but that won't be the day-to-day reality for most people.

# It's Still Early Days

It's also worth remembering that it's still very early in the current wave of interest in AI. SnapGPT, which triggered the raising of AI's profile, is barely three years old as I write this. There is still a lot of throwing stuff at the wall and seeing what sticks — and that is as it should be. Again, the role of corporate IT is to facilitate these experiments, if only because they will be happening *anyway*, so it's worth being involved to make sure they stay contained.

The trap here is staying too long in the experimentation phase, to the point that users get tired of waiting and go off and do their own thing. This is a fast-moving environment; any commitment is temporary, and is, or should be, capable of being easily reversed. Don't bet the farm on one LLM or one tool; they are all constantly leap-frogging each other, and a clear winner today may not be in a quarter or too. 

Again, I get to reiterate my own advice from the early days of cloud: keep your options open. When we started out scoping the market back then, we started with VMware (the major incumbent in our customer base) and AWS (the obvious rising star). However, we assumed that our next step would be to support the major Unix platforms: Solaris Zones and AIX LPARs (HP-UX was already dead on its feet, even then). However, by the time we got around to the development work, those platforms were hemorrhaging users, so we pivoted to Microsoft Azure and Hyper-V.

![A stack of coffee cups](/images/nathan-dumlao-3kZpELkaxHc-unsplash.jpg)

# Find The Value Up The Stack

The point is that, even in those fast-moving early days, we focused on how we as a management-tool vendor, and our customers in enterprise IT, could differentiate. Provisioning a virtual server was no great trick even back then, much as chatty AI bots are ten-a-penny these days. Where things got interesting was if you needed to deploy various software stacks and custom configurations, including certifying the compliance of the result, without having to maintain an unmanageably large catalogue of templates — and especially if you needed to deploy *clusters* of such things, which all needed to be aware of each other.

It's the same with AI. A generic chatbot is not interesting. One that has (safe and compliant) access to your specific internal data is better. One that can call on agents which in turn can trigger custom functions in other systems? Now we're talking. And if one of those agents or tools needs to change? Well, if you architect the overall system right, you can do that without disrupting users' work. 

Who won in cloud? The people who build value-added services on top of the basic compute elements, which had been turned into undifferentiated commodities.

Who will win in AI? My forecast is that it won't be the model builders[^1]: it will be the people who build useful services on top of them, whether as vendors or as users.

***

🖼️  Photos by [Linus Mimietz](https://linktr.ee/linusmimietz), [NASA](http://www.nasa.gov/), [Luca Bravo](https://unsplash.com/@lucabravo) and [Nathan Dumlao](https://unsplash.com/@nate_dumlao) on [Unsplash](https://www.unsplash.com)

[^1]: Here is my caveat: I do not mean that the current wave of LLM vendors will go out of business! AWS is doing just fine — but they hardly talk about EC2 these days; it's all about the myriad services which they (and others) have built on top of EC2. Yes, everything depends on the building blocks of compute, but that's not what's important to users, or to investors. Once the current excitement settles down a bit, I expect the same thing to happen in AI: pure-play model builders will fade into the background, while providers of AI-enabled services will take the next wave of investment and adoption. Some of those will happen to *also* develop models, but it won't be the main thing they do or talk about.