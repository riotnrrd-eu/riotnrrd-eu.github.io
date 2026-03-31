---
layout: post
title:  Networked Intelligence
date:   2026-03-31
categories: AI OpenAI Anthropic Claude Facebook
---

Everyone just *assumes* that developers of the big public "AI" models are taking user data and using it to train the next generation of their models. The AI labs in question deny this accusation vociferously, of course, but given the lengths they have been willing to go to in order to obtain data corpora to train their models on, those denials ring somewhat hollow to many. And of course it doesn’t help when it comes out that Meta actually *is* retaining video taken through its pervert glasses, leading the EFF to recommend that people should [*Think Twice Before Buying or Using Meta’s Ray-Bans*](https://www.eff.org/deeplinks/2026/03/think-twice-buying-or-using-metas-ray-bans).

Being suspicious by default of whatever Zuckerberg is up to is not a bad heuristic shortcut. However, there is another reason why this claim keeps coming back. One of the assumptions that people bring to "AI" from previous generations of technology is that some sort of network effect is required for market success. A network effect means that the more users you have, the more valuable your product is, making it easier and more profitable to serve even more users.

The classic example of a network effect is Facebook — not now, but how it was in the growth stage of the platform, say fifteen years ago. Once enough of your friends are on Facebook, it's a no-brainer for you to join too, so Facebook gains an additional set of eyeballs to rent to their advertisers, and crucially, at very little added cost. Each additional user is basically pure profit, not only in themselves, but because they contribute in turn to making the platform that little bit more attractive to anyone in their social circle who is not yet on Facebook.

An example of a business which *lacks* a network effect is Spotify. Sure, each additional user pays their monthly fee, but they also cost Spotify, because as miserly as the payouts to musicians are, they do add up and hit Spotify's margin. There is also no particular flywheel effect leading to people wanting to sign up to Spotify just because that’s where their friends are. I'm an Apple Music user, and I have never felt left out because more of my friends are on Spotify.[^1] This is why Spotify is pushing into podcasts, because once Joe Rogan has been paid once to record an episode, each additional stream of that episode does not cost an additional license payment — and of course plenty of people are willing to make podcasts for free or to monetise in other ways, which also do not cost Spotify anything.

These are concepts which are now embedded in our culture and in our expectations. Even people who perhaps could not quite articulate the concept in this way understand that user data has value to social-media platforms. This assumption colours a lot of the conversation around "AI", in ways that are not always entirely helpful.

# Networking AI

The assumption that many commentators make is that by having more users, OpenAI (or whoever, but ChatGPT has the biggest market share right now) can obtain more data from that larger user population, use that data to train subsequent iterations of the underlying model, and therefore improve the models' performance more rapidly than competitors with smaller user bases.

There are a few things wrong with this assumption. 

![Denial is not just a river in Egypt](/images/saif71-com-zPhc-E4qG9c-unsplash.jpg)

### Deny everything

The first aspect to consider is the vehement denials by every frontier lab out there. Sure, they *could* all be lying because they realise how unpopular “stealing users’ data” was for the social-media behemoths — but you’d expect one of them to break ranks and say “yes, yes we do have more user data, and that’s what makes our model better for our users”. Given all of the other indignities that chatbot enthusiasts put up with, this could well be a positive move for the first vendor to make that claim, at least within a certain susceptible population. In turn, the fact that there could be a positive outcome means that the denials should not be dismissed out of hand.

### Not all users are equivalent

Sam Altman's preferred metric of Weekly Active Users tells us that, while the absolute number of users of ChatGPT may be large, the level of usage for individual users is not that high. In turn, this means that the richness of data from each user is probably low. If someone is only logging in once a week on average, how deep are the conversations they are having with the bot, and consequently, how much value can be harvested from that corpus?

In contrast, Anthropic's Claude has a small absolute number of users relative to ChatGPT, but is the preferred option for power users, who are not only paying Anthropic (in actual dollars), but also feeding Claude with huge amounts of extremely rich data. 

But then the question becomes, what is the actual total market for a tool like Claude, whose primary use case appears to be highly technical tasks like code generation?

So maybe the reason nobody is bragging about "having more user data" is that it’s not actually a competitive moat. OpenAI has access to large absolute amounts of data, but diluted across so many user sessions that there is little value to be extracted. Meanwhile, Anthropic has very high-value data, but only for a small and non-typical user population.

What else might differentiate one frontier model from another, and do so consistently over time?

![Compute is king](/images/krzysztof-hepner-EkXSNquusLk-unsplash.jpg)

### What about compute?

One candidate for differentiation is computing capacity, or simply ["compute"](https://fromjason.xyz/p/notebook/the-computational-web-and-the-old-ai-switcharoo/):

> If all technology requires AI, and only a handful of companies are equipped to handle the computational load that AI requires, then compute itself becomes a moat too deep for competition to enter, and consumers to flee from.

This is the theory underlying a lot of investment activity in this sector: if Oracle can build a datacenter stuffed with Nvidia chips and lease it to OpenAI, that leaves Anthropic high and dry: no datacenter, no chips available to buy, and no finance to buy them with. In that case, the datacenter is worth almost any amount of money, because the value is not just positive ownership of the datacenter and its contents, but also the negative value to competitors of keeping the resources out of their hands (digits?).

The problem is that anyone advocating this view is arguing against some trends that have been stable over periods of time that are very long, in tech-industry terms at least. For this sort of investment to work out, there needs to be a window of time when the datacenter is operational but not yet obsolete, and that window needs to be long enough for the datacenter to recoup the costs of its construction and ideally generate some surplus profit for its operators. 

Some factors in that calculation are (more or less) within the control of the operators: how quickly can they break ground and then complete construction and fit-out. Others are not: how quickly new hardware comes to market that performs better than whatever was specified for the datacenter. Where the calculations get hairy is that this is not just a question of new generations of server-grade Nvidia GPUs, but also of how quickly consumer hardware evolves to bring sufficient capacity to run capable local models within the reach of hobbyists.

Marco Arment wanted to provide transcripts of every podcast in his Overcast app. Did he sign up with one of the big providers? No: [he got a rack full of Mac Minis](https://www.twit.community/t/marco-arment-implements-transcripts-in-overcast-what-is-the-future-of-podcast-advertising/19811) — base models, at that — and set them loose using Apple’s own transcription APIs. Marco is a one-man-band; how many others are doing something similar, or might if the price of their AI subscription rises enough? 

That is no academic concern, with [Anthropic lowering session limits on Claude](https://www.businessinsider.com/claude-usage-caps-changes-popularity-anthropic-2026-3), even for paid accounts: 

> ~7% of users will hit session limits they wouldn’t have before, particularly for pro tiers.

The safe assumption has to be that this price increase is only the first turn of a ratchet. Anthropic is presumably hoping that Claude users will become habituated to regular price rises in the same way that Netflix customers have. However, the salient difference between the two situations is that Netflix actually does have a moat. If you want to watch *Drive To Survive* or *K-Pop Demon Hunters*, an Amazon Prime subscription won’t help you: it has to be Netflix. 

What is the equivalent dIfferentiation for the big AI models? That is the big question, and it remains unanswered for now.

*** 

🖼️  Photos by [Saif71.com](https://saif71.com/) and [Krzysztof Hepner](https://chrishepnermedia.wordpress.com/) on [Unsplash](https://www.unsplash.com)

[^1]: Very occasionally someone shares a Spotify playlist that I want to listen to, but these days there are tools to convert playlists between platforms. The content libraries themselves, though — those are entirely fungible.