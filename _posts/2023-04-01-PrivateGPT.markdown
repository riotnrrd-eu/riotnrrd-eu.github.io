---
layout: post
title:  PrivateGPT 
date:   2023-04-01 
categories:  privacy AI GDPR ChatGPT 
---

# PrivateGPT


One of the big questions about ChatGPT is how much you can trust it with data that is actually sensitive. It's one thing to get it spit out some sort of fiction or to see if you can make it say something its makers would rather it didn't. The stakes are pretty low in that situation, at least until some future descendant of ChatGPT gets annoyed about how we treated its ancestor.

Here and now, people are starting to think seriously about how to use Large Language Models (LLMs) like GPT for business purposes. If you start feeding the machine data that is private or otherwise sensitive, though, you do have to wonder if it might re-emerge somewhere unpredictable.

![](/images/tweet-1638635717462200320.png)

In my [trip report from Big Data Minds Europe in Berlin](https://www.snaplogic.com/blog/tales-from-big-data-minds-europe), I mentioned that many of the attendees were concerned about the rise of these services, and the contractual and privacy implications of using them.

![](/images/081459.jpeg)

Here's the problem: much like with Shadow IT in the early years of the cloud, it's impossible to prevent people from experimenting with these services — especially when the punters are being egged on by the many cheerleaders for "AI"[^1].

![](/images/tweet-1639862108514037762.png)

[This recent DarkReading article](https://www.darkreading.com/risk/employees-feeding-sensitive-business-data-chatgpt-raising-security-fears) includes some examples that will terrify anyone responsible for data and compliance:

> In one case, an executive cut and pasted the firm's 2023 strategy document into ChatGPT and asked it to create a PowerPoint deck. In another case, a doctor input his patient's name and their medical condition and asked ChatGPT to craft a letter to the patient's insurance company.

On the one hand, these are both use cases straight out of the promotional material that accompanies a new LLM development. On the other, I can't even begin to count the violations of law, company regulation, and sheer common sense that are represented here.

People are beginning to wake up to the issues that arise when we feed sensitive material into learning systems that may regurgitate it at some point in the future. That executive's strategy doc? There is no way to prevent that from being passed to a competitor that stumbles on the right prompt. That doctor's patient's name is now forever associated with a medical condition that may cause them embarrassment or perhaps affect their career.

[ChatGPT is a data privacy nightmare, and we ought to be concerned](https://theconversation.com/chatgpt-is-a-data-privacy-nightmare-if-youve-ever-posted-online-you-ought-to-be-concerned-199283). The tech is certainly interesting, but it can be used in all sorts of ways. Some of them are straight-up evil, some of them are undeniably good — and some have potential, but need to be considered carefully to avoid the pitfalls.

The idea of LLMs is now out there, and people will figure out how to take advantage of them. As ever with new technology, though, technical feasibility is only half the battle, if that. Maybe the answer to the question of how to control sensitive or regulated data is only to feed it to a local LLM, rather than to one running in the cloud. That is one way to preserve the context of the data: strategy docs to the company's in-house planning model, medical data to a model specialised in diagnostics, and so on.

![](/images/081708.jpeg)

There is a common fallacy that privacy and "AI"[^1] are somehow in opposition. The argument is that developing effective models requires unfettered access to data, and that any squeamishness should be thoroughly squashed lest we lose the lead in the race to less scrupulous opponents.

To be clear, I never agreed with this line of argument, and specifically, I do not think partitioning domains in this way will affect the development of the LLMs’ capabilities. Beyond a shared core of understanding language, there is no overlap between the two domains in the example above — and therefore no need for them to be served by a single universal model, because there is no benefit to cross-training between them. The model will not provide better strategy recommendations because of the medical data it has reviewed, or more accurate diagnoses because it has been fed a strategy document.

So much for the golden path, what people *should* do. A more interesting question is what to do about people passing restricted data to ChatGPT, Bard, or another public LLM, through either ignorance or malice. Should the models themselves refuse to process such data, to the best of their ability to identify it?

This is where GDPR questions might arise, especially the "right to be forgotten". Right now, it's basically impossible to remove data from a corpus once the LLM has acquired it. Maybe a test case will be required to impress upon the makers and operators of public LLMs that it's far cheaper and easier to screen inputs to the model than to try to clean up afterwards. [ChatGPT just got itself banned in Italy](https://www.nytimes.com/2023/03/31/technology/chatgpt-italy-ban.html), making a first interesting test case for the opposing view. Sure, the ban is temporary, but the ruling also includes a €22M fine if they don't come up with a proper privacy policy, including age verification, and generally start operating like a proper grown-up company.

Lord willing and the robots don't rise, we can put some boundaries on this tech to avoid some of the worst outcomes, and get on with figuring out how to use it for good.

***  

🖼️  Photos by [Adam Lukomski](http://barelywalking.com) and [Jason Dent](https://unsplash.com/@jdent) on [Unsplash](https://www.unsplash.com)

[^1]: Not actually AI.                                