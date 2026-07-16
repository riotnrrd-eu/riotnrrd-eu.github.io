---
layout: post
title:  Object Permanence for AI
date:   2026-07-16
categories:  AI OpenAI
---

"AI" chatbots backed by LLMs like ChatGPT are persuasive on first encounter, but rapidly fall off a cliff of reliability as confabulations ("hallucinations") and other errors become evident. However, because the chatbot's responses are presented in convincing language, and overshadowed by the aura of unquestionable correctness granted by the fact that they are provided by the latest in high technology, human users have a tendency to accept them without performing any fact-checking or due diligence.

This acceptance of inaccurate information can be a problem, of course, and while both aspects are worth investigating, the reliability of outputs seems at first glance to be the easiest to solve. This was the problem with Siri, Alexa, and the other pre-LLM assistants: saying "hey dingus, play smooth jazz" is amazing when it works, but the shine comes off quickly when you hav to explain to the dingus for the seventeenth time what your home address is, who your spouse is, or which calendar or to-do list should be the default.

Right now AI tools do not have object permanence, beyond the ability to feed previous interactions in a conversation back in to give context to subsequent steps. The expectation of a Jarvis-like personal assistant is that it will learn over time, and this is where all of the previous iterations have fallen down. 

One reason why [AI has taken off in the enterprise way faster than in consumer applications is the availability of information for it to work on]({% post_url 2026-07-07-Absent-Intelligence %}). To put it another way, a company's processes are far more legible to AI than a person's daily life. With techniques like [Retrieval-Augmented Generation, or RAG]({% post_url 2024-12-11-Object-Permanence-for-AI %}), LLMs can easily parse those processes and present their analysis back to users. And of course there is code generation, where there is no bottleneck of availability of information; if anything, the problem is the opposite!

# An LLM in every pot

