---
layout: post
title:  The Ghost In The Machine 
date:   2023-08-30 
categories:  AI MongoDB ChatGPT 
---

# The Ghost In The Machine


At this point in time it would be more notable to find a vendor that was *not* adding “AI” features to its products. Everyone is jumping on board this particular hype train, so the interesting questions are not about whether a particular vendor is “doing AI”; they are about how and where each vendor is integrating these new capabilities.

I no longer work for MongoDB, but I remain a big fan, and I am convinced that generative AI is going to be good for them — but something rubbed me up the wrong way about how they communicated some of their new capabilities in that area, and I couldn’t get it out of my head.

# Three Ways To “Do AI”

Some of the applications of generative AI are real, natural extensions of a tool’s existing capabilities, built on a solid understanding of what generative AI is actually good for. Code copilot (aka “fancy autocomplete”) is probably the leading example in this category. Microsoft was an early mover here with Github and then VS Code, but most IDEs by now either already offer this integration, or are frantically building it.

Some applications of AI are more exploratory, either in terms of the current capabilities of generative AI, or of its applicability to a particular domain. [Sourcing and procurement](https://www2.deloitte.com/us/en/blog/business-operations-room-blog/2023/generative-ai-in-procurement.html) looks like one such domain to me. I spent more of this past summer than I really wanted to enmeshed in a massive tender response, together with many colleagues, and while it would have been nice to just point ChatGPT at the request and let it go wild, the response is going to be scrutinised to such a level that the amount of editing and review of an automated submission that would have been required is the same as, if not greater than, the effort required to just write the response in the first place. However, I am open to the possibility that with some careful tuning and processes in place, this sort of application might have value.

And then there is a third category that we can charitably call “speculative”. There is a catalogue of vendors trying this sort of thing that is both inglorious and extensive, and I am sad to see my old colleagues at MongoDB coming close to joining them: [MongoDB adds vector search to Atlas database to help build AI apps](https://www.infoworld.com/article/3700728/mongodb-adds-vector-search-to-atlas-database-to-help-build-ai-apps.html).

![](/images/114805.jpeg)

> *young developer: "Wow, how did you get these results? Did you use a traditional db or a vector db?"*
> *me: "lol I used perl &amp; sort on a 42MB text file. it took 1.2 seconds on an old macbook"*
> *from [Mastodon](https://xoxo.zone/@neilk/110962856306779380)*

I have no problem with MongoDB exploring new additions to their data platform’s capabilities. It has been a long time since MongoDB was just a noSQL database, to the point that they should probably just stop fighting people about including the “DB” at the end of their name and drop it once and for all — if that shortened name didn’t have all sorts of unfortunate associations. MongoDB Atlas now supports mobile sync, advanced text search, time series data, long-running analytical queries, stream processing, and even graph queries. [Vector search](https://www.mongodb.com/products/platform/atlas-vector-search) is just one more useful addition to that already extensive list, so why get worked up about it?

# Generative AI Is Good For MongoDB — But…

The problem I have is with the framing, implying that the benefit to developers — MongoDB’s key constituency — is that they will build their own AI apps on MongoDB by using vector search. In actuality, the greatest benefit to developers that we have seen so far is that first category: automated code generation. Generative AI has the potential to save developers time and make them more effective.

In its [latest update to the *Gartner Hype Cycle for Artificial Intelligence*](https://www.gartner.com/en/articles/what-s-new-in-artificial-intelligence-from-the-2023-gartner-hype-cycle), Gartner makes the distinction between two types of AI development:

> - Innovations that will be fueled by GenAI. 
> - Innovations that will fuel advances in GenAI.

Gartner's first category is what I described above: apps calling AI models via API, and taking advantage of that capability to power their own innovative functionality. Innovations that advance AI itself are obviously much more significant in terms of moving the state of the art forward — but MongoDB implying that meaningful numbers of developers are going to be building those foundational advances, and doing so on a general-purpose data platform, feels disingenuous. 

Of course, the reason MongoDB can’t just come out and say that, or simply add ChatGPT integration to their (excellent and under-appreciated) Compass IDE and be done, is that the positioning of MongoDB since its inception has been about its ease of use. Instead of having to develop complex SQL queries — and before even getting to that point, sweat endless details of schema definition — application developers can use much more natural and expressive MongoDB syntax to get the data they want, in a format that is ready for them to work with.

But if it’s so easy, why would you need a robot to help you out?

And if a big selling point for MongoDB against relational SQL-based databases is how clunky SQL is to work with, and then a robot comes along to take care of that part, how is MongoDB to maintain its position as *the* developer-friendly data platform?

Well, one answer is that they double down on the breadth of capabilities which that platform offers, regardless of how many developers will actually build AI apps that use vector search, and use that positioning to link themselves with the excitement over AI among analysts and investors.

# I Come Not To Bury MongoDB, But To Praise It

None of this is to say that MongoDB is doomed by the rise of generative AI — far from it. Given MongoDB’s position in the market, an AI-fuelled increase in the number of apps being built can hardly avoid benefiting MongoDB, along the principle of a rising tide lifting all boats. But beyond that general factor, which also applies to other databases and data platforms, there is another aspect that is more specific to MongoDB, and has the potential to lift its boat more than others. 

The difference between MongoDB and relational databases is not just that MongoDB users don’t have to use SQL to query the database; it’s also that they don’t have to spend the laborious time and effort to specify their database schema up front, before they can even start developing their actual app. That’s not to say that you don’t have to think about data design with MongoDB; it’s just that it’s not cast in stone to the same degree that it is with relational databases. You can change your mind and evolve your schema to match changing requirements without that being a massive headache. Nowadays, the system will suggest changes to improve performance, and even implement them automatically in some situations.

All of this adds up to one simple fact: *it’s much quicker to get started on building something with MongoDB*. If two teams have similar ideas, but one is building on a traditional relational database and the other is building on MongoDB, the latter team will have a massive advantage in getting to market faster (all else being equal). 

At a time when the market is moving as rapidly as it is now (who even had OpenAI on their radar a year ago?), speed is everything. MongoDB could have just doubled down on their existing messaging: “build your app on our platform, and you’ll launch faster”. What bothers me is that instead of that plain and defensible statement, we got marketing-by-roadmap, positioning some fairly basic vector search capabilities as somehow meaning hordes of developers are going to be building The Next Big AI Thing on top of MongoDB.

![](/images/114635.1.png)

Marketing-by-roadmap this way is a legitimate strategy, to be clear, and perhaps the feeling at MongoDB is that this is fair turnaround for all the legitimate features they built over the years and did not get credit for, with releases greeted with braying cries of “MongoDB is web scale!” and jokes about it losing data, long past the point when that was any sort of legitimate criticism. Building this feature and launching it this way seems to have got MongoDB a tonne of positive press, and investors expect vendors to be building AI features into their products, so it probably didn’t hurt with that audience either.

Communicating this way does bother me, though, and this is one feature I am glad that I am no longer paid to defend.

                             