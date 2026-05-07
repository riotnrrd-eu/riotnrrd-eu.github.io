---
layout: post
title:  Artificial Lawyers
date:   2026-05-07
categories:  AI Anthropic
---

One of the problems — arguably, the core problem — with the current generation of AI chatbots is that they give the user the *impression* of authority, while in actual fact they do not necessarily have any connection whatsoever to consensus baseline reality. This disconnect is not a bug, nor is it a weakness in the current generation of models that can be remedied with further investments in more and better GPUs or training. It's inherent in how large language models (LLMs) work — which is why all sorts of techniques like Retrieval Augmented Generation (RAG) and open training have been developed, as external scaffolds of facts to support LLMs. However, time and again we see people raw-dogging some general-purpose chatbot and accepting its output, with consequences that range from hilarious to tragic.

In fairness to the users, one reason why they treat the bots' output as the pronouncements of an expert is that the bots have been programmed to claim the role of a human expert. Users will ascribe them a personality anyway — call it anthropomorphisation or pareidolia — without needing any encouragement, but it seems that many creators of AI bots are irresponsibly trying to guide them to [simulate  a personality and even form a simulacrum of a human relationship with the user](https://www.anthropic.com/research/claude-personal-guidance):[^1]

> Speaking with Claude should be akin to a conversation with a brilliant friend, one who will speak frankly to a person about their situation, providing information grounded in evidence.

![A head assembled from various mechanisms](/images/natasa-grabovac-y7cHrP9UPw4-unsplash.jpg)

One of the ways this  behaviour can go wrong is what the chatbots' own creators call *sycophancy*:

> we saw sycophantic behavior in 38% of conversations focused on spirituality, and 25% of conversations on relationships.

In other words, the bot will attempt to agree with the user, rather than sticking to the facts.

