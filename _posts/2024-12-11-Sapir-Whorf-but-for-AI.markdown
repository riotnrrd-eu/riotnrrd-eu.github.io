---
layout: post
title: Sapir-Whorf but for AI
date: 2024-12-11
categories: AI language
---

The Sapir-Whorf hypothesis has fascinated me since I first heard of it. The idea that human cognition could be not only expressed through language, but fundamentally *shaped* by language at the very lowest levels, is the sort of idea that you need to sit down and ponder for a moment, while the fireworks go off behind your eyes.

While the strong Sapir-Whorf hypothesis has fallen out of favour (*pace* the excellent and utterly heart-rending film *Arrival*), I continue to believe in a weaker form of it — linguistic relativity, rather than full-on linguistic determinism. For example, in English there is only one word for the colour blue, while in many Latin languages there are two distinct words. In Italian they are “blu” and “azzurro”, respectively dark and light blue. It is important to point out that these are terms in the most common use, not at all like more *récherché* English words such as “azure” or “cerulean”, and they most definitely are distinct colours to speakers of Italian. If you point at a thing that is light blue and call it “blu”, you will be met with incomprehension or perhaps a enquiry as to whether you meant the thing that is obviously “azzurro”, much as if you had called a thing “red” that is very clearly brown.

A fascinating experiment tells us that this difference is so foundational that it affects the reaction times of colour identification by speakers of those languages. An English speaker can distinguish blue from green in an amount of time that is appropriate for distinctions between primary colours — but a speaker of Italian can distinguish between dark and light blue in that same amount of time, where the English speaker takes much longer, having had to switch into a different mode, suitable for identifying subtle shades of a colour. 

To me, this finding appears to be analogous to the one that showed that people are more utilitarian in their moral choices when [the question is posed in a language other than their mother tongue]({% post_url 2014-12-09-Debug-mode-for-humans %}). 
The extra time to reflect means that the answer is no longer purely instinctive, since the language gap means there is room for calculation.

![](/images/lukas-hND1OG3q67k-unsplash.jpg)

All of this lengthy preamble leads us to a fascinating question. Large language models run on, well, language. The training data is enormous reams of text, and the output is based on predictable patterns in human language.

The Sapir-Whorf hypothesis appears not to be true of humans — but might it be true of LLMs? And what might that mean for how we interact with them?

I remain sceptical of the possibility that LLMs (“spicy autocomplete”) can ever become conscious and achieve AGI. But that does not mean that they cannot be *useful* in their current and probable future state.

One of the big problems we have with LLMs today is still their propensity to hallucinate or confabulate: to provide output that is correctly formatted, but factually incorrect. Useful applications of LLMs these days tend to use a variety of strategies to protect against this happening and to mitigate the consequences if it does.

These techniques could be as simple as doing prompt engineering to prevent the confabulation, as we saw in the [leaked prompts for Apple Intelligence]({% post_url 2024-09-10-Too-much-AI %}).

A more complex technique is Retrieval-Augmented Generation, or RAG to its friends. In this case, instead of an LLM responding to user input based purely on its internal training data, a particular data set is first prepared and divided up into digestible “chunks” that are stored in a specialised data store, a vector data base. This encodes the chunks of informations into numerical representations whose proximity indicates their relationship.

The next level up is to use several different models in concert, acting as agents that have the ability to call on each other and evaluate each others’ responses, operating in concert to deliver some wider result. One benefit of this agentic, tool-calling architecture is the ability to include *guardrails*, with the goal of preventing incorrect output from one model that is part of this setup from impacting the final result.

![](/images/maximalfocus-naSAHDWRNbQ-unsplash.jpg)

It’s interesting to explore these techniques in terms of the Sapir-Whorf analogy. The behaviour of an LLM alone is determined purely by the language in the training data set. If that training data contains biases, whoever or whatever is consuming the model’s responses will encounter those, and will either have to deal with them, or learn how to minimise them by phrasing requests very carefully — what we call prompt engineering.

With RAG, we overlay an additional layer on top of that base model, forcing a considered response based on information in the vector store, instead of the instinctive response based on linguistic representation. That more considered response is more strictly rational, being based on the chunk of information that is presented to the model, but there is some delay and a little more effort involved. What? If you don’t think that effort is required to speak for a long period of time in a language other than your primary, even one that you speak well, let me assure you: it is [*exhausting*]({% post_url 2014-12-09-Debug-mode-for-humans %}).

And with agents calling and evaluating each other as part of a wider process, the analogy steps up one more level, to being conscious of biases in others — much as my wife has come to tolerate the fact that occasionally, I will emerge with something in “azzurro” when I had clearly been told to get the thing that is “blu”. She knows that when it comes to matters of colour, I am prone to confabulating, and my responses need to be checked against ground truth. She is my guardrail in this analogy, preventing my occasional hallucinations from causing problems further down the road — such as dressing the children incorrectly.

I don’t want to anthropomorphise LLMs too much here, though; I very much doubt they will ever develop into anything that we will need to develop a true theory of mind about. But humans are known for *pareidolia*, identifying patterns and even person-like traits where no such pattern exists. This is, after all, how LLM-powered chatbots work on us in the first place: we are primed to find signs and portents everywhere. Is it any surprise that we take a thing claiming to be a person at its word?

And while that tendency can be dangerous, given that it can’t be eradicated, we might as well try to make use of it. We humans reason well by analogy, and the Sapir-Whorf theory of GenAI seems like it has the potential to be a useful analogy in our semantic toolbox.

*** 

🖼️  Photos by [Lukas](https://unsplash.com/@hauntedeyes) and [Maximalfocus](https://www.maximalfocus.com) on [Unsplash](https://www.unsplash.com)