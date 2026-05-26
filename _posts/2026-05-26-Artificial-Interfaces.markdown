---
layout: post
title:  Artificial Interfaces
date:   2026-05-26
categories:  AI GUI UX
---

There are two main strands to the conversation about people using AI to create software. One is centred on the idea that jobbing programmers will increase their output dramatically, perhaps as much as 10x, but still within the context of the existing software industry. The other is that non-programmers will create their own application for purposes that were underserved until now.

I am not a software engineer, so I don't have a huge amount to say about the first scenario, except to note that in my experience working alongside programmers, the ability of a programmer to type more lines of code is not the main bottleneck in the creation of usable and desirable software.

The other angle is more interesting, though. After all, the business case for making programmers more productive is fairly obvious: if the demand is static, then you can satisfy it with fewer people — although [recent news stories](https://www.theverge.com/transportation/937116/uber-ai-investment-hard-to-justify) call into question what the influence of LLM tokens will be on the COGS. And if the demand turns out to be elastic, then the same number of professional programmers can presumptively turn out *much more software* with these tools. But what if there are whole domains of demand that are entirely untapped today? What might happen if that new opportunity for people to create their own tools could be unlocked with new technology?

We are told that [citizen developers are redefining enterprise AI development](https://www.techtarget.com/searchenterpriseai/tip/Citizen-developers-are-redefining-enterprise-AI-development), because people who understand the business process can now work directly through AI tooling to create apps that automate that process, instead of dealing with the laborious back-and-forth with professional programmers that would have been required in the past.

This idea of user empowerment is not a new concept: previous incarnations were labelled as "citizen developers", fourth-generation programming languages (4GL), SQL itself, and going all the way back to FORTRAN. The difference with GenAI is that, instead of easier ways to code up the permanent paths users will take within the system, we are now talking about being able to create graphical interfaces and user experiences that are single-use, entirely ephemeral. 

![Ephemeral views](/images/jr-korpa-tBA_u2bUMfg-unsplash.jpg)

This change from permanent to ephemeral user experiences is entirely a consequence of the changing temporal requirements for the creation of a new graphical interface (the real economics in terms of AI model tokens will not be clear for a while yet).

Previously, even creating something simple like a new report or dashboard required arcane knowledge of how the source system represented and exposed the data that it stored. Now, as we [delaminate user interfaces from the systems that underpin them](https://thejaymo.net/2026/05/25/ai-generated-interfaces-ui/), entirely new ways of working with that data become possible. No more dashboards being generated "because we've always done it that way" — and meanwhile, people and teams actually managing the reality of their business entirely offline, with spreadsheets, and only reconciling the spreadsheets with the system of record at the end of the quarter.

![Typical Apple product: one button labelled "Touch". Typical Google product: a search field with a button labelled "Find". Your company's app: a dog's breakfast of fields, labels, and buttons.](/images/simplicity.jpeg)

On the surface, this democratisation is a huge win: people are able to get the data that they need from the central system, and in return, they will be more willing to feed current and accurate data back into that system, for the use and benefit of other teams.

Here is the problem. Those horrible enterprise user interfaces all encode a particular representation of data that is optimised to match the back-end system of reference. Any organisation large enough to want or need an ERP or a CRM is *complex* by definition — so any representation of that organisation and how it does business is going to be just as complex. Any simplification leaves out details which might be important. Any criticism of such a system as being overly complex and not user-friendly misses the point: it *is* friendly to its users, it's just that those users are deeply familiar with the organisation, and what they want is a way to operate efficiently within its structure. 

There is absolutely good and bad user experience, or UX, in this world. I literally got my start in the IT industry this way! 

# Story time

I lived in Italy through high school, and in Italy, high school is a morning-only affair — so at the age of sixteen, armed with my teenage brashness, I marched into the front door of the local Apple reseller, and said, basically "I know Macs, give me a job". To their credit, they did not immediately throw me out on my ear: they sat me in a corner with a pile of hand-written warranty slips, which all had to be entered in to a FileMaker Pro database. This, I dutifully did for a few days, before returning to the Powers That Were with a list of complaints about how the database was set up.

Once again, said Powers showed admirable restraint, and told me I had a week to make something better. This, I duly did, with proper tab-ordering, pre-filled menus, context-aware sequences, and more that I have forgotten since. 

The point was that my new GUI was not just *prettier*, it was *more usable*: I could tab-tab-autocomplete my way through entering a warranty slip in less than half the time it would have taken to click around and re-enter redundant information in the old layout.

# Enough ancient history!

Okay, so this was all last century; why would anyone car now?

The point of my new UX is not that it was prettier, nor even that it enabled or sped up some business task — although it was, and it did. The way in which it did that was because the graphical representation in the interface was tied closely to the data in the underlying system and how it was processed.

Delamination of interfaces — the separation of the vibe-coded GUI from the underlying system — breaks that link. This disconnection is superficially good, because it enables people to create interfaces that suit their way of working. However, that disconnect can also be bad, because the back-end system is not set up to support these new consumption models that have grown up entirely separate from it.

![Layers of interfaces](/images/clark-van-der-beken-A1AV-H8ZBaM-unsplash.jpg)

The sorts of Systems of Reference, to go back to the [pace-layering]({% post_url 2016-05-03-Multimodal-IT %}) model, which underpin all of these new engagement models, are all set up and optimised to support certain access patterns. Creating a new consumption pattern is *probably* fine, as long as it remains on the level of a handful of users: the creator and their friends, say. But the system probably cannot tolerate more than a handful of people running those sorts of unpredictable — and unpredicted — queries. 

# What is to be done?

Luckily, the solution is known. GenAI is accelerating and democratising practices which already existed. This means that there are proven ways of dealing with these challenges. The big difference is that, as we heard at Gartner D&A:

> Thanks to AI, we have everyone’s attention.
> The downside is, we have everyone’s attention.

As an industry, we have an enormous opportunity thanks to AI: all of those eat-your-vegetables initiatives about data hygiene and performance optimisation are suddenly on the critical path to the success of key business initiatives.

This is the opportunity to get everyon to adopt good DevOps practice of clean interfaces ands decomposition. It's time to break up the enterprise monolith, because users are already doing it.

The main reason to do this is defensive, to minimise the blast radius of poor developments. After all, even the proponents of these tools admit that [vibe-coded software is often bad](https://www.wsj.com/tech/ai/vibe-coding-slop-ai-tools-e6a99394). And that's fine, if the tools really are as ephemeral as their proponents claim.

The problem is that, in business, there is nothing so permanent as the temporary fix. I fully expect these new tools to stick around, whether voluntarily — because they really do serve a need — or involuntarily — because they get forgotten, still refreshing a dashboard every day that nobody has looked at in years.

It's on us to architect our systems to be able to support these new usage models. It's well past the point where anyone can bury their head in the sand and hope that the new techniques — and the requirements they satisfy — will just go away.

***

🖼️  Photos by [Jr Korpa](https://unsplash.com/@jrkorpa) and [Clark Van Der Beken](https://www.clarkvanderbeken.com) on [Unsplash](https://www.unsplash.com)