---
layout: post
title: Mismatched Intelligence
date: 2025-01-30
categories: AI DeepSeek LLM
---

The initial wave of noise about DeepSeek has started to fade and be replaced with coherent analysis. I have been doing my own research to figure out what is actually going on, and it ended up turning into a blog post. I hope this is useful to somebody.

On the 26th of January, I started picking up lots of posts on social media about this new LLM out of China called DeepSeek, which was giving similar performance to the latest Western models but at a fraction of the price and training cost. The 26th was a Sunday, and by the time the markets opened on Monday, there were [all sorts of shenanigans](https://www.reuters.com/technology/chinas-deepseek-sets-off-ai-market-rout-2025-01-27/). The worst hit was Nvidia, which lost 17% of its market cap, or nearly $600 billion. This reaction makes sense, since its sky-high valuation (up 171% in 2024 alone) is largely based on the forecasts of continuing growth in the GPU market, driven by the need to train and run ever-larger AI models. 

![Stock market turmoil](/images/nicholas-cappello-Wb63zqJ5gnE-unsplash.jpg)

# So what's new?

The first thing that is weird about the sudden panic is that *none of it was news*. Ben Thompson devoted his [*Stratechery* update](https://stratechery.com/2025/stratechery-updates-deepseek-r1-deepseek-implications/)(paywall) on the 21st of January to DeepSeek. Ben links to a *Bloomberg* piece from the 9th of January titled "[China’s DeepSeek Shows Why Trump’s Trade War Will Be Hard to Win](https://www.bloomberg.com/opinion/articles/2025-01-09/chinese-ai-deepseek-shows-why-trump-s-trade-war-will-be-hard-to-win)".

Further back, Simon Willison mentioned DeepSeek no fewer than 11 times in his round-up of [Things we learned about LLMs in 2024](https://simonwillison.net/2024/Dec/31/llms-in-2024/). The first mention was not even because DeepSeek was newsworthy in itself; instead, DeepSeek was included as just one example of the use of synthetic data created by one model for training new models:

> DeepSeek v3 used “reasoning” data created by DeepSeek-R1. 

Simon also linked to the announcement of the availability of DeepSeek R1 to the public, back in November:

> DeepSeek made their [DeepSeek-R1-Lite-Preview](https://api-docs.deepseek.com/news/news1120) model available to try out through their chat interface [on November 20th](https://x.com/deepseek_ai/status/1859200141355536422).

Finally, Simon also offers some pretty decent analysis of the significance of DeepSeek, especially bearing in mind that this post was published nearly a month before the current panic, on the 31st of December 2024:

> #### Was the best currently available LLM trained in China for less than $6m? [#](https://simonwillison.net/2024/Dec/31/llms-in-2024/#was-the-best-currently-available-llm-trained-in-china-for-less-than-6m-)
> 
> Not quite, but almost! It does make for a great attention-grabbing headline.
> 
> The big news to end the year was the release [of DeepSeek v3](https://simonwillison.net/2024/Dec/25/deepseek-v3/)—dropped on Hugging Face on Christmas Day without so much as a README file, then followed by documentation and a paper [the day after that](https://simonwillison.net/2024/Dec/26/deepseek-v3/).
> 
> DeepSeek v3 is a huge 685B parameter model—one of the largest openly licensed models currently available, significantly bigger than the largest of Meta’s Llama series, Llama 3.1 405B.
> 
> Benchmarks put it up there with Claude 3.5 Sonnet. Vibe benchmarks (aka the [Chatbot Arena](https://lmarena.ai/?leaderboard)) currently rank it 7th, just behind the Gemini 2.0 and OpenAI 4o/o1 models. This is by far the highest ranking openly licensed model.
> 
> The really impressive thing about DeepSeek v3 is the training cost. The model was trained on 2,788,000 H800 GPU hours at an estimated cost of $5,576,000. Llama 3.1 405B trained 30,840,000 GPU hours—11x that used by DeepSeek v3, for a model that benchmarks slightly worse.
> 
> Those [US export regulations](https://www.cnbc.com/2023/10/17/us-bans-export-of-more-ai-chips-including-nvidia-h800-to-china.html) on GPUs to China seem to have inspired some _very_ effective training optimizations!


![Piles of cash](/images/alexander-grey-8lnbXtxFGZw-unsplash.jpg)

# It Cost How Much?
There is some weirdness about those costs, since I have been unable to trace them back conclusively to an authoritative source. The sub-$6M training cost for DeepSeek-V3 is an estimate, and a very rough one at that. The only actual hard number is the number of GPU hours of training, which DeepSeek discloses in their [report](https://arxiv.org/html/2412.19437v1) as "2.788M H800 GPU hours". The Nvidia H800 is a restricted NVIDIA GPU sold only into the Chinese market[^1], where they [reportedly](https://www.tomshardware.com/news/price-of-nvidia-compute-gpu-can-hit-70000-in-china) cost up to $70k. Even if we assume that is not the price DeepSeek payed, because they either stockpiled GPUs before the export controls went into full effect in 2023, or obtained them in bulk at lower prices, that still indicates to me that the actual financial cost may have been higher.

The whole [model configuration](https://thezvi.substack.com/i/153830656/run-model-run) is also hyper-optimized for that particular setup, which may make it hard to replicate this result. Hugging Face is reportedly working to replicate DeepSeek’s work, so this conclusion is tentative.

# License To Seek
Part of the hype around DeepSeek is that it is supposedly an open-source model embarrassing the closed models from "Open"AI. However, it is worth noting that, while DeepSeek does indeed use the open MIT license, the actual model is encumbered with some significant [restrictions](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL), which make it *ipso facto* not "open source", as I have [discussed]({% post_url 2024-10-18-That-old-open-source-business %}) [before]({% post_url 2024-04-04-Defensive-Moves %}).

This is a minor point, but worth mentioning.

# Express Train
The reason DeepSeek caught people's notice, even with some delay, is how much more efficiently it was able to train its model — 90%+ more efficiently than Western equivalents, albeit with [some caveats](https://www.linkedin.com/posts/azamat-omuraliev-b6241351_deepseek-model-is-incredible-but-the-6m-activity-7289691614036307970-KuC8/). Despite what some of the early reactions indicated, though, this efficiency does not negate the climate impacts of AI, because that increased efficiency may well just be folded back into the current approaches to training, enabling even larger models to be trained and for AI features to become even more ubiquitous.

This is a well-known mechanism, called Jevon's Paradox[^2], and was first [invoked by Satya Nadella](https://www.geekwire.com/2025/microsoft-ceo-says-ai-use-will-skyrocket-with-more-efficiency-amid-craze-over-deepseek/) as the likely outcome here. More efficient training does not necessarily mean *less training*, let alone *less usage* of the resulting models. Efficiency applies equally to large models as to small ones, enabling new capabilities to be developed and deployed.

It is also worth noting that one of the big advances here is DeepSeek's Mixture of Experts design, meaning that only a small number of the "experts" (sub-models) activate for any task, which is where the efficiency comes from. However for queries that actually benefit from the full model's power, that advantage goes away.

Also DeepSeek doesn't support tools, meaning that DeepSeek R1 can’t call external functions, APIs, or perform external tasks (the "agentic" model). It can only generate text based on its internal knowledge, which is limited to what it was trained on. Tools are the things that make it possible for LLMs to interact with the world outside chat.

Finally, reinforcement learning without human feedback is innovative, but unproven. The concerns that the use of synthetic data and the removal of human oversight might lead to involution of the resulting model and a decrease in quality have not been disproven.

![People are confused](/images/tim-gouw-1K9T5YiZ2WU-unsplash.jpg)

# What Does It All Mean?
‪Shout out to [Chris Jones‬](‪@chrisjones1.bsky.social) for [this banger](https://bsky.app/profile/chrisjones1.bsky.social/post/3lgqmskoy7c2z):‬

> > I think the excitement is that that is absolutely nothing specifically Chinese about this - it's all known components, nearly all invented in the USA, put together in standard ways. if they can do it we can; no reason why France couldn't have ChercheProfond in a few months
> 
> User: "ChercheProfond, what do you make of this 400-page pdf?"
> 
> ChercheProfond: "\<shrugs\> bof"

The biggest loser from DeepSeek is Nvidia, not so much because of lower GPU sales (see point about training above) but because of the loss of its competitive moat from the CUDA toolchain. Until now, Nvidia benefited from a one-two lock on the market: it made the fastest GPUs, and CUDA was required to unlock their full capabilities. Even if another chip vendor managed to close the performance gap, developers would expect it to support CUDA. DeepSeek not using CUDA is a shot across Nvidia's bows that is far more serious than the fact that they used fewer GPUs.

The runner-up is OpenAI, because their messaging focused on maintaining their lead through brute-force application of massive compute. If technological capabilities can be achieved (much) more economically, the case for that enormous investment becomes even weaker. OpenAI also managed to shoot themselves in the foot while trying to return fire, with some truly terrible comms given their public perception as IP thieves, resulting in a widely-shared *404 Media* piece entitled *[OpenAI Furious DeepSeek Might Have Stolen All the Data OpenAI Stole From Us](https://www.404media.co/email/855bf870-82ce-4544-8776-2225627fa39d/)*. If the general public perception of you is that you're a thief, your calls of "stop thief!" may well fall upon deaf ears — that, or people just laugh at you.

The biggest winners: basically, everyone using LLMs, so Meta and Apple — and also [Amazon](https://www.linkedin.com/feed/update/urn:li:activity:7290322104825139200/). 

In the wider market, I expect that the much-derided "thin wrapper apps" will actually be among the ones that benefit most from this change. I have long said that AI itself is a feature, with no long-term defensible competitive moat. Nvidia was positioning itself as selling shovels into a gold rush, but the real winners in a gold rush are *the people buying gold*. If you are adding (useful!) AI features to your app or service, and the cost of providing those just crashed, you can either provide the same level of service for a lower investment, or a much higher level of service for a similar investment. I mean, these days you can [run DeepSeek on a Raspberry Pi](https://www.youtube.com/watch?v=o1sN1lB76EA). If you're selling LLMs or GPUs, that's a scary proposition. If you're using them to do something else, that is a pretty good position to be in!

# Longer Term
A big part of this story has been the mismatch between public consumer conception of AI (chatbots that make tasks more cumbersome, search features that are unreliable, models that steal data and IP to train on) and actually valuable use cases — coding assistants, research assistants, and all sorts of automated processing of large volumes of data. This mismatch is what drove the *Schadenfreude* around Nvidia and OpenAI's troubles, although the claims that the AI bubble was going to burst all of a sudden last Monday morning appear to have been premature. The long-term prospects look to me to be fundamentally unchanged, although some short-term market turmoil probably inevitable.


***

🖼️  Photos by [Nicholas Cappello](https://nicholas-cappello.com/), [Alexander Grey](http://www.pexels.com/@mccutcheon) and [Tim Gouw](https://unsplash.com/@punttim) on [Unsplash](https://www.unsplash.com)

[^1]: Although it too was later hit by [export restrictions](https://www.tomshardware.com/news/us-prohibits-exports-of-nvidias-a800-and-h800-to-china-blacklists-chinese-gpu-developers).
[^2]: I was a little surprised to find that I had not mentioned this concept on the blog before, since it's a classic of cloud computing that I must have been using in presentations for at least fifteen years at this point, but apparently not.