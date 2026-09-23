---
layout: post
title:  Personal Data Silos
date:   2026-09-23
categories:  AI Meta Amazon privacy
---

I have written before that [the reason I have doubts about the potential of personal AI assistants is that what we still laughingly call our "private" lives are just not legible to machines]({% post_url 2026-07-07-Absent-Intelligence %}) in the way they would need to be for such a thing to be useful. So far, all the attempts to capture more information about us come across as straightforwardly creepy to everyone who is not already fully committed to enabling the rise of their Machine God.

Here is the *other* reason to be suspicious of the prospects of everyone getting their personal AI butler any time soon: companies think *they* own our data, as when [Amazon blocks Meta’s Muse AI assistant](https://www.geekwire.com/2026/amazon-blocks-metas-muse-ai-assistant-in-new-standoff-over-agentic-shopping/):

> Amazon says it has cut off Meta’s new Muse personal AI agent from shopping on Amazon.com on behalf of customers, after attempting unsuccessfully to get the Facebook parent company to voluntarily exclude the e-commerce site from the experience.
> 
> The problem, Amazon says, is that it never agreed to any of it. Meta didn’t tell Amazon that Muse would access its store, the agent doesn’t identify itself when it browses, and it appears to capture and store customer credentials, which the company says could create privacy and security risks.

![Alanis thinks that's a little too ironic](/images/alannis-morisette-ironic-for-millenials.jpg)

Oh, now *they* are on the receiving end of exploitation by AI, companies are complaining that they "didn't agree to any of it"? Where can *I* opt out of having AI bots access my information, or complain about it not identifying itself, or capturing and storing my credentials in ways that actually do create privacy and security risks? It's particularly galling when the leaks are all so *predictable*, and indeed predicted, like when [153M+ drivers licenses show up for sale on the dark web](https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/) and are quickly traced back to “a major identity verification company” that couldn't even be bothered to perform the minimum data hygiene of deleting the files once the verification was complete.

# Who owns the data?

Even if we set aside the crucial issue of consent for just a moment, Amazon is acting like the information belongs to Amazon. After all, [Amazon already removed a lot of information from their tracking emails](https://daringfireball.net/linked/2020/06/01/product-info-in-amazon-emails), precisely to prevent it from being harvested from customers' inboxes — including by those customers themselves. 

Meanwhile Amazon's customers could say that it's *their* information, thank you very much, and they will make their own choices about whether to let Muse (or Apple Intelligence, or whatever other assistant) access it or not. 

This is the world we live in, where we do not actually *own* any of the things that we think we own. If I "buy" a film or a book from Apple, technically I do not own the thing itself, but a license to reproduce it under certain conditions, and which can be revoked at any time without any recourse on my part. This issue is not specific to Apple: Sony Playstation owners were surprised and dismayed to learn in June that they would [lose access to Studio Canal titles from their video libraries due to “licensing agreements”](https://www.playstationlifestyle.net/2026/06/26/purchased-studio-canal-content-removed-playstation-library/) — after exactly the same happened to purchased Discovery TV shows back in 2023.

![Old-school book shopping](/images/eddie-junior-kZ7Mc7yo1-8-unsplash.jpg)

# Metadata — data *about* data

It might seem logical that users cannot export the films themselves due to the risk of piracy, but this lack of ownership also extends to the *metadata*. If I wanted to get better film recommendations by building an AI agent to run an analysis of my media habits across Apple TV+, Netflix, PrimeTV, and whatever else, I would be at the mercy of whether those services allowed me to access my own data in any meaningful way (answer: hahaha, *nope*). It sounds like PrimeTV at least would be right out, based on this current news story, and without trawling through their labyrinthine user agreements, I think it's a safe assumption that the others are no different. 

Each of these services would like us to be in an exclusive one-to-one relationship, but the reality is that even an Apple diehard like me also watches content from elsewhere — so recommendations from Apple that miss what I watch on Netflix are not as useful to me. But if I can't extract the information from each platform, because the operators consider it *their* proprietary information, not mine, then my hypothetical robot butler isn't going to be able to recommend anything useful.

*** 

This is incidentally why a lot of AI tools focus on pretending to be humans, driving "headless" web browsers and so on, rather than doing the thing that is obvious in computer science terms and connecting to a clean back-end interface that is designed for the purpose. In the enterprise we mostly moved away from doing Robotic Process Automation by driving the same graphical user interfaces that people access, because they are not really designed for the purpose, and there is a huge overhead in both designing and operating the automation. 

But even in the enterprise world, one of the stumbling blocks for automation that goes beyond the scope of a single department is disconnected silos of data that are owned by different teams with different goals. The rise of Software-as-a-Service (SaaS) delivered via the cloud means that different providers may also try to insert themselves in that conversation, as we saw when [Salesforce blocked Glean from indexing "its" Slack data](https://www.reuters.com/business/salesforce-blocks-ai-rivals-using-slack-data-information-reports-2025-06-11/). Actually, of course, Salesforce customers were under the impression that their Slack conversations and other data belonged to *them*, meaning they were free to search it with Glean or whatever other tool.

In the consumer world, where the silos are all owned by different companies except where someone has gone to significant effort to avoid committing to e.g. streaming music, video, and games, we are way past that point, which is why the vendors concerned can enforce such rigid isolation.

*** 

# But what is it all *for*?

There is of course a further question: even assuming we could get all of this data, how much use could or would we really make of it? 

This was my contention with the "quantified self" movement a few years ago, where people tried to gather all sorts of data about themselves. My issue was that, for most people, the process stopped with the creation of a dashboard. None of the data was really *actionable*.

![New Apple readiness score](/images/Apple-Watch-Ultra-4-readiness-260909_big.jpg.large_2x.jpg)

This is the same problem with Apple's new measurement of how ready Apple Watch wearers are for the day: what use is it to tell me that I am not at all ready, if I have to get going anyway? Kids must be got to school, work must get done, and unless I'm really dead, some sort of workout probably needs to happen too, because the week is tightly scheduled and I don't really have the leisure of waiting for a perfect night of sleep (insert hollow laugh here).

Philosophically I do wish that all of our data were more easily legible and even editable to us. I even think [opening up more access to data would be better *for the vendors*]({% post_url 2022-03-16-Help,-I'm-Being-Personalised! %})! But at this point I see very little possibility of that happening — although I do look forward to enjoying the "let's you and him fight" aspect of watching Meta and Amazon duke it out over access to users' data. But for myself, I remain convinced that the value of AI is going to be realised first in the enterprise, simply due to the availability of data, and later if ever in the consumer space, because of the lack of easy access to data — whether for technical reasons, or commercial ones, or simply because we find it all a bit creepy.

*** 

🖼️  Photos by [Eddie Junior](https://www.instagram.com/iameddiejr/) on [Unsplash](https://www.unsplash.com); Apple Watch readiness score image from [Apple Watch press release](https://www.apple.com/newsroom/2026/09/apple-advances-health-and-fitness-capabilities-using-apple-intelligence/)