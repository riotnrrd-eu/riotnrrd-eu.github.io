---
layout: post
title: More Haste, Less Speed
date: 2025-04-29
categories: AI support
---

When I [discussed using AI as front-line customer support]({% post_url 2025-02-03-Get-The-Robot-Off-The-Phone %}), I tried to balance between some obvious failure modes of the technology, and the promise of what it could deliver if it did work as advertised.

> As with most proposed applications of AI, the question of whether the AI is worth its GPU runtime is one of trade-offs. IF the AI can reduce the rate of tickets closed without solving the customer’s problem below the 65% cited by the Intercom CEO, that is good. BUT, what is the rate of customers whose problem cannot be solved by the AI, and who are at best delayed along the way to getting a resolution? To know whether the deployment of the notional AI-staffed Tier Zero is a good idea, you have to quantify those two aspects, and then factor in the cost of deploying and operating the system.

![A robot telephone](/images/p-l-2_t8WTny6iw-unsplash.jpg)

Well, someone actually [went and did it](https://news.ycombinator.com/item?id=43683012) — and, spoiler alert, it did not go well, but for a different reason than I had thought of. 

Users of [Cursor](https://www.cursor.com), self-described as "the best way to code with AI", were suddenly being logged out if they had multiple active sessions:

> Like,you’d be working on your desktop, switch to your laptop, and all of a sudden you're forcibly logged out. No warning, no notification, just gone.
> 
> Naturally, people thought this was a new policy.
> 
> So they asked support.
> 
> And here’s where it gets batshit: Cursor has a support email, so users emailed them to find out. The support peson told everyone this was “expected behavior” under their new login policy.
> 
> One problem. There was no support team, it was an AI designed to 'mimic human responses'

Basically, the support AI [hallucinated/confabulated](https://pmc.ncbi.nlm.nih.gov/articles/PMC10619792/) a non-existent support policy that would justify the behaviour which users were reporting — but seemingly, without actual reference to the real support policy.

There is now some confusion about what actually happened, but [this *Ars Technica* post](https://arstechnica.com/ai/2025/04/cursor-ai-support-bot-invents-fake-policy-and-triggers-user-uproar/) has a good rundown. 

To be clear, there are ways of designing AI-enabled services to avoid this sort of problem. It's a fairly safe assumption that [Retrieval-augmented generation, or RAG](https://en.wikipedia.org/wiki/Retrieval-augmented_generation), was used by Cursor in designing their support bot, but RAG is specifically designed to avoid this sort of problem by providing a source of ground truth via a vector database. Something more complicated must have happened here, and I would be very curious to see a full post-mortem.

Regardless, I love to see my point proven by reality so quickly. If you wire up an LLM to your docs and FAQs and set it loose to answer customer queries, you had better make very very sure that it is **only** going to base its responses on those approved sources. I had in my naïveté assumed that this was in the ground rules, and I was already focused on the next level: how customers can get escalated if their Question is not one that is Frequently Asked enough to make it into the bot's knowledge.

Or maybe Cursor just vibe-coded its own AI support bot, and now gets to regret that choice at their leisure. Certainly the fact that their fix appears to be the following does not fill me with confidence:

> "Any AI responses used for email support are now clearly labeled as such," he added. "We use AI-assisted responses as the first filter for email support."

If that is the case, what is the value of the AI support agent in the first place? As a user, I cannot trust anything with this "AI-assisted" label, because it may be disowned at any point by the company. And of course the irony is thick enough to cut with a knife in the fact that it's an AI-assisted coding company that gets bitten by over-enthusiastically deployed AI — not least because this whole debacle is not exactly a ringing endorsement of Cursor's AI chops.

I think the Cursor customers who cancelled their subscriptions made the right move here.

***

🖼️  Photos by [P.L.](https://unsplash.com/@partrickl) on [Unsplash](https://www.unsplash.com)