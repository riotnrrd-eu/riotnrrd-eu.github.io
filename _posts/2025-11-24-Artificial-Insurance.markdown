---
layout: post
title:
date: 2025-11-24
categories: AI
---

For all the talk of AI transforming our society and economy, hard data on real world adoption is still very hard to come by. Benedict Evans' latest update to his "[AI Eats the World](https://www.youtube.com/watch?v=niJpDnNtNp4)" presentation notes that in the context of the sort of total revolution in human affairs that GenAI is supposed to be, weekly active users are not remotely the right metric. How transformative is something that you use maybe once a week, really?

Meanwhile far too many of the people who *are* using ChatGPT and friends on a daily basis are using it to just raw-dog stuff they really really shouldn't, like [legal briefs](https://calmatters.org/economy/technology/2025/09/chatgpt-lawyer-fine-ai-regulation/). People will also believe what ChatGPT tells them, even when it [makes up features in a software package](https://www.404media.co/chatgpt-hallucinated-a-feature-forcing-human-developers-to-add-it/) — until the developers capitulated and added the made-up feature. Even leaving aside the weird stuff like the [spiral cults](https://www.rollingstone.com/culture/culture-features/spiralist-cult-ai-chatbot-1235463175/), it's clear that this tech can't be used unattended.

![A spiral staircase](/images/remy-penet-zaM9LhySx_0-unsplash.jpg)

I have been around AI since long before ChatGPT broke cover (unlike most of the AI bros of LinkedIn), and I have been giving the same advice since the beginning: Large Language Models are powerful, but they're not magic, and they need to be integrated with care into products and services. On the other hand, they are very attractive and even addictive to at least some users, enough that just saying "no" won't stop people from using them. Instead, they will go around the prohibition, and may get into even worse trouble that way.

# Deterministic auditability where it matters and probabilistic speed where it counts

Instead, the right approach is to integrate LLMs in ways that work to their strengths, and figure out ways to mitigate their weaknesses. One approach that I tend to assume is obvious, but apparently is not, is Retrieval-Augmented Generation, or RAG. This is a technique designed specifically to address the problem of hallucination or confabulation.

Simplifying enormously, LLMs will try to give a statistically probably response to a prompt. This is different from a search engine, as much as Google has been blurring that distinction. If I query Google for legal precedents, I will get back a list of real legal precedents that did actually occur. As long as I watch out for "helpful" interventions, like "did you mean FOO?" when I actually searched for BAR, I'm good to go. 

LLMs do not work like this. 

An LLM will return something that looks like a statistically probable response to prompts similar to what was entered. Sometimes that will be a real legal precedent or whatever, and sometimes it will be something that *looks* like a legal precedent, but has no basis in our actual consensus reality. The key point is that this is not some sort of error that can be corrected, or a bug that can be ironed out in future versions. This is how LLMs work; it's why they are so good at generating convincing text, but it's also why they cannot be used like search engines.

That is where RAG comes in: the LLM is used as a conversational interface to a database, but the hard data for the response comes from the database, not from the LLM.

I would say that at this point, three years and innumerable embarrassing news stories into the age of GenAI, not using RAG and similar best-practice techniques is tantamount to malpractice when deploying these tools in production, especially in customer-facing roles.

If further encouragement is needed, here is this article from the *Financial Times*: [Insurers retreat from AI cover as risk of multibillion-dollar claims mounts](https://www.ft.com/content/abfe9741-f438-4ed6-a673-075ec177dc62):
  
> AI hallucinations typically fall outside standard cyber cover, which is triggered by security or privacy breaches. So-called tech “errors and omissions” policies are more likely to cover AI mistakes, but new carve-outs could narrow the scope of the coverage offered.

![A quizzical teddy bear](/images/oxana-lyashenko-FtNM2H1RXZ8-unsplash.jpg)

Yes, if you roll out a chatbot to save yourself some call center costs, and it tells people there is a discount available or whatever, now you not only need to honour that discount, your insurer won't cover the losses if a million people use it. Or if the teddy bear toy to which you added an AI chatbot *for some insane reason* [starts giving kiddies BDSM advice](https://www.independent.co.uk/news/world/americas/us-politics/ai-teddy-bear-suspended-explicit-advice-b2868720.html), your insurer is going to leave you entirely on your own to deal with the mobs of enraged pitchfork-wielding parents. 

Maybe this will concentrate attention on the problem. And to be clear, this is not a problem of AI; the LLM is just doing what it's supposed to do. The problem is a question of service and product design. The fact that LLMs hallucinate is hardly news, but too many people were eager to rush something to market regardless, and if insurers refusing coverage is what it takes to get their attention, then so be it.

In the grand scheme of things this is a positive sign really. A new market may be a bit of a Wild West, but anything that is to get mainstream adoption gets regulated along the way. These are the growing pains of GenAI. 

And if you're at all sensible with how you add LLMs to your product or service, you will be absolutely fine.

*** 

🖼️  Photos by [Rémy Penet](https://remy-penet.fr/) and [Oxana Lyashenko](http://www.sanateddy.com/) on [Unsplash](https://www.unsplash.com)