---
layout: post
title:  Software Is Eating Itself
date:   2026-06-15
categories:  AI cloud open-source SpaceX Anthropic
---

[SpaceX went public](https://apnews.com/article/musk-spacex-tesla-ipo-trillionaire-billionaire-worth-rockets-7723f82b6063a9a17c194e25982cd66d), popped nearly 20% on the first day of trading, and made That Guy a trillionaire. Meanwhile, Anthropic released its Fable 5 model, which is basically [the Mythos model which was previously limited to approved users]({% post_url 2026-04-09-Mythical-Intelligence %}), and it quickly got [banned by the US government](https://www.nbcnews.com/tech/tech-news/anthropic-suspends-new-ai-models-fable-mythos-government-directive-rcna349901).

> This is 100% Anthropic reaping what they have sown:
> 
> “oh no, our AI is too dangerous, it must be regulated” (repeat 1000x, get the pope involved too)
> 
> “…not like that.”

-- [Me on Bluesky](https://bsky.app/profile/theriotnrrd.eurosky.social/post/3mo5kwtshf22v)

So what does it all mean?

If there is a thread running through this blog, it's that there is very little that is new under the sun. Remember the [crypto wars of the 90s](https://en.wikipedia.org/wiki/Export_of_cryptography_from_the_United_States#PC_era)?[^1]

![This shirt is a munition](/images/Munitions_T-shirt.jpg)

What is different this time is the nature of what is being banned. Software used to have zero marginal cost, but in the era of software that is provided "as a service", that is no longer true. From Matt Levine's [*Money Stuff* newsletter](https://links.message.bloomberg.com/s/c/Hv5bhBbJxHkyDIiR30bwmTvBIwks1lB3ms-lPFUZSkP9du423c34_VPguuNDyfxXdSCNeo7DGDpXchDlANf1PFpUwFfLRtbhpKMtD7KLKiReRUgKX1VQaxYtrrZeSHKKxxdUWh69TBQQF2oDpcZvTqMIjDas4hmu4Togfx20_57yIa4cE3naDdI_Qty-5wVtfpf8LnrmIoH4R7yK9bBD-EEcTNmT6sEt_vOq_oQFIpFiN9-LCwOGlsDIjfnyS5mmvcuvsGffQ2IHfmjDlIp7oQnlrBYuxb3e_TH4Jk3IqcKrwWkwKz9MEo7xk02cybu-nSeEHutPqgmRDnR5cBAtIuXxTqG5jEVdab3FbjLzh4nkhB4AKfvrXCIK0Q/a9QMpN_jvMQYHqoKB_lR5WPUlFCRQUPS/21):

> A lot of the biggest and most successful companies now are [_enormously_ capital-intensive](https://links.message.bloomberg.com/s/c/0r36sM1kxNI0y5w6sE2JDeo19-TNLUPCDgN_-XLATWFU99nQkbI2zrTZISr26pwTYGvwwq5Vk_-VI2Kliue6obTlj9JiC3-kjCf-CxIwCqHQhi5DIxJBacRXnFVSO8OVwqk4dZZze5VKqBnXC9ReGpexw9AeZ1r5BVwraX8sWUpQ834aOeKhIVNcJJNROGPgjUziTLMRZ318BgAVALDpnJPFKTmKn0BGsZadjhJo-7T6p3On5KOFMqlEuTT5fh4mqU_Kdt_r75ybhskOD8U1yCDBnNd16K_gzvxpvExyVgpw4jJIB8UZ342uxPH76oOzwM7rNPG0YuS6N47sWhdw-csdmHvA05Xuo-x353h9IDc1U47cFWZ8V7Wif9I/KueOFzj3V1Vzuy25mkfdUoIi7A7Dq_Dx/21). They are artificial-intelligence hyperscalers, and their business model is like “build nuclear power plants and orbital data centers and massive chip fabrication facilities.” After years in which the cutting edge of the economy was nearly zero-marginal-cost software, now the cutting edge of the economy is extremely capital-intensive, uh, [software](https://links.message.bloomberg.com/s/c/lkH_MALJguBz8Xssl5QddOnCEcjEooP-8TKJVomb7CMqHhdlRahGVWoU-1mHuJDlE1GFEAsyV8TH7Ls9zV8jMak8ZMuf2DFoPgfnrFtCFMcmgkOvkSXQMgq75aIuinohY2kRH5ZI5WCo2Lo_-T6Ma-wNVTT-pxLs7-HZPdan-f6rG_SHdPGbcaxTTIi_-ILjv2ey4fYaWOWa4vEEH-7WDw7CChSlmh-4w1a0kuGPLhDr4qQRVsMviKfGDbZfnU5FeSBRgtrvfBj46oNRFa9FjVA8sX0MmopzEe-_vEvgjGqxmSPMomkIXtp6nAsIS1Rq9mGxHckO_1pUgu39Z2tDmV78Z2G_-ET9ZfAWXj8c6HKOQ5vA7fzfcO5g1M4/LKQVG8LyCcfNxQKmHQUY00S_cGBkkRiH/21).

All of that capital outlay only makes sense if it is matched by a proportional revenue stream. This is [the Sam Altman thesis](https://gizmodo.com/sam-altman-says-intelligence-will-be-a-utility-and-hes-just-the-man-to-collect-the-bills-2000732953): "We see a future where intelligence is a utility, like electricity or water, and people buy it from us on a meter."

![An electricity meter](/images/dylan-michaud-nEwgrvIwmw4-unsplash.jpg)

The problem with meters from the point of view of users is that *they keep running*, as Uber found out when [developers blew through Uber's entire 2026 AI token budget in just four months](https://www.forbes.com/sites/janakirammsv/2026/05/17/uber-burns-its-2026-ai-budget-in-four-months-on-claude-code/). A mystery company reportedly [spent half a billion dollars on Claude Code in a single month](https://www.fastcompany.com/91550884/claude-ai-costs-climb-company-spent-half-a-billion-dollars-in-a-single-month-report).

# Scale to zero — or to the stars

This problem of open-ended cost structures is not a new one that is specific to AI. The most recent iteration of the billing dilemma was in serverless platforms. 

Cloud software is roughly divided into three layers:

- **IaaS**, or Infrastructure as a Service: basically, virtual servers in the cloud. Apart from them running in someone else's datacenter, these behave like normal servers: you log into them directly, deploy software, reboot them, and so on. Your bill is for a certain number of servers.
- **SaaS**, or Software as a Service: you have no idea where the software is running, you just connect via a web browser and get to work. Your bill is for a certain number of users, or "seats".
- **PaaS**, or Platform as a Service: this is an intermediate level of abstraction, where you are not connecting directly to a server, but to application software running on top of one or more servers. The details are not important or even visible to you; it's just "compute" (short-hand for "computational power/capacity"), but your bill might still be for a certain number of servers.

Serverless billing applies to that last model. The idea is that, since with PaaS you don't access the servers directly, you should just pay for however much platform capacity you use, rather than for a fixed pool of capacity, as you would with per-server billing. This approach is pitched as being particularly attractive to startups: you don't know if your offering will take off, so you don't want to commit to high up-front costs — and if you do hit the big time and your thing is blowing up, you don't want to be constrained by capacity.

Here's the catch: serverless compute is *significantly more expensive* than pre-purchased units of compute billed as servers. The reason is that the risk of paying for idle capacity doesn't go away, it just gets transferred from the hopeful startup to the cloud provider. Of course the cloud provider is aggregating demand and betting that no more than a certain portion of its customers will suddenly need a whole lot of compute capacity at once, but they are also charging a risk premium for their trouble. Basically, it's an insurance model.

This means that if you do know your demand profile, you are better off *not* using the metered serverless model, but instead pre-purchasing the capacity that you know you need. You may even be able to mix and match, with baseline guaranteed capacity at one price point and a buffer on top that is charged at surge pricing rates if it turns out that you do need it.

But right now that is not how any of the frontier models work. They consume "tokens", and they do so at a rate that is not always easy to predict, and which can be affected by non-obvious architectural choices.[^2] In other words, the meter is always running.

# What if you don't have coins to feed the meter?

The problems extend beyond commercial software. At least in that world there is a revenue stream. As long as the token budget is less than the revenue which the token burn enables, the business case still stands up. But what about open-source software, or other non-commercial models? It's one thing for coders to donate their time to projects, but even then, many projects are in trouble, with volunteer maintainers struggling to pay the bills even for projects that are foundational to many companies' operations.

![The famous XKCD cartoon about all modern digital infrastructure relying on a project some random person in Nebraska has been thanklessly maintaining since 2003 https://xkcd.com/2347/](/images/xkcd-2347-dependency_2x.png)

If widespread use of code-generating AI tools becomes the norm, and those tools burn through enough tokens that working on them comes at substantial financial expense, that equation starts to become impossible. This is [one of the problems with Anthropic's Mythos bug-finding AI model]({% post_url 2026-04-09-Mythical-Intelligence %}): *finding* a bug in a piece of open-source software is one thing, but *patching* it with AI tools would require a bunch of tokens, which a volunteer-run organisation may not have immediately available. And that does not even touch on the problem of *deploying* a fix once it has been developed, which may be especially hard for open-source components that are embedded deeply in other offerings.

# Watching the meter

This is why it is particularly interesting that [S&P Dow Jones Indices decided against fast-tracking SpaceX, Anthropic, and OpenAI into the S&P 500](https://www.fool.com/investing/2026/06/06/spacex-anthropic-openai-ipo-sp-500-2026/). The S&P 500 is what many index funds use; if OpenAI et al are not in the index, they do not have access to funds invested that way. The reverse is also true, of course, but investors always have the option of buying stock in those companies *actively*; the whole point of index funds is they are *passive*, and their investors don't really want to worry about the contents of the fund on a day-to-day basis, or whether some overweight proportion of it is suddenly a massive bet that an unprofitable endeavour can become profitable within a reasonable timespan. 

This choice by the S&P has been characterised as a bet against these companies making it; I am far from an investment professional, but I read it instead as a refusal to be bounced into making an exception on the basis of hype. Once these companies have been publicly traded for a year in a process called "seasoning", they can be considered for inclusion in the S&P 500 index. 

![A taxi meter](/images/simone-dinoia-FXu9jE6AJVU-unsplash.jpg)

The reason to take this "wait and see" approach is that the thesis of companies and individuals continually topping up the meter on these AI services is far from proven. With more and more stories coming out of spiralling token bills, there is now a drive to [manage AI’s runaway costs](https://techcrunch.com/2026/06/05/the-token-bill-comes-due-inside-the-industry-scramble-to-manage-ais-runaway-costs/):

> “In April and May, I started hearing from companies: ‘Oh my god, we are 3x over our entire 2026 token budget and it’s only April,’” J.R. Storment, executive director of the FinOps Foundation, a project under the Linux Foundation, told TechCrunch. “We started hearing existential crises, and the whole conversation shifted from [tokenmaxxing](https://techcrunch.com/2026/04/17/tokenmaxxing-is-making-developers-less-productive-than-they-think/) and ‘go fast’ to ‘we need guardrails, how do we control this?’”

The big AI labs' problem is that AI has advanced enough that many AI tasks do not need the latest and greatest frontier models. Marco Arment, creator of the Overcast podcast app, [built a transcription service for *every podcast on Earth* using a rack full of Mac Minis](https://appleinsider.com/articles/26/04/07/giant-mac-mini-cluster-powers-overcast-podcast-transcripts-without-the-cloud) — and the base model, at that. Sure, Marco had to come up with the up-front cost of the hardware, but he doesn't have to worry about huge open-ended costs for using a metered service forever. 

This sort of offline usage is a problem for the business model of the frontier labs precisely because it does not generate the ongoing ever-growing token revenue which their stock market valuation is built on.

# But what about regulation?

Offline AI models are also the reason why any attempt at AI regulation that assumes the ability to prevent certain uses, or its use by certain groups, is doomed to failure. That doesn't mean regulation is not worth doing, mind: it's perfectly reasonable to say that the Instagram app should not have a built-in feature to "nudify" pictures that people post there. On the other hand, we should also not expect that a ban on AI features like that, or on entire hosted models like Fable 5, will eliminate abuse entirely. The reality is that bad people will continue to find ways to be bad. There probably do need to be controls on AI, but more in the way that we have controls on fertiliser, enforcing regulation and tracking at the point of sale.

The US Government can ban Fable 5 because it is provided as a service, which means there is a single point of access which can be blocked: Anthropic's servers themselves. The attempt to ban PGP in the 90s failed because there was no one place you had to go to get PGP, and once you had it, you didn't have to go back to the source every time; you could use your local copy of PGP entirely offline. But because ["AI" models don't have a moat]({% post_url  2026-04-14-Compute-Me-A-Moat %}), a ban on Fable 5 only buys a little bit of time until some other model which can be run offline achieves comparable performance.

Regardless, the lack of clarity around what the future usage patterns for the frontier AI models will be is the reason why the S&P 500 is not taking on the AI bet, or at least, not right now. They want to let things play out for a year, and then see what happens. The Fable 5 ban, regardless of its specific merits, justifies that caution, as it implies that government regulation of the AI market is a very real possibility.

And if you really do want to buy stock in SpaceX, Anthropic, and OpenAI in the meantime, you still have the choice of going and doing that directly, actively, rather than have it included willy-nilly in a passively-managed index fund, at least while the future outcome is still so uncertain.

*** 

🖼️  Photos by [Dylan Michaud](https://unsplash.com/@dylan_michaud) and [Simone Dinoia](https://unsplash.com/@simonedna) on [Unsplash](https://www.unsplash.com)

[^1]: You know, back when "crypto" meant something good and useful to society.
[^2]: Yes yes, you can pre-purchase tokens at some discount, but the mechanism of token consumption is still very opaque, and the use-it-or-lose-it ratchet is much more aggressive than most of the existing cloud pricing models. It's more of a financial arbitrage than a meaningfully different pricing model.