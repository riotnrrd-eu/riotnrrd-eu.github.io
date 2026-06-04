---
layout: post
title:  Everyone Hates AI Datacenters
date:   2026-06-04
categories:  AI
---

According to a recent Gallup poll, it seems that [*Americans Oppose AI Data Centers in Their Area*](https://news.gallup.com/poll/709772/americans-oppose-data-centers-area.aspx), even as we read that ["A JPMorgan analysis last month found that more than 60% of data-center capacity planned for completion in 2027 isn’t yet under construction, and another 7% is delayed."](https://www.wsj.com/tech/ai/americas-data-center-build-out-is-falling-way-behind-schedule-e408a9a8).

I think it's worth digging into the reasons for their objections to understand the current state of the public perception of AI.

# Water, water everywhere

The most frequently cited category of objections is "Effect on resources"; the sub-category of "Water/Excess water usage" heads the list, cited by 18% of respondents who oppose datacenter construction. Now this is a weird one, because of all the many possible objections to AI, water consumption seems to be the one that has taken off with the general public. It's weird because this is the *least substantiated objection to AI*.

We could talk about IP theft, or the dangers of financial bubbles, or the potential effects on the job market, or all sorts of other legitimate concerns — but no, it's always "AI datacenters will take all our water".

![Parched earth](/images/dan-gold-H0Jp8pX-0zw-unsplash.jpg)

It is true that many AI datacenters are cooled by water, due the extreme thermal demands of the GPUs that power the models, but those cooling systems are moving from evaporative cooling, which does "consume" water through evaporation, to closed-circuit systems, which do not. There are even systems coming online that run on recycled waste-water, as well as [attempts to formalise existing best-practice standards around water management](https://www.msn.com/en-us/news/technology/google-pushes-water-standards-amid-data-center-backlash/ar-AA24IOcb). 

Datacenters also do not pollute the water they use; it's not like having a plastics manufacturer or a tannery in your town. At worst, even evaporative cooling does return the water to the usual water cycle — which is no consolation if you're in a drought situation, but it's not as if the water is lost for ever. For a more academic treatment of the topic, see this ACM article [Making AI Less 'Thirsty'](https://dl.acm.org/doi/10.1145/3724499).

The most concrete problem seems to be the cases where permits have been granted to construct datacenters in places where water supply was constrained to begin with — but that is a problem with the local permit system. The canonical example seems to be this one, where [a data center guzzled \[sic\] 30 million gallons of water](https://arstechnica.com/tech-policy/2026/05/data-center-used-30-million-gallons-of-water-without-initially-paying/):

> On Friday, Politico reported that one of the country’s biggest data center developments had guzzled nearly 30 million gallons of water without paying for it. Even worse, the water grab came at a time when nearby drought-stricken residents were warned to restrict their personal water consumption, and some reported sudden decreases in water pressure.
> 
> QTS eventually paid about $150,000 for the water, but there were no consequences for exceeding peak limits established by the county during the data center planning process. Frustrating residents, the county declined to fine QTS. Fayette County’s water system director, Vanessa Tigert, told Politico that the decision was partly because the county blamed itself and didn’t want to offend QTS. “They’re our largest customer, and we have to be partners,” Tigert said. “It’s called customer service.”

# Jobs for the boys

I am not at all clear what value the county is expecting to get from its "largest customer". It's certainly not local jobs, although 55% of the survey's respondents who were in favour of datacenter construction in their area are also hoping for "Job opportunities". I hate to disappoint these hopeful people and the government of Fayette County, but that is simply not going to happen. 

![A man working in a datacenter](/images/jesse-orrico-RBWDrxW3xog-unsplash.jpg)

We are not quite at the point of the proverbial datacenter staffed by a man and a dog — the man to feed the dog, the dog to bite the man if he touches anything — but we are not far off. A datacenter has probably the worst ratio of on-site employment to surface area out there. There are going to be a handful of security guards (not exactly skilled labour) and a handful of on-site techs to deliver the "remote hands & eyes" service, and that's it. Any logistics warehouse will generate far more local jobs. All of the economic value produced by the datacenter is going to be accrued by its remote users and operators, not by the local community, apart from some small amount of taxes — which are anyway set on the physical building, not its valuable contents, and often deferred or offset as part of attempts to attract the datacenter construction in the first place.

# Generators of AI

By comparison, the entire "Pollution" category is only cited by 16% of respondents to the Gallup survey, with the leading sub-category of "Noise/Noise pollution" only coming in at 9%. This objection is far more substantiated, with the best-known case being that of [OpenAI's datacenter in Memphis that is pulliting and deafening residents](https://www.theguardian.com/technology/2026/jan/15/elon-musk-xai-datacenter-memphis). Since the operators could not get sufficient electrical power from the grid, they ran the whole facility on generators 24/7. 

Generators are noisy and polluting; they are typically designed for emergency use, such as if grid power is lost, or in remote locations, where grid power is unavailable. Running them full-tilt all the time in the middle of a residential area is not at all neighbourly. [Anthropic has now leased the entire site](https://www.idlen.io/news/anthropic-spacex-colossus-memphis-300mw-gpu-deal-2026/), but it remains to be seen whether the generators will scream on.

![Obsolete machinery](/images/philippe-krief-m9BgiVb7DGA-unsplash.jpg)

# The future of datacenters

There is also the question of the future value of the datacenters if and when the AI bubble pops. AI enthusiasts love to head off any criticism of AI by comparing its current state to the early days of the web, and this is no exception: they claim that, while telcos did indeed go bust building out fibre-optics projects, that "dark fiber"[^1] did eventually come in useful and got lit up over the subsequent decades. 

The problem is that, while a datacenter's physical plant may have value for years or decades, the GPUs it contains have a very short half-life before they become obsolete. The GPUs in that Memphis datacenter are already on the downward part of the curve: while we do not know the precise breakdown of the chips that make up the [Colossus](https://en.wikipedia.org/wiki/Colossus_(supercomputer))[^2] installation, it is known to have started out with 100.000 [Nvidia H100 chips, first announced back in 2022](https://www.theverge.com/2022/3/22/22989182/nvidia-ai-hopper-architecture-h100-gpu-eos-supercomputer).

The [rapid obsolescence of AI chips is why they cannot be a competitive moat for operators]({% post_url 2026-03-31-Networked-Intelligence %}), even as they struggle get hold of [enough chips to fill new datacenters]({% post_url 2026-04-14-Compute-Me-A-Moat %}). The current shortage does explain why a bunch of four-year-old chips still have value for Anthropic, but it still doesn't mean that sitting Smaug-like on a massive pile of GPUs is a viable long-term strategy.

The whole saga just emphasises the short-term nature of much of the planning in this space. Get in quick, get your bag, and get out even quicker, seems to be the operating model. Given that, it's perhaps not surprising that the general public is opposed to projects which seem to have significant and immediate downside, and very little discernible upside — even if the fixation on water usage does not seem to be the most salient problem.

***

🖼️  Photos by [Daniel Gold](https://www.danielcgold.com/), [jesse orrico](https://jesseorrico.com), and [Philippe Krief](https://unsplash.com/@phkrief) on [Unsplash](https://www.unsplash.com)

[^1]: Yes, I am now terminally confused by how to manage spelling differences between British and American English. My brain is perpetually stuck in the middle of the Atlantic somewhere, buffeted back and forth by forces beyond my control.

[^2]: Seriously with the hubristic names? Plus there already was a [Colossus computer](https://en.wikipedia.org/wiki/Colossus_computer), which actually did deliver a lot of value for humanity.