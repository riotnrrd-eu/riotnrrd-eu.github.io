---
layout: post
title:  Not Biting My Tongue 
date:   2017-07-11 
categories:  bsm BMC enterprise AIOps 
---

I spend a lot of time explaining enterprise buyers and vendors. There are often perfectly good reasons for doing something in a way that is now considered old-fashioned or uncool. Especially for vendors, the argument of "people still buy X! for money!" is a powerful incentive to continue making X.

Where things go wrong is when stodgy enterprise vendors put on their dad-jeans and go down to the skate park.

![](/images/giphy-3.gif)

Case in point: [BMC trying to jump on the AIOps bandwagon](http://www.bmc.com/blogs/what-is-aiops/ "What Is AIOps? AIOps Explained"). The whole thing is a pretty spectacular case study in missing the point, but I think this paragraph is the nadir:

> As mentioned above, AIOps platforms should encompass the IT disciplines of Performance Management, Service Management, Automation, and Process Improvement, along with technologies such as monitoring, service desk, capacity management, cloud computing, SaaS, mobility, IoT and more.

If you’re not familiar with AIOps, it’s a model that [Gartner came up with](https://www.gartner.com/doc/3263717/innovation-insight-algorithmic-it-operations "Innovation Insight for Algorithmic IT Operations Platforms") (paid link, unless you’re a Gartner subscriber) to describe some shifts in the IT operations market. The old category of ITOA had been broadened to the point that it was effectively meaningless, and AIOps recognises a new approach to the topic.

The first thing to know about AIOps is that the "AI" bit did not originally stand for Artificial Intelligence. When the term was originally coined, AIOps actually stood for Algorithmic IT Operations. However, in these fallen times when everyone and their dog claims AI, Machine Learning, or other poorly-understood snake-oil, everyone assumed that AIOps was something to do with AI. Even Gartner have now given up, and retconned it to "Artificial Intelligence for IT Operations". 

Anyway, AIOps solutions sit at the intersection of monitoring, service desk, and automation. The idea is that they ingest monitoring data, apply algorithms to help operators find valuable needles in the haystack of alerts, sync with service desk systems to plug in to existing processes, and trigger automated diagnostic and resolution activities.

![](/images/083448.jpg)

So far so good - but here’s why it’s so laughable for BMC to claim AIOps. 

BMC’s whole model is BSM - Business Service Management. Where the centre of AIOps is the algorithms, the centre of BSM is the CMDB. 

![](/images/083859.jpg)

The model for applying BSM goes something like this:

1. Fully populate CMDB: define service models & document infrastructure
2. When an alert comes in, determine which infrastructure element it came from, then walk the service model to determine what the cause and effect are
3. Create a ticket in the ITSM suite to track resolution

Note the hidden assumptions, even in this grossly over-simplified version:

1. The CMDB can be fully populated given finite time and effort
2. All alerts relate to known elements, and all elements have known dependencies
3. Every failure has one cause and falls within one group’s area of responsibility

In today’s IT, precisely *none* of these assumptions hold true. No matter how much effort and how many auto-discovery tools are thrown at the task, the CMDB will always be a snapshot in time[^1]. Jorge Luis Borges famously [documented](https://en.wikipedia.org/wiki/On_Exactitude_in_Science) the logical endpoint of this progression:

> ... In that Empire, the Art of Cartography attained such Perfection that the map of a single Province occupied the entirety of a City, and the map of the Empire, the entirety of a Province. In time, those Unconscionable Maps no longer satisfied, and the Cartographers Guilds struck a Map of the Empire whose size was that of the Empire, and which coincided point for point with it. The following Generations, who were not so fond of the Study of Cartography as their Forebears had been, saw that that vast map was Useless, and not without some Pitilessness was it, that they delivered it up to the Inclemencies of Sun and Winters. In the Deserts of the West, still today, there are Tattered Ruins of that Map, inhabited by Animals and Beggars; in all the Land there is no other Relic of the Disciplines of Geography.
>
> *purportedly from Suárez Miranda, Travels of Prudent Men, Book Four, Ch. XLV, Lérida, 1658*

There is also a timing factor: what happens if an alert comes in between a change occurring and being documented? Another question is, what happens if operators simply don’t have visibility into part of the infrastructure - say, managed hosting, or outside telco networks? And finally, the big one: what if there is no one root cause? Modern architectures are sufficiently robust and resilient that it’s quite rare for any one macro-event to take them out. What gets you is usually a combination of a number of smaller issues, all occurring together in some unforeseen way.

The whole architecture of BSM is built around assumptions that are less and less true. This is not to say that individual *products* within that suite don’t have value, but the old BSM model is no longer fit for purpose. The result is an example of “shipping the org chart”: the CMDB is at the core and Remedy is the interface, because that is what the organisation demands. However, you can’t just drape AIOps over the old suite and call it good! Radical changes are required, not weak attempts to shoe-horn existing "IT disciplines" into the new mold.

AIOps represents the **algorithmic** convergence of ITOM & ITSM. In contrast, if we consider the sequence of BSM, these are assumed to be different discrete steps in a sequential process. This is Waterfall thinking applied to IT Ops, where today’s IT infrastructures demand Agile thinking.

The most relevant question for users is, of course, "do I trust a legacy vendor to deliver a new model that is so radically different from what it has built its entire strategy around?" 

The answer is simple, because it’s determined by the entire structure and market position of all the Big Four vendors. Like its peers, BMC makes its revenue in the old model of IT. As long as there is money to be made by doing the same things it has always done, there is enormous inertia to work against (the [Innovator’s Dilemma](https://en.wikipedia.org/wiki/The_Innovator%27s_Dilemma) in action). It takes an existential threat to disturb that sort of equilibrium. It was not until ServiceNow was seriously threatening the Remedy user base that BMC started to offer SaaS options and subscription pricing. It will take an equivalent upheaval in its business for any legacy vendor to adopt a radically new strategy like AIOps. These days, customers can’t wait for one vendor to see the writing on the wall; they need to move at the speed their customers require.

Much as I would like to believe that [we](http://www.moogsoft.com) have got BMC running scared, I don’t think that’s the case - so they will continue along their very profitable way. This is of course exactly how it should be! If they were to jump on every new bandwagon, their shareholders would be rightly furious. They absolutely should focus on doing what they do well. 

But that does not include doing AIOps. If you’re a practitioner looking at this, I hope it’s obvious who you want to go with: the people creating the new model and who are steeped in what is required to deliver and adopt it - or the ones who see a keyword trending on Google, and write a quick ambulance-chasing blog post - or claim that [Remedy is a key part of AIOps](http://www.bmc.com/it-solutions/aiops.html) - or even that [mainframes are](https://www.bmc.com/blogs/aiops-improving-it-operations/).

![](/images/unknown_filename.246.jpeg)

[^1]: Which is why BMC’s own automation products have their separate real-time operational data stores, which sync with the CMDB on a schedule.