---
layout: post
title:  Dog Bites Man
date:   2026-06-08
categories:  AI work
---

There has been a lot of talk over the years about how new tech-sector jobs can compensate for jobs lost in other sectors of the economy. The latest wheeze is [Keir Starmer, UK PM, telling us that data centres will replace closing factories](https://www.bbc.com/news/live/cr5j43zp2rpt?post=asset%3Aa9404349-9816-4c67-89d4-a51081917eb5#post). I do not think that bet will pay off; one of the reasons that [everyone hates AI datacenters]({% post_url 2026-06–04-Everyone-Hates-AI-Datacenters %}) is that they do not actually bring all that many jobs:

> We are not quite at the point of the proverbial datacenter staffed by a man and a dog — the man to feed the dog, the dog to bite the man if he touches anything — but we are not far off. A datacenter has probably the worst ratio of on-site employment to surface area out there. There are going to be a handful of security guards (not exactly skilled labour) and a handful of on-site techs to deliver the “remote hands & eyes” service, and that’s it.

In online conversation about this topic, this Brookings report came up: [*New evidence on data center employment effects*](https://www.brookings.edu/articles/new-evidence-on-data-center-employment-effects/). Superficially, it seems to contradict my assertion above, but I think it’s worth digging into why (as usual!) it’s a bit more complicated than that. Handily, the report includes a short list of takeaways, so I will go through those in order.

![Person working on two laptops](/images/freestocks-I_pOqP6kCOI-unsplash.jpg)

> 1. **Data centers do create local jobs,** though fewer than industry advocates claim. Naive estimates that fail to account for preexisting growth trends overstate the effect by a factor of three.

In keeping with the Brookings Institutions’ centrist positioning, the report begins by pointing out that many datacenters[^1] are placed in locations that already have good growth trajectories, so simply counting the marginal addition of employment from adding a datacenter to a vibrant local economy is overly simplistic and unlikely to be replicated elsewhere without that existing support base. 

> 2. **Not all data centers are equal.** The technology ecosystem effects that distinguish data centers from warehouses are concentrated in hyperscale investment. Colocation facilities generate construction activity but not the IT  agglomeration that makes data centers a distinctive economic development tool.
> 3. **Clusters generate the largest effects.** Single facilities produce modest employment gains. The information sector benefits require multiple facilities in the same area.

These two points are related, so I will address them together. Almost the entirety of gains in employment come from locations where at least one of the following conditions is true:

- The datacenter is used by a hyperscaler, not for simple colocation 
- The datacenter is part of a cluster of at least four local facilities

I would argue that the reason is the same: the jobs are not coming from employment in the datacenter itself, which is still staffed by the man and the dog. All of the jobs come from the *ecosystem* surrounding the datacenter. If you are building the first datacenter in an area, you might hire local construction crews, but for anything more specialised, you bring in specialised contractors from outside. Once the construction is done and the outside specialists have departed, you got a brief blip in the local hospitality sector, plus whatever property taxes and other fees you didn’t negotiate away to attract the datacenter in the first place, and that’s pretty much it. 

![IT factory worker](/images/tecnic-bioprocess-solutions-RyMTGAYZpjY-unsplash.jpg)

This assessment is backed up by the UK government’s own research, in the shape of a report titled [*Data centres: planning policy, sustainability, and resilience*](https://researchbriefings.files.parliament.uk/documents/CBP-10315/CBP-10315.pdf).[^2] The report admits that “the number of people employed at data centres is uncertain due to a lack of official statistics”, but ends up settling at a calculation of 54 FTE jobs per site.

The ecosystem jobs are on top of that employment, but only really materialise once there is enough of a local centre of gravity to attract them. I suspect that the two situations listed above are actually the same, because hyperscalers mostly do not just drop a single datacenter on its own. Microsoft and Google have been known to make exceptions to the rule, but if AWS sets up a region, it always starts from three availability zones, each of which requires at least one datacenter facility. While the three AZs are by design somewhat distant from each other, they are still within the same general area — say, Virginia for the infamous us-east-1 region — meaning that a local ecosystem can be jump-started to serve those three facilities.

In other words, the key distinction is not whether a particular facility belongs to a hyperscaler, but the absolute number of physical datacenter facilities in the area, and the fact that a hyperscaler datacenter is almost always close to at least two other similar facilities. From the point of view of a contractor laying cable or whatever, it doesn’t really matter who owns the endpoints, just that there is a certain ongoing base level of demand for their services.

> 4. **Workers see modest real gains.** Wages rise 3%-4% for both existing workers and new hires, with no significant effect on home prices.

Again, not surprising. The highly-payed AWS jobs are back in Seattle (especially with the ongoing roll-back of remote-work), not out in the provinces. Those local jobs, while they do exist, are mostly blue-collar tech work, dealing with messy physical infrastructure, not the glorious abstractions that it supports.

![Piles of coins](/images/towfiqu-barbhuiya-jpqyfK7GB4w-unsplash.jpg)

> 5. **Incentives may be poorly targeted.** Overall, state incentives are small relative to private investment. In hyperscale counties, incentives represent about 2% of total construction investment. Location decisions for these facilities are driven by power availability, land, and fiber infrastructure, not by tax breaks. In colocation counties, incentives represent a much larger share of total investment (62%), meaning subsidies may matter more for precisely the facilities that generate the smallest employment benefits.

This is my contention overall, both at the local level, and even at the national level. Sure, I’ll grant Keir Starmer that it’s better to have a datacenter than just the shell of an empty factory — but not by as much as you might think, and a lot of the benefits are shipped overseas. The hardware comes from US companies, and if the datacenter is used for AI, so do the AI models, and all the revenue from them. It is far from clear where the benefits are to British companies from having this facility — and if those benefits do exist, surely the market would cause it to be built anyway. The one reason for governments to support such a build would be competition, if e.g. there were going to be one AI datacenter for Western Europe, and British companies would benefit from it being in the UK rather than somewhere on the Continent. But that does not seem to be the case here.

If on the other hand the goal is “digital sovereignty”, then the EU has the better approach, as it works to [strengthen Europe’s tech sovereignty](https://commission.europa.eu/news-and-media/news/strengthening-europes-tech-sovereignty-2026-06-03_en) by working simultaneously at all levels of the stack:

- Semiconductors, with the “Chips Act 2.0” aiming to boost the EU semiconductor strategy and reduce strategic dependency
- R&D, with the “Cloud And AI Development Act” aiming to develop competitive sovereign options in cloud and AI
- Software independence, with an explicit strategy to foster and adopt open-source alternatives to US providers
- Integrating energy strategy to ensure new datacenters do not unbalance or overwhelm electricity grids and other infrastructure

That is a far more ambitious and longer-term roadmap than just cutting a ribbon on a new datacenter and declaring “mission accomplished”, but it does hold out the promise of actually making a difference.

***

🖼️  Photos by [freestocks](https://freestocks.org/), [TECNIC Bioprocess Solutions](https://tecnic.eu/), and [Towfiqu barbhuiya](https://unsplash.com/@towfiqu999999) on [Unsplash](https://www.unsplash.com)

[^1]: Yes, I still have no idea how to choose between US and UK spelling. It doesn’t help that I have long ago capitulated and set my work devices to US spelling, because it all just got edited to US preferences anyway.
[^2]: The report incidentally also backs up my point that water use by AI datacenters is a red herring: “An accurate assessment of a data center’s water use — and its effects on communities and the environment — must examine local restrictions on water use, competition for water, the watershed’s safe withdrawal rate, the cooling system type, and climatic conditions at a given location.”