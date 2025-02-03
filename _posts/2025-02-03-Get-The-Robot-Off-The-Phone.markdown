---
layout: post
title: Get The Robot Off The Phone
date: 2025-02-03
categories: AI support
---

One of the situations in which we see AI already being rolled out to replace human jobs is in customer service. See for instance [this recent example](https://www.linkedin.com/posts/eoghanmccabe_more-and-more-well-see-people-realize-that-activity-7290496199181090817-mh9r) from Eoghan McCabe, CEO and founder at Intercom: 

> More and more we’ll see people realize that AI is just better than humans. I feel like we’re about two years out from the majority of consumers preferring to speak with an AI agent than a human. Our research shows that ~65% of tickets closed by human agents don’t actually resolve the customer problem. And average customer service response times in different reports have hovered around 12 hours. I really admire the customer service leaders who are embracing these truths and racing to the future with agents. Their customers will love them for it.

I agree insofar as way too many human-mediated customer service experiences are terrible. This is why the only time I call up a customer-service line is because I already tried and failed to accomplish whatever task or find whatever piece of information through other channels. This is also why I get *incandescently angry* at repeated nudges to "go to the website" or "download the app" that come between me and speaking to a competent human being who can address whatever edge case I have unearthed.

I can't imagine the AI being much help to me in those situations either; it's only going to replace the lowest-quality human interactions. 

# Time For A Story

Way back when rocks were warm, I worked in technical support. We had a classic three-tier setup: 

- Tier One answered incoming calls and tried to solve them directly. 
- Anything that could not be addressed at Tier One got escalated to Tier Two, which was staffed by experts who could focus on harder problems without the distraction of incoming phone calls. 
- Tier Three was the actual developers of the product; if something got that far, it meant it was some sort of major problem, requiring code changes at some level to resolve it.

One day, the company decided to hire outside contractors to work as Tier Zero — effectively, a phone firewall to take some of the load off of Tier One. The idea was that they would answer the RTFM[^1] questions, the ones that were *actual* Frequently Asked Questions. Now we were supporting products with five- and six-figure price tags, ones that required programming experience to use, so the average technical level of the questions was generally fairly high — although this did not prevent me from having to explain to one customer how to use notepad.exe… 

*Anyway*, this meant that the contractor staff should answer the phones and respond with a relevant FAQ article, and escalate to Tier One if that did not solve the problem. Simple and foolproof, right? How could such a plan fail to succeed?

Well, fail it did, and so spectacularly that my notoriously cost-conscious employer (still the only company that has made me share a room with a colleague on business trips) paid an actual penalty fee to get out of the contract early, because of how bad the impact of Tier Zero was on customer satisfaction.

The problem was that the Tier Zero contractors were, yes, responding with FAQ articles — but apparently they were selecting them by rolling dice, because the responses rarely had anything to do with the actual question.

![Robots back to back](/images/brett-jordan-5L0R8ZqPZHk-unsplash.jpg)

# What Was The Question Again?

I have no doubt that AI could improve on that performance. However, even then, with a website that would be considered fairly rudimentary by today's standards, most of the FAQ-level questions were dealt with by customers looking up the answers for themselves. The questions that came to us were always the weird ones: "I'm doing what the doc says and getting a different result", "I think I understand this but want to validate my understanding", or "what does this error message mean that is not listed in the public support pages?"

The AI *may* be able to validate a user's understanding, and could potentially use an internal document base to answer question that are not in the customer-facing site — although why you would wire a public AI up to something that is not customer-facing is an important question! But most of the questions I dealt with back in the day needed some combination of actual investigation and hand-holding of the customer. 

As with most proposed applications of AI, the question of whether the AI is worth its GPU runtime is one of trade-offs. IF the AI can reduce the rate of tickets closed without solving the customer's problem below the 65% cited by the Intercom CEO, that is good. BUT, what is the rate of customers whose problem cannot be solved by the AI, and who are at best delayed along the way to getting a resolution? To know whether the deployment of the notional AI-staffed Tier Zero is a good idea, you have to quantify those two aspects, and then factor in the cost of deploying and operating the system. 

It may of course be the case that you're in a business that has a huge proportion of basic FAQ requests, and so the above equation gives an unambiguous result in favour of deploying the AI Tier Zero. In other situations, it's not as simple as just deploying something that can identify a relevant FAQ article 95% of the time. But it's up to the humans to know the difference.

Otherwise consumers will start deploying their own AIs to get them through phone trees, and we end up in the old joke about modems sounding like robots screaming at each other, except the screams are encoded PDFs being passed back and forth.

***

🖼️  Photo by [Brett Jordan](https://unsplash.com/@brett_jordan) on [Unsplash](https://www.unsplash.com)

[^1]: Read The Fine Manual. Less customer-friendly versions of the acronym also exist with alternative interpretations for the F.