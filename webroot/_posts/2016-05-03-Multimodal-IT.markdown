---
layout: post
title:  Multimodal IT 
date:   2016-05-03 
categories:  enterprise bimodal 
---

# Multimodal IT


![|1080x720](/images/unknown_filename.239.jpeg)

The current big debate in Enterprise IT (now that we have mostly moved on from arguing about hybrid cloud) is [Bimodal IT](http://www.gartner.com/it-glossary/bimodal).

To recap: the idea is that enterprises will have both stable and predictable services, sometimes unkindly referred to as "legacy", and new, unpredictable services just being developed. These two types of services have different priorities and expectations: the former focus above all on reliability and availability, while the latter instead need to deliver quickly on new requests, evolving rapidly by definition. These differing requirements are sufficiently at odds that - so the theory goes - they should be split off and operated by two different teams.

So far, so good. The [objection](http://blog.gardeviance.org/2015/10/if-you-really-want-bimodal-then-youll.html "If you really want bimodal then you'll need to give something up." ) is that few people will want to work on the "legacy" services, preferring to hone their skills on more cutting-edge, trendy technology. Over time, this will hollow out the legacy support team, undermining its mission of quality and reliability.

![|1080x865](/images/unknown_filename.240.jpeg)

## Why it’s not that simple

Personally, I think both positions are over-simplifications. First of all, mainframe people aren't dinosaurs; they're just solving for a different set of variables (Simon Wardley’s Town Planners). I've been in the room when someone was presenting version 56 (!) of a mainframe product, and people were excited to hear about what it could do for them and how it could improve their jobs. Also, the idea that there are no jobs to be had on the mainframe side of the house is rubbish: it's a niche, sure, so absolute numbers are low, but if you specialise in that niche, it can be very profitable. The first person in my graduating class to get a job - in the teeth of the post-bubble, post-9/11 *complete lack of IT jobs* - was a friend of mine who had been one of the few to take the COBOL class.

Secondly, the Bimodal IT picture is a snapshot of a moment in time. To extend bimodal to [the classic three modes of Pace Layering]({% post_url 2014-04-16-Tech-in-Layers %}): right now, mainframes are systems of record, classic ERP middleware represents systems of differentiation, and the new DevOps-Agile-Web 2.0-whatever brings the systems of innovation. Over time, though, things flow down the stack and sediment at lower layers. SQL used to be the neat new thing that had all the promise. Now? Now everyone scoffs at relational databases and the cool kids at the conferences are all about the NoSQL. Meanwhile, all of those relational databases are still humming away, keeping everything up and running.

This looks a little like fossilisation: the dynamism of a freshly-introduced service dries up, because it's generally not a good idea to change the foundations too much once you have started building on top of them. Messing around with foundations is a major effort, and the sort of thing that [makes the news](http://www.swissinfo.ch/eng/multimedia/massive-zurich-building-completes-19-hour-trip/32745688 "Massive Zurich building completes 19-hour trip" ).

![|480x270](/images/unknown_filename.238.gif)

As a rule, you want to put your efforts into making those foundational systems as stable and reliable as possible. This will ensure that the layers further out are free to innovate on top of those solid underpinnings. The whole point is that nobody worries about the database being up, they focus on how to query it and what to do with the results.

![|1080x720](/images/unknown_filename.241.jpeg)

## Innovation trickles down

What all this means is that instead of treating this conversation about Bimodal IT as an argument between Old and New, we need to pull back and focus instead on the lifecycle of individual services. Once we have an idea of which systems of innovation are catching on and making the transition to systems of engagement and record, we need to start taking decisions about how we treat those systems and allow for their dependencies. Today’s fast-moving top of the stack is tomorrow’s mid-stack connective tissue and next week’s bottom-of-stack foundation element.

The good news is that none of this should be new. Interestingly, the two extremes have more in common than the centre, if you squint a little. Both mainframes and modern distributed services share a focus on small units of work, defined interfaces and checkpoints, and no assumption of reliability on the part of other components in the pipeline. Arguably, the intervening generation of relatively monolithic and rapidly-obsolescent enterprise IT is the aberration.

Jez Humble articulated this point in [a widely-shared piece](http://continuousdelivery.com/2016/04/the-flaw-at-the-heart-of-bimodal-it/ "The Flaw at the Heart of Bimodal IT" ):

> Gartner’s model rests on a false assumption that is still pervasive in our industry: that we must trade off responsiveness against reliability. The conventional wisdom is that if we make changes to our products and services faster and more frequently, we will reduce their stability, increase our costs, and compromise on quality.
>
> This assumption is wrong.

The responsiveness-reliability dichotomy is a product of fragility. The attitude of "if it ain’t broke, for pity’s sake, *don’t touch it!*" comes from [knowing that the whole thing is a massive pile of cards](http://www.stilldrinking.org/programming-sucks "Programming Sucks" ):

> Right now someone who works for Facebook is getting tens of thousands of error messages and frantically trying to find the problem before the whole charade collapses. There's a team at a Google office that hasn't slept in three days. Somewhere there's a database programmer surrounded by empty Mountain Dew bottles whose husband thinks she's dead. And if these people stop, the world burns. Most people don't even know what sysadmins do, but trust me, if they all took a lunch break at the same time they wouldn't make it to the deli before you ran out of bullets protecting your canned goods from roving bands of mutants.

Fortunately, this situation is now the base assumption of any sane IT architect. IT used to work to grandiose Soviet-style Five Year Plans:

> IT will firmly implement the CIO's new strategy, new concept and new mission, promote structure adjustment, layout optimisation, and transformation and upgrading, as well as insist on green power strategy, overall lean management, staff innovation and creation, harmonious development, profit increase and strengthen the <del>Party</del> enterprise construction in an all-round way in order to further solidify production safety foundation, speed up the development method and mechanism adapting to the "new normal", and go all out to launch IT’s innovative and balanced development of the "13th Five Year Plan to update the CMDB" successfully.[^1]

Today, we work with what we have, and assume that will change - often in unpredictable ways, since the IT department is no longer the gatekeeper of IT adoption in the company.

![|1080x721](/images/unknown_filename.242.jpeg)

## People, Process, Technology

Technological solutions are emerging to help with this transition. My own employer, [Moogsoft](http://www.moogsoft.com "Moogsoft - IT Operations Analytics" ), is part of this trend, helping to bring monitoring data from all the different tools and systems in the enterprise together in a way that is comprehensible and actionable for humans.

As usual, though, the technology is the easy part. The hard parts are the people using the technology, and the process according to which they do so.

I already hinted at one people problem: if you divide IT into the Cool Kidz and the Old Fuddy-Duddies, pretty soon you’re going to run out of people to take care of the mainframes (or SAP, or Oracle, or whatever tech is actually running big chunks of your business). Also, you’ll find that suddenly consultants in that area have added a zero to their hourly rates, and are booked up for months in advance.

A process problem is that you simply cannot freeze even the systems of record, as the faster-moving systems still need to interface with them to get their job done, and will require changes. Maybe you can’t do two-week sprints, especially if your release process itself takes a fortnight, but you still need to allow for that continuous delivery process. Otherwise, the change you can’t accomodate in-band will happen out-of-band when management starts screaming, and it doesn’t take too many of those before something breaks.

To quote Antoine Lavoisier:

> Dans la nature rien ne se crée, rien ne se perd, tout change.

Or in our world:

> In <del>nature</del> IT nothing is created, nothing is lost, everything changes.

Change is in the nature of the beast. Let’s sit down together and figure out how to accomodate it.

***
Images by [Vladimir Chuchadeev](https://unsplash.com/@chuchad), [Patrick Tomasso](http://patricktomasso.com), [Erol Ahmed](http://instagram.com/erol_is/) and [Gabriel Garcia Marengo](http://photo.gabrielgm.ch) via [Unsplash](https://unsplash.com)

[^1]: only very lightly paraphrased from [here](http://www.shanghaipower.com/power/nr/mn/201603/t20160311_26356.html).

                              