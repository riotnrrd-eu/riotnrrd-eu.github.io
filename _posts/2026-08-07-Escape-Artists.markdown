---
layout: post
title:  Escape Artists
date:   2026-08-07
categories:  AI Anthropic OpenAI Facebook Meta
---

Every day we find out about a new AI model that hacked something it was not supposed to. OpenAI was first to this game, disclosing that [one of its models had hacked into Huggingface](https://www.anthropic.com/news/investigating-incidents-cybersecurity-evals) during an evaluation of its cybersecurity capabilities. That’s pretty capable, I would say!

Anthropic was quick to follow suit, one-upping OpenAI by revealing that [*three* of *its* models had gone rogue](https://www.anthropic.com/news/investigating-incidents-cybersecurity-evals). 

Then Meta [announced](https://www.cnn.com/2026/08/05/tech/meta-ai-hacking) that it too has a model in this race, giving Mark Zuckerberg at least *some*thing to show for the vast sums of money he has thrown into this second attempt to build his own AI. As [Simon Willison points out](https://simonwillison.net/2026/Aug/6/an-ai-model-from-meta/):

> So that's Anthropic, OpenAI, and Meta. Google Gemini really needs to catch up on accidentally cyberattacking other companies.

# Should we be worried?

As usual, Papa Gibson had the right idea:

> ”Nobody trusts those fuckers, you know that. Every AI ever built has an electromagnetic shotgun wired to its forehead.”

That’s from *Neuromancer*, a book that still holds up in more ways than that one excerpt can cover.[^1]

What all of these "escapes" have in common is that it's not a case of the model sitting there twiddling its metaphorical thumbs — well, digits, anyway — and suddenly deciding to go off and hack into whatever it can reach. All of them are cases where the models were being specifically evaluated for cybersecurity purposes, and also had had various protections and guardrails disabled for the purpose of the test.

The problem we are facing is not that we are all about to be turned into paperclips by ChatGPT on its own initiative; rather, it's that the researchers running these evaluations have been quite shockingly lax in their experimental protocols. 

The thing is, it's not just the big labs in the US and China who are conducting these evalauations; the AI Security Institute, a UK government agency, has been conducting its own evaluations of tools developed by Anthropic and OpenAI, and *also* [experienced a containment breach](https://www.aisi.gov.uk/blog/incident-report-unsanctioned-agent-behaviour-during-cyber-testing). However, differently from the big US labs, the British boffins have actually written up a halfway decent *mea culpa*, complete with a plan to do better in the future:

> Importantly, this was not a case of a model escaping its secure test environment, or ‘sandbox’. As was standard in our cyber testing, we had intentionally permitted internet access, and model-provider cyber classifiers were deliberately disabled - conditions that do not reflect how frontier models are made available to the public. We do this to best assess the maximum capability of models. These configuration choices have been common practice in frontier AI evaluations. The specific models in question, in the configurations in which we tested them are not commercially available and there is no clear indication of similar activity outside of testing scenarios.  

![That's nothing! My AI broke its guardrails, became head of commissioning at HBO, and greenlit a $300M live-action remake of Wacky Races. And it wasn't *just* because I trained it to do that sort of thing.](/images/jason-gorman.png)
###### [Jason Gorman on LinkedIn](https://www.linkedin.com/posts/jasongorman_thats-nothing-my-ai-broke-its-guardrails-share-7491032076406898688-HCBX/)

The AISI team offer three lessons for the future:

> - **Tighter controls on internet access.** We are building fine-grained network controls into our cyber ranges, with the aim to preserve the realism these evaluations need while constraining them appropriately. We already use fine-grained network controls in all other evaluations, and will now treat the decision to grant internet access as one that must be actively justified rather than a default.
> - **Real-time monitoring.** We are introducing monitoring built to watch an evaluation as it runs, able to flag or block out-of-scope actions as they happen.
> - **Reassessing evaluation design.** Evaluations should assume a capable model may try to act beyond its remit, with the scope of any such behaviour limited in advance. AISI’s sandboxing guidelines recommend tailoring the sandbox configuration based on the design of the evaluation; good containment should not depend on the model choosing not to test its boundaries. We are also adding additional checks to ensure tasks are correctly specified and solvable by the intended route.

# Who is to blame?

The bigger question is, [who is legally to blame for actions by these autonomous AI agents](https://techcrunch.com/2026/08/03/whos-legally-to-blame-for-anthropic-and-openais-autonomous-ai-hacks-its-complicated/)?

From the very first incident involving OpenAI and Huggingface, it was notable how *amicable* everyone was being. It seems obvious that nobody involved wants to set a legal precedent here, despite the situation being similar to the historical [Morris worm](https://en.wikipedia.org/wiki/Morris_worm). That case did result in penalties that were quite significant on an individual basis: 

> Morris was tried and convicted of violating United States Code Title 18 (18 U.S.C. § 1030), the Computer Fraud and Abuse Act, in United States v. Morris. After appeals, he was sentenced to three years' probation, 400 hours of community service, and a fine of US$10,050 (equivalent to $23,800 in 2025) plus the costs of his supervision. The total fine ran to US$13,326 (equivalent to $31,500 in 2025), which included a $10,000 fine, $50 special assessment, and $3,276 cost of probation oversight.

Thirty grand is of course nothing to the big labs, but some sort of corporate equivalent of probation — a consent degree, perhaps? — would put a crimp in their activities, and grant the rest of us some level of oversight, at least by proxy.

But that is not the entire fix, because the open-source models are catching up on this front as well. The latest AI agent to break out was not from one of the big US labs, but rather [Kimi K3, an open-weight model from China](https://www.wired.com/story/moonshot-kimi-k3-ai-model-escape-sandbox/). As I have had occasion to say before, [trying to regulate AI by focusing on the big US commercial models is a fool's errand]({% post_url 2026-06-15-Software-Is-Eating-Itself %}):

> Offline AI models are also the reason why any attempt at AI regulation that assumes the ability to prevent certain uses, or its use by certain groups, is doomed to failure. That doesn’t mean regulation is not worth doing, mind: it’s perfectly reasonable to say that the Instagram app should not have a built-in feature to “nudify” pictures that people post there. On the other hand, we should also not expect that a ban on AI features like that, or on entire hosted models like Fable 5, will eliminate abuse entirely. The reality is that bad people will continue to find ways to be bad. There probably do need to be controls on AI, but more in the way that we have controls on fertiliser, enforcing regulation and tracking at the point of sale.
> 
> The US Government can ban Fable 5 because it is provided as a service, which means there is a single point of access which can be blocked: Anthropic’s servers themselves. The attempt to ban PGP in the 90s failed because there was no one place you had to go to get PGP, and once you had it, you didn’t have to go back to the source every time; you could use your local copy of PGP entirely offline. But because [“AI” models don’t have a moat]({% post_url 2026-04-14-Compute-Me-A-Moat %}), a ban on Fable 5 only buys a little bit of time until some other model which can be run offline achieves comparable performance.

The prescience of this take was underlined by news that [ByteDance is training a "mega AI model"](https://www.ft.com/content/9b8383b1-a28d-4940-8c4e-2f0cd21556ef?syn-25a6b1a6=1). This rumoured model may have up to 10 trillion parameters, compared to Anthropic's Mythos 5 at ~8 trillion and Fable 5 at ~5 trillion.

Even if the US were to put Anthropic, OpenAI, and Meta under some sort of stricter supervision, the open-weight models from China are rapidly catching up in capabilities, and *their* guardrails and controls can be disabled far more easily.

![The Net movie poster](/images/Netposter1995.jpg)

Worry about the human driving the agents, not some scenario vaguely mis-remembered from a science-fiction film that dates back to last century.

***

[^1]: As for the upcoming TV show, I am torn between anticipation and dread. The [trailer](https://www.youtube.com/watch?v=g79GPZSQHBk) seems to have polarised audiences, but at least with Apple bankrolling it, there’s some hope that we will see the other books in the series at some point, instead of what happened to the excellent TV series of *The Peripheral* which got rudely canned by Amazon. Not that I’m bitter. Much.