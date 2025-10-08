---
layout: post
title:  Oh Brave New World, That Has Such UX In It
date:   2025-10-08
categories: AI LLM UX
---

I spend probably more time than is healthy on LinkedIn and in adjacent circles, and I keep reading statements like this one[^1]:

> In the future, many UIs will be a combination of two things: 1) agentic ChatGPT-like user experiences powered by agents, many of which will be built by iPaaS agent builders that will have evolved into adaptive process orchestration and 2) custom-built code from application generation (AppGen) platforms.

I disagree quite fundamentally with both halves of that statement. 

Fundamentally, I think the assumption that the user interface to everything must be chat is misguided. This default is the product of a very specific historical coincidence, that the first app of this wave of AI to hit big with the general public happened to be a chatbot. This fact conditioned everybody's assumptions. There is always a certain amount of bandwagon-jumping in these moments, with companies wanting to be "the ChatGPT of X", in the same way that they would have claimed to be "Uber for X" a few years ago. But even apart from that, the success of ChatGPT created an unexamined assumption that **AI = chat**.

The thing is, many AI applications are not suited to chat — nor are all chat applications "AI" in any meaningful sense.

![A cyclist at high speed](/images/jahanzeb-ahsan-ZbFoi92fyzY-unsplash.jpg)

# The Need For Speed

The chat paradigm is fundamentally interactive, which also means there is an assumption of a maximum acceptable response time that is fairly short. Users will wait around only for so long while an idle animation spins ("thinking…") before they get bored and wander off. 

Note that this is not a problem that can be solved by throwing more compute power at the LLM that is backing the chatbot! If the bot is to do anything actually useful, it will need to interact with outside systems — and then it is at the mercy of the response time of those systems. Many of the crucial systems that run the world these days respond at a pace that is positively glacial when the query is in any way unusual or unexpected — which is most of them, if you give users the sort of open-ended freedom to ask questions and request action that the more excitable demos of "Agentic AI" always include.

The key point is that this is how the system works, by design. The data that underpins our modern world is held in systems that work in one of two ways. One group is designed to support *transactions*: this is the back-end to the websites and mobile apps that we use every day. These systems give lightning-fast responses at massive scale — but they do so by only accepting certain very specific types and patterns of requests. These patterns can be determined ahead of time by the developers of the apps and websites, and so the backend system can be optimised to answer queries that are known ahead of time.

The other type of system is the systems that are designed to support *analysis*. These systems are accessed by vastly fewer users, typically analysts that work for the company offering the service powered by the website or app described in the previous paragraph. These analysts are asking novel and unprecedented questions — and they are fine with waiting some time for the results to be computed. They value the completeness of the result, not how quickly it can be produced (within certain limits, of course). Analysis questions which are routine — end-of-month reports, for instance — can be encoded in reports and dashboards to be generated or refreshed on a schedule, so that they do not need to be computed every time they are needed. But if the analysts are doing their job right, they will be continuously coming up with new ways to interrogate the data in search of ways to improve or optimise the performance of the business.

Neither use case really benefits from a chat interface. Analysts have very specific questions, and a prompt that is sufficiently precise for their purposes becomes so formal that you might as well just write the SQL query and be done. And as for transactional use cases, entering into an interactive conversation that starts with "Book me a flight to London next Monday" and goes on from there is almost certainly going to be slower than just pulling up the airline's app and doing it myself. 

More on that in a bit — but first, let's look at the code generation part of the statement above.

![A mug on a table with a bottle](/images/nick-rickert-bwq_f_JGKvg-unsplash.jpg)

# Drunk Coding

The other part of that LinkedIn quote, about "application generation platforms", might *sound* like a better fit for AI, but it's actually no closer once you examine it in a bit more detail. 

