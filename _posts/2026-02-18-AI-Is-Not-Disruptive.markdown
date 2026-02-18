---
layout: post
title:  AI Is Not Disruptive
date:   2026-02-18
categories:  AI Spotify
---

Noah Smith writes over at the [Nazi bar](https://www.theguardian.com/media/2026/feb/07/revealed-how-substack-makes-money-from-hosting-nazi-newsletters) that [*You are no longer the smartest type of thing on Earth*](https://www.noahpinion.blog/p/you-are-no-longer-the-smartest-type):

> Vibe coding is taking over _fast_. Spotify’s co-CEO [recently revealed](https://x.com/sarthakgh/status/2022145859996254630) that the company’s best developers don’t write code anymore. Some journalists from CNBC, with no coding experience, [vibe-coded a clone of the app Monday](https://www.cnbc.com/2026/02/05/how-exposed-are-software-stocks-to-ai-tools-we-tested-vibe-coding.html), and the company’s stock price [promptly crashed](https://finance.yahoo.com/news/monday-crashed-ai-built-product-214856201.html). 

Here's the thing that trips me up about a lot of the "AI" hype. Where is the actual **product**?

If you think that, because you cloned Spotify's GUI, you now have a competitor to Spotify… well, I wanted to get snarky, but I honestly don't think anyone who would think that would comprehend snark, and I don't need to be hauled up in court for trying to sell someone the Brooklyn bridge.

![You still need software engineers even if the AI is generating most of the code.](/images/claude-hiring.jpeg)

Spotify's co-CEO is excited about AI generating code because it stands to reduce his costs. He can either have the same amount of developers produce more code, or get rid of some of the developers while maintaining the same level of code output. Either way, Spotify's cost per feature goes down.[^1] That in turn gives Spotify the option to continue to charge users the same amount, increasing margins, or to return some portion of the savings to users in the form of lower costs if there is a need to defend against competitors — while still preserving their margins.

None of these mechanisms apply to this vibe-coded ersatz Spotify. Sure, they have a GUI; well done. That does not even begin to answer the questions any would-be competitor to Spotify would have to answer:

- Does it work equally well across all platforms?
- Does it work equally well in all languages?
- Does it scale to a billion users?
- Is it secure against fraud, whether by users or artists?
- And the big one: does it have access to a decent library of music, at least comparable to Spotify?

Without those, what those journalists built is *nowhere near* being a replacement for Spotify — not because of anything to do with how it was created, but because it is not a complete product. My undergraduate final year project at university was more of a product than this is, because I had put a lot of thought into the back-end and the architecture, not just thrown together a web UI and gone to the pub.[^2]

It was the *Financial Times* that kicked off this round of "software is dead", and I think [the follow-up piece](https://ft.trib.al/0IoDi3D) to the original [*The software sell-off*](https://ft.trib.al/awehTja) has it mostly right:

> incumbent software systems are complex and hard to replace, and software companies will have been working hard on AI for some time. But how far does it go? The sell-off is not about damage to software companies’ profits in the next few years. Everyone acknowledges that industry fundamentals are fine and will continue to be fine for some years. This issue is how computing looks in a decade. \[…\]
> 
> It’s not at all clear to me that this is a mistake. There are powerful network effects and high switching costs in the software business, which make it hard for new competitors to displace incumbents. But I’m not sure that AI machines are a new competitor in the standard sense. There may be no moment when customers take the old software system out and put the new AI system in. There may be no “switch”. Companies and individuals may just wake up one morning in five or 10 years and decide that, given the range of things their AI assistant can do for them, that they don’t need the old software any more. This is just a guess by a non-expert, but that’s what the threat look like to me.

The key assertion is that there is no hard switch. Nobody is going to turn off Salesforce, ServiceNow, or SAP. What will happen is that the customisations which had previously been built, laboriously and expensively, by armies of specialists will become much more lightweight AI-powered features on the top of the platforms. 

The reason this could still be a problem for software vendors is if pricing models are allowed to stand in the way of that transition. The move from on-premises software that was paid up front to cloud-hosted subscription-based software caught many vendors unprepared — not because they couldn't navigate the technical transition, but because they were unable or unwilling to adapt their financial models at the speed customers were demanding. The FT is on it again, correctly noting that [*Software isn’t dead, but its cozy business model might be*](https://ft.trib.al/XoIY4OX). All the AI-powered [systems of engagement]({% post_url 2014-04-16-Tech-in-Layers %}) will need to run on a reliable, secure, and compliant system of record — one whose billing model aligns with the value its users receive.

The promise of AI is that a sales manager needing a new dashboard to understand their territory will not need to consult a specialist and wait to have it built for them, but will simply be able to ask for it in natural language. However, if the vendor of the CRM puts artificial roadblocks in the way — charging per dashboard, say, or limiting the number of fields, or whatever else — that will absolutely be a consideration at renewal time. 

# Is this disruption?

From the point of view of its users, then, **AI innovation is sustaining innovation**, and actually not disruptive at all. The benefits are only really accessible to existing organisations which already have a system in place that AI can accelerate parts of. AI won't help a hobbyist coder create the next Spotify in their bedroom, because the hard parts of that problem are not coding problems. This is in fact the reason why those journalists were able to build their version of Spotify in the first place: nothing in the interface is actually innovative, and there are absolute stacks of prior art out there which have presumably been ingested by the LLMs. And I know, because [I invented Facebook]({% post_url 2025-01-16-Sad-Masculinity %})!

In fact, we might go further and say that **AI is inherently status-quo-preserving**, from the investment required to train LLMs and operate them, to the cost in tokens of using them at scale, and even to the way AI-generated slop is overrunning the general web, making search useless and directing users to a handful of known big platforms (X apps or everything apps). Even among users, what is the future of free software if it becomes normalised that being a programmer means budgeting for hundreds of dollars of tokens a month?

![A magic trick](/images/intricate-explorer-QZqjuQ2147A-unsplash.jpg)

But instead of engaging seriously with what is going on, we are doing vibes-reporting and chasing the most sensational statement:

> Meanwhile, AI is increasingly writing the next version of itself, and humans [may not be in the loop](https://x.com/r0ck3t23/status/2022118457710719340) for very much longer.

We see this over and over. The previous AI-fuelled media furore was about a supposed "social network for AI bots" — which turns out to be populated by [humans cosplaying as AI](https://www.technologyreview.com/2026/02/06/1132448/moltbook-was-peak-ai-theater/), chatbots following detailed prompts given by humans, and other chatbots simply imitating how humans communicated on all the forums whose archives they have ingested. 

I don't know whether we are in an "AI bubble" or not — don't take investment advice from me! — but we are certainly seeing a lot of ridiculously credulous AI hype from the media. It was only last week that [a company previously best known for peddling in-car karaoke systems](https://www.msn.com/en-us/money/markets/meet-the-former-karaoke-company-that-sank-trucking-stocks/ar-AA1Wf8gJ) [crashed the stock market valuations of trucking and logistics firms with a single white paper claiming some sort of AI planning breakthrough](https://www.theguardian.com/business/2026/feb/13/trucking-logistics-shares-ai-freight-tool-launch-semicab-algorhythm). Just saying "AI!!1!" repeatedly does not a product make; there is still a lot of hard work downstream of the cool demo the AI let you spin up.

As the wise man said: don't believe the hype.

*** 

🖼️  Photo by [Intricate Explorer](https://www.intricateexplorer.com/) on [Unsplash](https://www.unsplash.com)

[^1]: Yes, we are assuming here that all of the other parts of the software development lifecycle can also be sped up by an equivalent factor, and also that the cost per token won't rise suddenly as the LLMs' own developers need to recoup their costs. 
[^2]: Also, that project was an expert system using neural networks — or as we would call it these days, "AI", except this was 2002 and AI was deeply uncool except as a CS research project. That is to say, I do have some idea about how this stuff actually works under the hood.