---
layout: post
title:  All Software Sucks 
date:   2013-06-24 
categories:  tech cloud
---

It is a truism in high-tech that *All Software Sucks*. (There is an equally valid corollary that *All Hardware Sucks*.) The usual reason for restating this universally accepted truth is to deflate someone who is lapsing into advocacy of one platform over another. There is a deeper truth here, though, and it's about who builds the software, who for, and why.

Many open-source projects have terrible interfaces, major usability issues, and appearances that only a mother could love. This is because the creators by and large did not get into the project for that part; they wanted a tool that would perform a specific, often quite technical, task for them, and assembled a band of like-minded enthusiasts to work on the project in their off-hours.

This is great when the outcome of the project is something like the Linux kernel, which is safely hidden away from users who might cut themselves on its sharp edges. Problems start to occur when the band of hackers try to build something closer to the everyday surface that people see and use. There must be a thousand Linux desktop environments around when you count the combinations, and while each of them suits *somebody*'s needs, they are otherwise pretty uniformly horrible to look at and inconsistent to use.

The same applies to enterprise software, but for a slightly different reason. Cynics have long suggested that the problem with enterprise software is that the buyer is not the user: purchasing departments and CIOs don't have to live with the consequences of their decisions. While I don't doubt that some of this goes on, in my experience both groups of people are usually trying to do their best. The problem is with the selection process itself.

Who specs enterprise software? Until very recently, only the IT department, and even now they still do most of it. Much like open-source hackers, they draw up the specification based on their own needs, drivers, and experience. These days, though, more and more people within the enterprise are doing more and more with the software tools, and they expect even more. Gone are the days of sending a supplication through inter-office mail to the high tower of IT. People have become used to self-service systems with attractive interfaces in their personal lives, and they expect the same at work.

Enterprise IT departments are struggling to adapt to this brave new world:

+ Their security policies are crafted around the concept of a *perimeter*, but that perimeter no longer exists. Personally-owned devices and corporate devices used for personal purposes have fuzzed the edges, and great chunks of the business process and even the infrastructure now live outside the firewall.
+ Their operational procedures are based on the idea that only a small band of experts who all work together and understand each other will work on the infrastructure, but more and more of the world doesn't work that way any more. Whether it's self-service changes for users, shared infrastructure that IT does not have full control over, developers doing their own thing, or even the infrastructure changing itself through automation, there is simply no way for every change to be known, in advance or indeed at all.
+ Their focus on IT is narrow and does not encompass all the ways people are interacting with their devices and systems. In fact, the IT department itself is often divided into groups responsible for different layers, so that an overall view even of the purely technical aspects is difficult to achieve.

This is important right now because enterprise IT departments are looking at a phase change, and many are failing or shying away from the new challenges. These days I am working on cloud management platforms, which are at the intersection of all of these issues. Too many of these projects take too long, fail to achieve all of their objectives, or never even get off the ground.

## How does this happen?

The reasons for these failures are exactly what I described above. Here are a couple of real-life examples (names have been removed to protect the guilty).

The CIO of a large corporation in the energy and resource sector illustrated his cloud roadmap to me. The roadmap had been developed with the advice of a large consultancy, and was ambitious, long-term, and complete - except for one thing. After his presentation was complete, I asked him who he expected the users and use cases to be. His answer was: "The IT department, of course!" Noting my flabbergasted expression, he added: "Why, what else are they going to do?" What else, indeed? As far as I know, that roadmap has still not found any existence beyond the CIO's PowerPoint slides.

A major international bank did begin its cloud project, and implemented everything successfully. New and very advanced state-of-the-art hardware was procured, all the infrastructure and management software was installed, everyone congratulated each other, and the system was declared open for business. A few months later, the good cheer had evaporated, as usage of the system was far below projections: a few tens of requests per month, instead of the expected several hundred. It seems that nobody had thought to ask the users what they needed, or to explain how the new system could help them achieve it.

Something even worse happened to a big European telco. The cloud platform was specified, architected, evaluated, selected, and implemented according to a strict roadmap that had been built jointly by the telco’s own in-house architects and consultants from a big-name firm. Soon after the first go-live milestone, though, we all realised that utilisation was well below projections, just as in the case of the bank above.

As it happened, though, I was also talking to a different group within the company. A team of developers needed a way to test their product at scale before releasing it, and were struggling to get hold of the required infrastructure. This seemed to me like a match made in heaven, so I brokered a meeting between the two groups.

To cut a long story short, the meeting was a complete train wreck. The developers needed to provision "full stack" services: not just the bare VM, but several software components above that. They also needed to configure both the software components and the network elements in between to make sure all the bits & pieces of their system were talking to each other. All of this was right in the brochure for the technology we had installed - but the architects flatly refused to countenance the possibility of letting developers provision anything but bare VMs, saying that full-stack provisioning was still nine months out according to their roadmap.

That project managed to stagger on for a while, but eventually died quietly in a corner. I think it peaked at 600 simultaneous VMs, which is of course nothing in the cloud.

What is the lesson of these three stories?

The successful projects and products are the ones where people are not just designing and building a tool for themselves, but for a wide group of users. This is a fundamentally different approach, especially for enterprise IT, but it is necessary if IT is to survive.

## So what do we do now?

If you are in enterprise IT, the new cloud services that users are asking for or even adopting on their own are *not* your competition. If someone out there can offer a better service more cheaply than you can operate it in house, that's ***great***; one less headache for you. Your job is not to be engaged in the fulfilment of each request - because that makes you the bottleneck in the process. That sort of thinking is why IT is so often known as "the department of No". Instead, focus on making sure that each request is fulfilled, on time, on spec, and on budget.

If you are *selling* to enterprise IT, help them along this road. Talk to the users, and share your findings back with the IT department. This way everybody wins. 

Talk to the users, they'll tell you what the problem is. Have no doubt about that.
