---
layout: post
title:  Thinking Two Steps Behind 
date:   2017-01-19 
categories:  cars sales disruption enterprise 
---

![City traffic](/images/unknown_filename.443.png)

In [my day job](http://www.moogsoft.com), I spend a lot of my time building business cases to help understand whether our technology is a good fit for a customer. When you are building a startup business, this is the the expected trajectory: in the very early days, you have to make the technology work, translating the original interesting idea into an actual product that people can use in the real world. Once you have a working product, though, it’s all about *who* can use it, and *what* they can do with it.

In this phase, you stop pitching the technology. Instead, you ask questions and try to understand what ultimate goals your prospective customer has. Only once you have those down do you start talking about what your technology can do to satisfy those goals. If you do not do this, you find yourself running lots of "kick the tyres" evaluations that never go anywhere. You might have lots of activity, but you won’t have many significant results to show for it.

This discipline of analysing goals and identifying a technology fit is very useful in analysing other fields too, and it helps to identify when others may be missing some important aspect of a story.

### Let’s think about driverless cars

Limited forms of self-driving technology already exist, from radar cruise-control to more complete approaches such as Tesla’s Autopilot. None of these are quite ready for prime time, and there are fairly regular stories about their failures, with consequences from the comic to the [tragic](http://www.theverge.com/2016/6/30/12072408/tesla-autopilot-car-crash-death-autonomous-model-s "Tesla driver killed in crash with Autopilot active, NHTSA investigating").

Because of these issues, Tesla and others require that a drivers keep their hands on the wheel even when the car is in Autopilot mode. This brings its own problems, falling into an “uncanny valley” of attention: the driver is neither fully engaged, nor can they fully disengage. Basically it’s the worst of both worlds, as drivers are no longer involved in the driving, but still cannot relax and read a book or watch a film.

These limitations have not stopped much of the commentary from assuming self-driving car technology to be, if not a problem that is already solved, at least one that is *solvable*. Extrapolations from that point lead to car ownership becoming a thing of the past as people simply summon self-driving pods to their location, which in turn causes massive transformations in both labour force (human drivers, whether truckers or Uber drivers, are no longer required) and the physical make-up of cities (enormous increases in the utilisation rate for cars mean that large permanent parking structures are no longer required) - let alone the consequences for automotive manufacturers, faced with a secular transformation in their market.

### Okay, maybe not cars

Self-driving technology is not nearly capable (yet) of navigating busy city streets, full of unpredictable pedestrians, cyclists, and so on, so near-term projections focus on what is perceived as a more easily solvable problem: [long-distance trucking](https://www.wired.com/2016/10/ubers-self-driving-truck-makes-first-delivery-50000-beers/ "Uber’s Self-Driving Truck Makes Its First Delivery: 50,000 Beers").

The idea is that currently existing self-driving tech is already just about capable of navigating the constrained, more predictable environment of the highways between cities. Given some linear improvement, it does not seem that far-fetched to assume that a few more years of development would give us software capable of staying in lane and avoiding obstacles reliably enough to [navigate a motorway in formation with other trucks](http://www.theverge.com/2016/4/7/11383392/self-driving-truck-platooning-europe "Self-driving truck convoy completes its first major journey across Europe").

Extrapolating this capability to the wholesale replacement of truckers with autonomous robot trucks, however, is a big reach - and not so much for technical reasons, as for less easily tractable external reasons.

Assuming for the sake of argument that [Otto](https://ot.to) (or whoever) successfully develop their technology and build an autonomous truck that can navigate between cities, but not enter the actual city itself. This means that Otto or its customers would need to build warehouses right at the motorway junctions in areas where they wish to operate, to function as local hubs. From these locations, smaller, human-operated vehicles would make the last-mile deliveries to homes and businesses inside the city streets, which are still not accessible to the robot trucks.

This is all starting to sound very familiar. We already *have* a network optimised for long-distance freight between local distribution hubs. It is very predictable by design, allowing only limited variables in its environment, and it is already highly instrumented and very closely monitored. Even better, it has been in operation at massive scale for more than a century, and has a whole set of industry best practices and commercial relationships already in place.

I am of course talking about railways.

![Model train](/images/unknown_filename.444.png)

### Get on the train

Let’s do something unusual for high-tech, and try to learn something from history for once. What can the example of railways teach us about the potential for self-driving technology on the road?

The reason for the shift from rail freight to road freight was to avoid trans-shipment costs. It’s somewhat inefficient to load your goods onto one vehicle, drive it to a warehouse, unload them, wait for many other shipments to be assembled together, load all of them onto another vehicle, drive *that* vehicle to *another* warehouse, unload everything, load your goods onto *yet another* vehicle, and finally drive that third vehicle to your final destination. It’s only really worthwhile to do this for bulk freight that is not time-sensitive. For anything else, it’s much easier to just back a truck up to your own warehouse, load up the goods, and drive them straight to their final destination.

Containerisation helped somewhat, but railways are still limited to existing routes; a new rail spur is an expensive proposition, and even maintenance of existing rail spurs to factories is now seen as unnecessary overhead, given the convenience of road transport’s flexibility and ability to deliver directly to the final destination.

In light of this, a network of self-driving trucks that are limited to predictable, pre-mapped routes on major highways can be expected to run into many of the same issues.

### Don’t forget those pesky humans

Another interesting lesson that we can take from railways is the actual uptake of driverless technology. As noted above, railways are a far more predictable environment than roads: trains don’t have to manoeuvre, they just move forwards along the rails, stopping at locations that are predetermined. Changes of directions are handled by switching points in the rails, not by the operator needing to steer the train around obstacles. Intersections with other forms of transport are rare, as other traffic generally uses bridges and underpasses. Where this separation is not possible, level crossings are still far more controlled than road intersections. Finally, there are sensors everywhere on railways; controllers know exactly where a certain train is, what its destination and speed are, and what is the state of the network around it.

So why don’t we have self-driving trains?

The technology exists, and has done so for years - it’s a much simpler problem than self-driving cars - and it is in use in a few locations around the world (e.g. [London](https://en.wikipedia.org/wiki/Docklands_Light_Railway) and [Milan](https://en.wikipedia.org/wiki/Milan_Metro_Line_5)); but still, human-operated trains are the norm. Partly, it’s a labour problem; those human drivers don’t want to be out of a job, and have been known to [go on strike](https://www.theguardian.com/uk-news/davehillblog/2015/nov/05/docklands-light-railway-strike-explodes-driverless-tube-theories) against even the possibility of the introduction of driverless trains. Partly, it’s a perception problem: trains are massive, heavy, powerful things, and most people simply feel more comfortable knowing that a human is in charge, rather than potentially buggy software. And partly, of course, it’s the economics; human train drivers are a known quantity, and any technology that wants to replace them is not.

This means that the added convenience of end-to-end transportation limits the uptake of rail transport, and human factors limit the adoption of driverless technology even when it is perfectly feasible - something that has not yet been proven in the case of road transport.

### A more familiar example?

In Silicon Valley, people are often moving too fast and too busy breaking things that work to learn from other industries, let alone one that is over a hundred years old[^1], but there is a relevant example that is closer to home - literally.

When the Internet first opened to the public late last century, the way most people connected was through a dial-up modem over an analogue telephone line. We all become expert in arcane incantations in the [Hayes AT command language](http://home.intekom.com/option/hayesat.htm), and we learned to recognise the weird squeals and hisses emitted by our modems and use them to debug the handshake with our ISP's modem at the far end. Modem speeds did accelerate pretty rapidly, going from the initial 9.6 kbits per second to 14.4, to 28.8, to weird 33.6, to a *screamingly fast* 56k (if the sun was shining and the wind was in the right quarter) in a matter of years.

![](/images/unknown_filename.445.png)

However, this was still nowhere near fast enough. These days, if our mobile phones drop to EDGE - roughly equivalent to a 56k modem on a good day - we consider the network as being basically unusable. Therefore, there was a lot of angst about how to achieve higher speeds. Getting faster network speeds in general was not a problem - 10 Mbps Ethernet was widely available at the time. The issue was the *last mile* from the trunk line to subscribers' homes. Various schemes were mooted to get fast internet to the curb - or *kerb*, for Americans. Motivated individuals could sign up for ISDN lines, or more exotic connectivity depending on their location, but very few did. When we finally got widespread consumer broadband, it was in the form of ADSL over the existing copper telephone lines.

### So where does this leave us?

Driverless vehicles will follow the same development roadmap[^2]: until they can deliver the whole journey end to end, uptake will be limited. Otherwise, they are not delivering what people need.

More generally, to achieve any specific goals, it is usually better to work with existing systems and processes. That status quo came to be over time, and generally for good reason. Looking at something now, without the historical context, and deciding that it is wrong and needs to be disrupted, is the sort of Silicon Valley hubris that [ends in tears](https://techcrunch.com/2016/08/30/washio-on-demand-laundry-service-shuts-down-operations/).

Right now, with my business analyst hat on, driverless vehicles look like a cool idea (albeit one that is still unproven) that is being shoe-horned into a situation that it is not a good match for. If I were looking at a situation like this one in my day job, I would advise everyone to take a step back, re-evaluate what the actual goals are, and see whether a better approach might be possible. Until then, *no matter how good the technology gets*, it won’t actually deliver on the requirements.

But that doesn’t get as many visionary thinkpieces and TED talks.

[^1]: The old saw is that "In Europe, a hundred miles is a long way; in the US, a hundred years is a long time". In Silicon Valley, which was all groves of fruit trees fifty years ago, that time frame is shorter still.
[^2]: Sorry - not sorry.

***
Images by [Nabeel Syed](http://nabeelsyed.com) and [Darren Bockman](https://unsplash.com/@bockman) via [Unsplash](https://unsplash.com), and by [ronnieb](http://www.therising-sun.us) via [Morguefile](https://morguefile.com)