The first problem is that generation of code is actually a relatively small part of the job of a developer. I touched upon this point in [my latest Coffee Talk video](https://www.youtube.com/watch?v=5XgllDpWaGg), referring to Bain's recent [*Technology Report 2025*](https://www.bain.com/insights/topics/technology-report/). The estimate there is that between 10% and 40% of programmers' time is spent actually bashing code out on a keyboard, so even assuming that the code output from the AppGen tool is *perfect*, there is still a lot of work left over.

Of course the argument for these vibe-coding tools is that they enable *everyone* to generate applications, not just programmers. A lot of programmers' non-coding time is spent on requirements gathering: understanding just what it is that the code should do. Most programming these days is in the pursuit of automation of processes, and so either the programmers need to become experts in those processes, or there needs to be extensive communication between those experts and the programmers. This process is inevitably time-consuming and error-prone, meaning that, on top of the non-coding time that is required, even the code that *is* written may well need rework because of some subtlety or special case that was misunderstood or not fully communicated.

AI-powered AppGen, or the various iterations of low-code or no-code platforms designed for a "citizen developer", look like an end-run around this issue. The person who understands the process — order-to-cash, hire-to-retire, or what have you — can build the automation themselves and cut out all of the misunderstandings.

What's the problem? Software engineering and architecting is about a lot more than basic competency in a programming language. We are no longer living in the days when everything had to be laboriously specified in impossibly terse and platform-specific assembly language; COBOL, the Common Business-Oriented Language, appeared in the 1960s, and was designed precisely to automate common administrative data processing tasks. Writing out a logical flow in a modern programming language is not particularly complex — and AI coding assistants have taken auto-complete to a level where the barrier to entry is basically a minor speed bump.

But that is not an *application*. Generating an entire application, even a relatively trivial one, is a whole other level. Sure, you can *do* it, but the resulting app is not anything that you should put into production. You can use it for a one-shot task, but even if the logic is fully correct, it's almost certainly filled with performance and even logic issues that only arise in certain situations, and which would need to be uncovered with the same sort of rigorous testing that human-generated code would be subjected to. And who writes the tests?

Let's not even talk about maintainability. I have seen far too many demos where the vibe-coded app looked great — but even the most trivial question or request for a change derailed the whole conversation, as the structure behind the demo app was completely opaque to its nominal creator. I talked about this problem in [my very first Coffee Talk video](https://www.youtube.com/watch?v=HnXnRolCyX8):

> It's easy — some might say, all too easy — to stand up a cool demo with AI and get everyone excited… And it's a lot harder to get it to production scale and delivering value.

This is not a problem that can be obviously solved with better models, more tokens, or wider context windows. In fact, current evidence is that the performance of models gets *worse* the longer the user session lasts. In other words, even if the actual code can be generated by AI, the architecture that it fits into and operates within still needs to be designed by expert humans. The AI can accelerate their work, sure, but only for certain tasks, not for the whole job.

![Drawing out a user interface on paper](/images/kelly-sikkema-gcHFXsdcmJE-unsplash.jpg)

# Interfaces Are For Users

Coming all the way back to the point: who is this supposed future vision of chatbots and vibe-coded apps supposed to be *for*? On the provider side, the only constituency for such a vision is the makers of the chatbot interfaces themselves — and there can only ever be a handful of those. For everyone else in the value chain, this vision amounts to ceding a huge part of their customer experience to a third party — something which I have [advised against]({% post_url 2017-02-14-Own-Your-Interfaces %}) in the past.

User experience is not only, or even primarily, a technical problem. Even assuming a chatbot that makes all of its data interfaces perfectly fungible, there will always be complexities to be addressed in what that data encodes and represents. 

Let's take that ubiquitous example of travel booking. I do actually need to go to London in November for [Integreat 2025](http://snaplogic.com/integreat-tour/london?utm_source=MKTG&utm_medium=REF&utm_campaign=2025_1104_EV_EMEA_Integreat-Tour-London&utm_content=MKTG-Dominic-Wellington-25), so I tell my hypothetical chatbot to book me flights and a hotel.

Already we hit a snag: even counting only direct flights between Milan and London, there are half a dozen carriers, ranging from flag carriers to discount airlines, offering flights at different times of day, and probably tens of thousands of hotels in London. How are we narrowing that down?

- Assume the bot has a profile of me, with my loyalty cards, travel preferences, and budget — and since this is a work trip, applicable expense policy[^2]. 

- Assume further that the bot knows my schedule for the trip, so it can filter by time of arrival, hotels within a reasonable distance, and so on.

- And of course, assume that each airline, hotel chain, and travel-booking portal has some sort of interface that the bot can communicate with — and do so in a reasonable amount of time.

That's starting to look like a lot of assumptions, but okay, we now have a list of suitable flights and hotels. How do I decide which to book?

Maybe two airlines have a similar up-front price, but one will charge me for a cabin bag, leading me to check a bag instead, which needs extra time at both ends of the trip. Maybe two hotels have a similar room price, but one is in a chain where my loyalty status gets me free fast wifi, while the other is a nicer hotel, but it's off the Tube network, meaning more time in transit.

Maybe a conversation with the AI bot can help me make these determinations, but we are back to discrete tasks again. It's not a fire-and-forget request; it's a whole process, spanning many different disconnected systems. If the operators of those systems design their *human-facing* interfaces well, I can get through the whole process much faster using those specialised tools, rather than trying harder and harder to contort a general-purpose tool until it conforms to my will.

That general-purpose AI tool can still be useful, mind you. I lived in London for years and still visit frequently, so in this case I wouldn't need a bot's assistant, but when visiting a city I'm not familiar with, something that would be useful would be a quick update on the state of the travel network, any planned strikes or weather events which might affect my trip, and any fun events I might want to catch in my (entirely hypothetical) downtime. But none of that requires the omniscient planning bot I described above for the sake of assumption. It's more of a set of open questions: "what's the best way to get downtown during rush hour" or "I have two hours free on Wednesday morning, what current exhibitions are open then".

![A busy office](/images/arlington-research-kN_kViDchA0-unsplash.jpg)

# Back To The Office

In the enterprise world, this means that you can't just put a chatbot in front of your users and call it good. You have to put some thought and effort into designing a service for them. AI will make some of the work easier, and it may open up some unexpected use cases: MCP has the potential to make it much easier to connect existing systems and data to AI tools, instantly improving both sides. But somebody has to do the work to define what those tools are, think about the regulatory and policy implications, and put some security around the data.

There is a tendency to leap to the fun and creative part of any job. In programming, this is known as the WHISCY problem: **W**hy **H**aven't **I** **S**tarted **C**oding **Y**et. AppGen vibe-coding tools make it even easier to create something, and get the dopamine hit from doing so — but the hard part of the work is still there, and still needs [hard-won experience]({% post_url 2021-04-11-The-Changing-Value-Of-Mistakes %}) and expertise.

As I said in [that recent Coffee Talk video](https://www.youtube.com/watch?v=5XgllDpWaGg), it's all about the process. Adding AI to an existing process requires understanding of the AI, yes, but also of the process. And there is no AI shortcut for that.

***

🖼️  Photos by [Jahanzeb Ahsan](https://unsplash.com/@jahan_photobox), [Nick Rickert](https://unsplash.com/@nick_rickert), [Kelly Sikkema](http://inkypixelsdesign.com/), and [Arlington Research](http://www.arlingtonresearch.global/) on [Unsplash](https://www.unsplash.com)

[^1]: Not linking to the source because it's actually an aside in the pursuit of a different point; it just happened to be the representative example that pushed me over the line.

[^2]: The most important unwritten rule of expenses: "make sure the sales person is buying", with its corollary "and there's a customer there too so their name appears on the expense claim".