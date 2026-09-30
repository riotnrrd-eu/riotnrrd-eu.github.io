---
layout: post
title:  Delegated Interfaces
date:   2026-09-30
categories:  AI UX
---

We receive news. Apparently, [*The Death of Apps Has Already Begun*](https://webdesignerdepot.com/the-death-of-apps-has-already-begun/). However, upon reading further, I have doubts about this author’s understanding of how humans live. This lack of understanding is quite possibly due to the fact that the piece emits a quite suffocating stench of AI slop. In fact, the whole thing put me in mind of this guy, who is getting roasted all up and down Bluesky:

![Tweet by @nicksaraev: "I am not joking when I say this. Spotify, Apple Music, and streaming in general is over. Al music is now very, very good. You just don't know yet because all Al music circulating today is from ~2-3 generations ago. Suno v6 pro et al has solved infinite personalized music.](/images/bafkreicdzuh6jjfs7ivtohu7ulaqu6aaj2xthbcek5mv3yj5cm2hvvxktq.png)
#### "Solved music", Cthulhu help us all

Anyway, one of the arguments for why we should abandon dedicated apps in favour of a single general-purpose AI assistant is this:

> Why browse restaurant listings when your assistant already knows you want?

Of course this argument entirely misses the point of why people go to restaurants. I hardly ever go to a restaurant on my own; maybe when travelling, but even then I generally wind up either in my hotel or in the immediate neighbourhood, rather than going hunting for something very specific. If I go with friends, what exactly is the scenario — we all put our AI butlers in touch with each other and then go with whatever the one with most tokens chose? No, it’s going to be Alice feels like Chinese, Bob wanted Italian, but everyone ends up going for Indian because it was close to Claire’s office.

![A group of friends shares an intimate candlelit dinner at a long wooden table inside a cozy restaurant with warm ambient light.](/images/romain-gal-UEjjO-aJtZ8-unsplash.jpg)

Even beyond the purely human factors, and sticking to the technical aspects of using software, the mode of interaction is very different depending on the task; a single general-purpose interface is by definition not going to be the best at any one specialised task. The demo scenario beloved of every Silicon Valley man-child of “book me flights and hotels, here is my credit card and a *terrifyingly vague* set of instructions” falls down badly as soon as it encounters reality, as I explored [last year]({% post_url 2025-10-08-Oh-Brave-New-World-That-Has-Such-UX-In-It %})

> Let’s take that ubiquitous example of travel booking. I do actually need to go to London in November, so I tell my hypothetical chatbot to book me flights and a hotel.
> 
> Already we hit a snag: even counting only direct flights between Milan and London, there are half a dozen carriers, ranging from flag carriers to discount airlines, offering flights at different times of day, to and from different combinations of airports — and then there are probably tens of thousands of hotels in London. How are we narrowing that down?
> 
> - Assume the bot has a profile of me, with my loyalty cards, travel preferences, and budget — and since this is a work trip, applicable expense policy.
>
> - Assume further that the bot knows my schedule for the trip, so it can filter by time of arrival, hotels within a reasonable distance, and so on.
> 
> - And of course, assume that each airline, hotel chain, and travel-booking portal has some sort of interface that the bot can communicate with — and do so in a reasonable amount of time.
> 
> That’s starting to look like a lot of assumptions, but okay, we now have a list of suitable flights and hotels. How do I decide which to book?
> 
> Maybe two airlines have a similar up-front price, but one will charge me for a cabin bag, leading me to check a bag instead, which needs extra time at both ends of the trip. Maybe two hotels have a similar room price, but one is in a chain where my loyalty status gets me free fast wifi, while the other is a nicer hotel, but it’s off the Tube network, meaning more time in transit.
> 
> Maybe a conversation with the AI bot can help me make these determinations, but we are back to discrete tasks again. It’s not a fire-and-forget request; it’s a whole process, spanning many different disconnected systems. If the operators of those systems design their *human-facing* interfaces well, I can get through the whole process much faster using those specialised tools, rather than trying harder and harder to contort a general-purpose tool until it conforms to my will.

Dedicated apps for each sub-task are simply going to be a lot quicker if I have any external constraints at all.

# Start from step zero

There is an hurdle that has to be overcome even before I get to the point of asking a chatbot to organise my travel schedule. How do I even know that it is capable of doing so, or whether it is any good at the task? How can I discover these capabilities, short of trial & error that could really mess up my trip?

Discoverability was the big problem of command line interfaces, which meant that the learning curve was pretty much vertical. An interface that can potentially do anything is very hard to navigate, because there is no indication of what the possibilities are or how they might be invoked. 

The natural-language conversational capabilities of chatbots are of course a bit easier to navigate than the impossibly terse commands of the UNIX shell, with their impenetrable syntax embedding all sorts of historic constraints and assumptions, but the core problem still holds true: how do you know what you can ask them?

And let’s not forget the second half of the question: even if the thing advertises travel booking as one of its capabilities, or the user somehow discovers that it has that functionality — how can we determine whether to trust it?

The fear that the computer could do bad things is one that has always held users back, and still does today. There is a famous story in Marcin Wichary’s fascinating and extremely *comprehensive* book [*Shift Happens*](https://shifthappens.site "SHIFT HAPPENS - A BOOK ABOUT KEYBOARDS" ) about Bravo, the Xerox PARC editor, and its terrifying failure mode that could result in total data loss simply from typing "edit":

- In Bravo’s command mode, E meant Everything (select everything).
- D meant Delete.
- I meant Insert/Input mode.
- So typing EDIT while already in command mode meant, effectively, Everything → Delete → Insert T.
- Because early Bravo had only one level of undo, you could undo the insertion of T, but not the preceding deletion. Thus the document was effectively wiped.

This is the sort of thing that scares people unused to computers: that a seemingly innocuous set of actions will result in disproportionately disastrous consequences. Familiarity means identifying the signposts that tell us where danger is, and is not. Visible controls in a well-presented app not only make the interface navigable by advertising capabilities, but also illustrate how actions are constrained. The action "add to basket" is different from "pay now"; I might be doing price comparisons in another app or tab, or I might be checking travel directions in my Maps app, and don’t want to finalise a transaction, but I also don’t want to lose a promising candidate.

![This phone does not inspire confidence](/images/hardik-sharma-27mgWH0pzhA-unsplash.jpg)

The existence of the app itself is also a signal. A janky app that has obviously not been updated in a while is a red flag. A full-featured app that is easily navigable is its opposite. I have literally switched utility providers over the quality of the online experience they offered.

# Will gatekeepers let a second horse inside their walls?

Finally, there is a major unspoken assumption here: that where ITA Airlines or the Marriott hotel chain today offer apps that let them engage directly with customers (and try to up-sell them on additional services, let’s not forget), in this agentic future they will meekly offer an MCP server or whatever that any random agent can consume. 

What is the upside for these providers — that they can more easily be disintermediated so that consumers lose any sight of the differentiation they offer compared to Ryanair and Travelodge? It’s far more likely that they will do the opposite, and try to throw up road blocks to this sort of usage — whether technical, legal, or in the form of user incentives. Providers learned their lesson from the rise of Facebook, which lured them in with the promise of direct connections to their fans, and then turned around and charged them simply to ensure that their content was delivered *to people who had specifically signed up to see it*. They will not be in any hurry to elect another gatekeeper, one whose ambition is explicitly to insert itself into every transaction and charge a toll.

# But what about the enterprise?

All of the above goes for the consumer space, because those are the examples in the original piece that I was reacting to. A move away from apps is far more plausible in the business world, not least because it has largely already happened. An app that needs to be provisioned to users' devices is just one more source of friction that gets between vendor and revenue. A web application is easier to build, quicker to update, and more universally compatible. And none of those web apps is *beautiful*; beauty, and even usability, are secondary concerns when the buyer is not the user. In fact, the vibe-coded custom GUI is often a step up in usability, because it is built by someone who is directly involved in whatever the business process is, interacting daily with the vendor-supplied GUI, and sufficiently frustrated by the experience to come up with their own alternative.

[I still don't believe in the SaaSpocalypse]({% post_url 2026-09-11-SaaSpocalypse-Now %}), though: customising the front-end is very different from replacing the back-end. Both will evolve, and may well need to be [repackaged in new and interesting ways]({% post_url 2026-01-09-Cursing-and-Recursing/ %}), but that's a story for another day.

***

🖼️  Photos by [Romain Gal](https://linktr.ee/romgal) and [Hardik Sharma](https://instagram.com/v4ssu) on [Unsplash](https://www.unsplash.com)