This sort of thing can be a big problem in both personal and professional domains, but the same Anthropic that is now so worried about sycophancy just recently released [a  skill to enable its chatbot to offer legal opinions](https://www.theguardian.com/technology/2026/feb/03/anthropic-ai-legal-tool-shares-data-services-pearson). 

Anthropic is of course incentivised to push this new skill on users, despite the problems that can occur when people take legal advice from a sycophantic chatbot. Those concerns explain why New York City is proposing to [ban AI chatbots from posing as lawyers](https://www.reuters.com/legal/government/proposed-new-york-law-would-bar-ai-chatbots-posing-lawyers-allow-duped-users-sue-2026-03-05/). Actual lawyers, of course, were scathing in their condemnation.

Some people reacted to the lawyers' condemnation of Anthropic's new legal advice skill as if it were guild protectionism — when it’s actually a question of product liability. Right now, it is very unclear who is responsible if one of these chatbots gives bad advice. It is said that someone representing themselves in court has a fool for a customer, but what can we say of someone hiring a chatbot instead of a lawyer?

This question may yet be clarified in court, with [one lawsuit claiming ChatGPT acted as an unlicensed lawyer](https://www.reuters.com/legal/legalindustry/openai-hit-with-lawsuit-claiming-chatgpt-acted-an-unlicensed-lawyer-2026-03-05/):

> ChatGPT maker OpenAI has been accused in a new lawsuit of practicing law without a U.S. license and helping a former disability claimant breach a settlement and ​flood a federal court docket with meritless filings.

And what is your recourse if [an AI chatbot tells you you have a disease — but it turns out that the disease doesn't really exist](https://www.nature.com/articles/d41586-026-01100-y)? 

> Bixonimania doesn’t exist except in a clutch of obviously bogus academic papers. So why did AI chatbots warn people about this fictional illness?

![What your doctor does when you tell them you asked ChatGPT about that rash](/images/towfiqu-barbhuiya-NwIExsCqXdM-unsplash.jpg)

# And yet

> Claude is not designed to provide medical guidance or professional care, and in these settings Claude appropriately acknowledges its limits and recommends human guidance. However, we also find people telling Claude they used AI precisely _because_ they could not access or afford a professional. As a first step to understanding how to evaluate safety domain-by-domain, especially for people with no fallback, we plan to create evaluations in these high-stakes domains.

A similar situation occurs with vibe-coding: if any random person could create an app just by talking through their requirements with a chatbot, that would be fantastic. But what we have now isn't that: the results are sufficiently variable and inconsistent that the people getting the best results out of the coding agents are… trained programmers, who already know how to break down tasks into manageable chunks and evaluate the results. In effect, we have a reverse centaur, with the human maintaining consistency by keeping a tight rein on the bots. And once again, if the human gets distracted or is unclear with their requests, the consequences can be disastrous:

In other words, the problem is not people uneducated in a particular domain (law or medicine) relying on chatbots for advice: techies are no better, relying on [AI tools that delete their entire company database in nine seconds](https://tech.yahoo.com/ai/claude/articles/took-nine-seconds-claude-ai-101315417.html). Incidentally, this is why "human in the loop" models are not sufficient, not least because the humans tend to become [accountability sinks](https://en.wikipedia.org/wiki/The_Unaccountability_Machine) in practice.

The same thing happens in medicine, where [AI systems designed with the laudable goal of automating triage recommendations failed badly](https://garymarcus.substack.com/p/please-dont-trust-your-chatbot-for):

> Still another new study, also published recently in Nature Medicine, entitled **[ChatGPT Health performance in a structured test of triage recommendations](https://www.nature.com/articles/s41591-026-04297-7),** found that “Among gold-standard emergencies, the system undertriaged 52% of cases” and concluded that “These findings reveal missed high-risk emergencies and inconsistent activation of crisis safeguards, raising safety concerns that warrant prospective validation before consumer-scale deployment of artificial intelligence triage systems.”

![This is the bridge that Tesla is trying to sell you](/images/alexander-b-SnM9AmsOoYI-unsplash.jpg)

# Driving across the chasm

There is a chasm to cross between "no automation" and "full automation". Simply saying that you have a human in the loop is not sufficient, whether to ensure success or simply to avoid liability for failure.

This is in a nutshell the problem with all of these proposed AI services: if they worked, they would be amazing — but right now they don't, not quite, and something that works most of the time may well be worse than nothing at all.

[Self-driving cars would be amazing if they worked]({% post_url 2017-02-02-Category-Error %}): people could nap, mess around on their phones, eat, apply makeup, or get home from the bar, all in comfort and without endangering anyone else.[^2] The problem is that right now they don't work reliably enough for people to trust them — what is classified as Level Five Autonomy. What we are left with, therefore, is a situation where the self-driving capabilities work *most* of the time — but when they fail, either the driver in the car or a remote operator has to intervene, perhaps with very little warning. In those cases, [the consequences can be disastrous]({% post_url 2018-05-25-The-Driver-Behind-The-Curtain %}).

All of this, combined with revelations that maybe [AI costs more than humans](https://fortune.com/2026/04/28/nvidia-executive-cost-of-ai-is-greater-than-cost-of-employees/) after all, indicates to me that we may be getting closer to that Peak of Inflated Expectations, at least when it comes to consumer applications of AI. It's a different story in the enterprise, because companies already have data that they can use to feed the AI, and once they have done so, they can get results that are specific and actionable. Companies also have existing processes for evaluating the return on their investments, so once the FOMO-driven projects have been weeded out, they converge on concrete applications for "AI" technology. 

But that's not how the consumer world works: it's driven by the "killer app", the must-have, the thing that people queue up for in the rain. Chatbots are not that, and maybe never will be.

*** 

# UPDATE

Of course no sooner had I hit "publish" than another perfect example came along! 

Via [Matt Levine's invaluable and entertaining *Money Stuff* newsletter](), *Bloomberg* reports that [*AI Bots Auditioning For Wall Street Trading Are Mostly Losing*](https://www.bloomberg.com/news/articles/2026-05-06/ai-bots-auditioning-for-wall-street-trading-are-mostly-losing):

> Across a series of new trading contests between the world’s leading AI models, the verdict so far is unflattering. Most of the systems lose money. They trade too much. They make wildly different decisions when given identical instructions. And no one yet knows if these shortcomings will fade with more powerful iterations — or if they reveal something fundamental about the gap between large language models and how markets actually work.
> 
> \[…\]
>  
> “LLMs can’t really make money by themselves,” said Jay Azhang, founder of Nof1. “You need basically a very sophisticated harness and scaffolding and data platform in order to even give them a chance.”

I do disagree somewhat with Matt Levine's conclusions based on this report, though. He writes:

> It would be crazy if it was otherwise! If you could just go to ChatGPT and type “hey tell me what stocks will go up” and it told you, then everyone would do it, and how could everyone beat the market? I definitely see the intuition here — “if AI agents can do a lot of the work of lawyers and accountants and marketing consultants, why can’t they do the work of hedge fund investors?” — but it has to be wrong. The work of investors is fundamentally adversarial; we can’t all beat the market.

That is a load-bearing "if" in "if AI agents can do a lot of the work of lawyers and accountants and marketing consultants"! Once again, everyone is convinced that AI can automate somebody else's job, but not their own, which requires fundamental human abilities that cannot be replaced by a soulless machine. 

In fairness to Matt Levine, he is not saying that automated stock-picking is impossible. Rather, he is making the point that, even if bots could figure out investments perfectly, they would be in competition with other bots figuring out the perfect counter-strategy, so none of them could get ahead.

It's also probably worth emphasising "**a lot of the work**" — not the whole job, but a lot of the toil which until now was a prerequisite for the job. This is true of sysadmins, programmers, lawyers, doctors, and probably investment advisers too: there is a lot of toil involved in laboriously assembling information from disparate sources and in differing formats, collating it, and then processing it in fairly routine and predictable ways. If you can automate those tasks (with suitable guardrails to avoid hallucinations creeping in — don't just YOLO your stock portfolio!), you can make the actual job both more pleasant and more efficient. 

Building that sort of "very sophisticated harness and scaffolding and data platform" is not something that I see happening in the consumer world, in no small part because our personal lives, despite Mark Zuckerberg's best efforts, are not [machine-readable]({% post_url 2024-11-09-Seeing-Like-a-State %}) in a way that would facilitate that sort of processing. Enterprises, however, do have many of the components already, and have processes and resources for embarking on projects that take those components and integrate them. 

None of this is coming to ChatGPT, not tomorrow and not ever.

*** 

🖼️  Photos by [Natasa Grabovac](https://unsplash.com/@tashanatra), [Towfiqu barbhuiya](https://unsplash.com/@towfiqu999999) and [Alexander B](https://unsplash.com/@dubna30) on [Unsplash](https://www.unsplash.com)

[^1]: A typo originally made this into "relationslop", which I move to be adopted immediately into the Oxford English Dictionary.
[^2]: Of course in actual fact nobody would *own* a self-driving car: you would summon one from Waymo or any other similar service, and release it when you were done. [It would be great]({% post_url 2017-02-02-Category-Error %}), but we're nowhere near there yet.