But of course plenty of companies would still like to try to crack the consumer market, which leads us to this report from *Bloomberg* that [OpenAI’s First Device Will Be Home Speaker Built as AI Companion](https://www.bloomberg.com/news/articles/2026-07-14/openai-s-first-device-will-be-moveable-screenless-speaker-built-as-ai-companion). I am not quite clear on whether this is the long-rumoured device that Jony Ive has been working on, nor how it may relate to [Apple's lawsuit against OpenAI over hardware trade secrets specifically](https://9to5mac.com/2026/07/10/apple-sues-openai-trade-secret-theft/), but one thing that does seem clear is that this is OpenAI trying to learn its users' worlds. 

> OpenAI’s much-anticipated push into consumer devices is slated to begin with a mobile, screen-free smart speaker designed to be a new type of home computer for the AI era, according to people familiar with the matter.
> 
> The product — still under development — is meant to serve as a humanlike AI companion that lives in the home, said the people, who asked not to be identified because the project hasn’t been announced. It will help control smart-home appliances, play media, answer questions, respond to messages and tap into the range of capabilities offered by OpenAI’s ChatGPT, they said.
> 
> OpenAI believes the product’s defining feature will be its personality and ability to connect on a humanlike level with users. The speaker incorporates mechanical elements that can move on their own, creating a sense that it is alive and not just an object responding to commands. The machine also will draw on personal information such as emails to better understand its owner.

I am not sure that I find "a physical manifestation of OpenAI’s ChatGPT" a compelling proposition, especially if it is going to want access to my emails. 

> Another central difference is that the device includes a rechargeable battery, allowing it to be carried from room to room throughout the day. A user could bring it into the laundry room while doing chores, move it into the kitchen for cooking assistance, and later place it in a living room or bedroom to have it play music. It can also remain plugged into a single room if the customer chooses.

This is the "reverse centaur" pattern of AI: instead of a human empowered by AI, here the human is doing work for the AI by lugging this weighted companion cube around with them. There would need to be a pretty huge payoff to make this a proposition that could be sold to more people than bought [Humane's ill-fated AI Pin]({% post_url 2025-02-19-End-of-Product-Life %}).

# Won't somebody think of the models?

The other aspect of large language models that is interesting is users' tendency to treat them as people. This anthropomorphisation of computer programs capable of emitting fluent language has been known since Joseph P Weizenbaum's early experiments with [ELIZA](https://en.wikipedia.org/wiki/ELIZA) in the mid-60s. ELIZA had two levels, the generic language analyser and a script which enabled the program to take on different roles. The best-known script is called DOCTOR, and enabled ELIZA to act as a Rogerian psychotherapist — or, as Weizenbaum scrupulously notes, a parody of one — responding to user input with questions which reflect the user's statements back at them. 

Weizenbaum was sufficiently shocked by the public reaction to ELIZA, and especially to DOCTOR, to write up an extended response in "Computer Power and Human Reason", a book published in 1976 but most of which could be re-released unaltered tomorrow. He lists three specific "shocks" that prompted him to write the book:

> 1. A number of practicing psychiatrists seriously believed the DOCTOR computer program could grow into a nearly completely automatic form of psychotherapy. \[…\]
> 2. I was startled to see how quickly and how very deeply people conversing with DOCTOR became emotionally involved with the computer and how unequivocally they anthropomorphized it. Once my secretary, who had watched me work on the program for many months and therefore surely knew it to be merely a computer program, started conversing with it. After only a few interchanges with it, she asked me to leave the room. Another time, I suggested I might rig the system so that I could examine all conversations anyone had had with it, say, overnight. I was promptly bombarded with accusations that what I proposed amounted to spying on people's most intimate thoughts; clear evidence that people were conversing with the computer as if it were a person who could be appropriately and usefully addressed in intimate terms.
> 3. Another widespread, and to me surprising, reaction to the ELIZA program was the spread of a belief that it demonstrated a general solution to the problem of computer understanding of natural language.

This all sounds very familiar today, fifty years later:

1. Jobs will be automated! 
2. People treat their preferred chatbot as a person and share their most intimate secrets with it.
3. And of course, Artificial General Intelligence (AGI) is just around the corner.

I think it's clear that the first of these predictions is not happening. Geoff Hinton told the world in 2016 to stop hiring radiologists, because AI would be able to do their jobs. In fact, [the Mayo Clinic has increased the number of radiologists by 55% in the decade since that prediction](https://www.forbes.com/sites/jonmarkman/2026/01/26/the-radiologist-effect-why-ai-creates-more-jobs-not-fewer/). Meanwhile, predictions of the imminence of AGI at this point are unfalsifiable statements of religious belief in the Rapture of the Nerds, so there is not much point engaging with them.

But what about that second point?

With this new device, OpenAI is engaging in a "remaking of the world in the image of the computer", to cite Weizenbaum once again. We already [outsource huge parts of our lives to black-box algorithms]({% post_url 2017-09-20-Algorithmic-Reality %}), and this trend is only going to accelerate as the front-end for those algorithms becomes more persuasive.

![A shoggoth with a smiley-face mask](/images/shoggoth-with-smiley-face.png)

A personal assistant is undoubtedly something that people want. The idea of an unflappable [Jeeves](https://en.wikipedia.org/wiki/Jeeves) that will organise our lives for us sounds great — although in reality, I suspect that I at least would kick like Bertie Wooster, and choose to wear my favourite straw hat regardless of the pain it might cause. There are also some sociological questions about the fact that what people want is, effectively, a slave — but, much like with lab-grown meat, I come down on the position that if technology can enable us to satisfy our desires while removing the ethical downsides, I see little point in further interrogating the desires.

This is where OpenAI's putative device falls down, at least on the strength of this report. People by and large don't mind using chatbots as apps on their phones, because they already have plenty of reasons to carry those around. But getting them to carry a second device around is a tall order. The OpenAI companion cube would have to offer something distinct from what the ChatGPT app could do alone, and at least for now, it's not clear what that could be.

This is not a technical argument, mind: AI tech is still evolving very fast. But if both device and app rely on the same model hosted by OpenAI, that can't be a point of differentiation. The version embodied on the device could potentially have more sensors than a phone does, or ones that do not require the owner to wave it around, at least — but multi-modal use cases like that burn tokens *fast*, and token prices are rising fast and expected to continue to accelerate.

Would OpenAI offload some components to run locally on the device? Maybe, although they have been reluctant to do that — and the problem with this approach is that they would become victims of their own success. Because of the AI boom, prices for computer components are *stratospherically high* right now, while availability is very limited. A device powerful enough to have much onboard intelligence would necessarily have a price tag in the four figures, further reducing its appeal.

I stand ready to be proved wrong by Sam Altman and Jony Ive, but for now, I think I'm going to continue to focus on the enterprise side of things.