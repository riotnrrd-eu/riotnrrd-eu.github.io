---
layout: post
title:  How Sovereign Is Your Intelligence?
date:   2026-03-25
categories:  AI
---

Today brings an interesting juxtaposition of news items, each helping to illuminate the other.

We learn that [*For all but two nations, the AI race is already over*](https://www.washingtonpost.com/opinions/2026/03/17/ai-canada-europe-strategy-competition/). Here I have to admit that I can’t get the full article, so I am relying on the [excerpt](https://theoverspill.wordpress.com/meta-job-cuts-forecast-start-up-2632#7a746f59038208d381373d0633284ea4) from Charles Arthur’s invaluable newsletter, [*The Overspill*]:

> The middle powers in the West — European countries and Canada — are increasingly hoping to chart a course through the artificial intelligence revolution independent of China and the United States.

The authors then set in to demolish those hopes for digital sovereignty:

> In other sectors, settling for developing homegrown second-best technology might be a viable strategy for preserving sovereignty. In AI, that’s a riskier bet. If the gap between cutting-edge and second-tier systems continues to widen, and especially if advanced AI accelerates scientific research and industrial innovation, access to the best systems could become decisive for economic growth.
> 
> …Today’s AI infrastructure projects determine tomorrow’s catch-up capacity, and middle powers lag far behind. The European Union’s up to five planned AI “gigafactories” are slated to come online between 2026 and 2027; in 2024, Elon Musk’s xAI built a cluster of comparable size in 122 days. Europe’s most ambitious AI infrastructure projects are two to three years behind the curve, an eternity in AI development. Canada has committed roughly $2bn to “sovereign AI compute” over five years; Microsoft will spend over $100bn, more than 50 times as much, on its biggest data center in Wisconsin.

Sovereignty is a complex topic, especially in the age of AI. Partly there is the question of what we actually *mean* by "sovereignty" in the context of AI. Most people first encountered this concept as one of the objections to the wholesale adoption of cloud computing. For the first time around 2010 people from other countries might find their data inadvertently subject to US legislation. Even then, countermeasures were not as easy as “just don’t store your data in the US”; having a US legal entity, or even a US-**controlled** one, in charge of your data might still leave it subject to US law, even if the servers were located in, say, Ireland.

![don't trust anyone](/images/benjamin-lehman-ZYnXZ4pk_Ns-unsplash.jpg)

# You're not paranoid if they're really out to get you

The reason people and companies cared about digital sovereignty in the first place was not just paranoia; after all, if your list of potential attackers includes *the US government*, you probably make specific arrangements for your hosting that do not include us-east-1. The more generally applicable problem was that, especially in the EU, privacy laws, notably the GDPR, were seen as broadly incompatible with American willingness to subpoena everything in sight.

I do not want to relitigate what was a tedious conversation at the time, and has only become more polarised since then. What I do want to say is that the original digital-sovereignty *does not apply to AI in that form*. Whatever else it may be up to, the NSA is almost certainly not issuing demands to OpenAI that it reveal its training data in the hopes of finding evidence of some sort of mischief. Therefore, AI sovereignty is not *specifically* about control of data — although this may well be a relevant concern if you are using an LLM to process data that is subject to those regulations. In that case, you probably want to host both data and LLM on compute resources that you control, located in a jurisdiction which also gives you robust (and auditable) controls.

Instead, AI sovereignty, much as with many other aspects of AI discourse, is concerned with far more theoretical concerns, primarily with control over the models themselves. The thinking here is that if developers of a model, or of its hosted interface, can inject low-level instructions into it in ways that users are not aware of, that may influence the model’s outputs when prompted about particular topics. This insertion does not have to moustache-twirlingly nefarious; it could be as simple as advertising. It's hard to trust a product recommendation that may have been bought and paid for.

# Sovereignty, then and now

One interesting aspect of this new version of the sovereignty question is how the sides are drawn. In the original digital-sovereignty argument, it was mostly the US that was seen as the privacy-invading antagonist of the rest of the world. Although many other countries had *ambitions* that were equally invasive, few of them had the opportunity which the US enjoyed to extend their nosiness to the data of other countries‘ citizens, willingly stored on their own soil and in their own legal jurisdiction.

When it comes to AI sovereignty, the US presents itself much more as a potential *victim* of a resurgent China. How can US consumers protect themselves from the intrusions of the Chinese Communist Party, as mediated by whichever frontier lab is in the news this week? 

![First time, huh?](/images/first-time.jpg)

While there is a temptation on the part of the rest of us to enjoy the Schadenfreude of seeing the tables turned in this way, the concern is not entirely invalid.

# The problem with AI sovereignty is how hard it is to achieve in practice

For a successful AI project, you famously need two things: an AI model, and data to feed it with. The data side is relatively easy to conceptualise and manage, since this is literally the previous digital-sovereignty problem. But how are you managing the AI-specific part?

The hard question is where you are getting the AI model. If you want sovereignty, hosted services from the likes of OpenAI, Anthropic, and Google are presumably non-starters. But even if you’re looking at self-hosting your AI model, most of the top-ranked models — DeepSeek, Qwen, and so on — are from labs in China. And here we come to the second news item: even [Meta had to bail out of the AI race due to the sheer expense](https://www.reuters.com/business/world-at-work/meta-planning-sweeping-layoffs-ai-costs-mount-2026-03-14/). That expense also means you are probably not going to start training your own model, even if you could get the loads of Nvidia GPUs that you’d need to do that.

This is why the AI sovereignty question tends to abandon personal or corporate responsibility as a lost cause, and focus on national-level actors, which is where we started from. Sometimes this is an irredeemably disingenuous conversation, trying to push whatever country to spend more money with the American vendors of AI models. It is not at all clear to me how British sovereignty, for example, is increased by giving money to OpenAI, a US corporation, let alone encouraging British businesses and educational institutions to do so under the guise of "AI literacy".

![Broken lock. Sadness.](/images/thomas-hunter-ii-K1sqEGiRJR8-unsplash.jpg)

But even when the conversation is a bit more serious, talking about creating actual national AI champions, it runs into the same two issues: the immense cost of training new AI models from scratch (and the question of whether the compute hardware to do so is even available), and the need for suitable data with which to do that training. With the heightened attention to IP issues, it can be assumed that the freewheeling days of downloading a bunch of data from BitTorrent and not asking too many questions are over, at least for projects that wish to be seen as above-board and legally unproblematic — surely requirements for such would be national AI champions.

# What is to be done?

And so we come full circle: it probably isn't possible to have sovereign AI in the sense of a fully-isolated trusted and certified stack, at least not unless you are operating with the resources of a nation state or a very large corporation — in which case, hi, let's talk.

This is not a counsel of despair, nor a Unabomber-style manifesto arguing that we should abandon AI and retreat to a cabin in the woods.

What *is* possible is to architect a system that uses AI in ways that are safe and sane. For instance, our current models are not deterministic, that is, they are not predictable, nor do they give the same results for the same inputs. Because of how they operate, that is not a bug that can be ironed out; it's just how they work. This does not mean that you accept non-deterministic results of a process that should be deterministic! Nor does it mean that you cannot use AI around that process. It just means that you have to architect your system with that factor in mind. Perhaps you use the AI model to implement a static (therefore deterministic) automation that will actually execute the process in question. Because this output automation is static, it can be analysed and reasoned about in a way that AI models cannot be, and its results are knowable and (importantly) auditable.

This generic pattern can be applied to many different domains. I am working right now with two separate bank that are using AI in loan approval and fraud detection. The important thing is that they are not using general-purpose LLMs for the actual decisions; those are specialised models created and trained for that one purpose, and compliant with all the many (many) applicable regulations. Then there are the sorts of LLMs that you might encounter most days that are used to produce the various documents and analyses that surround the core yes-no decision — preparing a loan prospectus, or handling communications with customers who have been victims of fraud.

That same model is what will give us AI sovereignty: a carefully-constructed architecture, separating data that is actually sensitive from what is not, defining access controls and granular authorizations, and no doubt including AI in many different places, but doing so in ways that are adapted to each of those domains, not just ceding all control to AI. 

Not paranoia, not rushing to throw money at any possible solution, but thoughtful design of an appropriate solution. Hey, a guy can dream…

***

🖼️  Photos by [benjamin lehman](https://benjaminlehman.com/) and [Thomas Hunter II](https://thomashunter.name/) on [Unsplash](https://www.unsplash.com)
