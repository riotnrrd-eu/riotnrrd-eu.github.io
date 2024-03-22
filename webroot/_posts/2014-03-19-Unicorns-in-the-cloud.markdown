---
layout: post
title:  Unicorns in the cloud 
date:   2014-03-19 
categories:  cloud tech 
---

# Unicorns in the cloud


No, it’s not [what](http://www.ascrewsloose.com/2012/10/25/rainbow-farting-unicorns/) [you](http://diversity.net.nz/the-great-cloud-api-debate-and-vmwares-hybrid-cloud-inside-baseball-unicorns-and-rainbows/2013/09/12/) [think](http://it20.info/2013/12/unicorns-pendulums-and-private-clouds/)… Here “unicorns" are guru-level sysadmins, difficult to find in the wild when you really need them.[^1]

![](/images/unknown_filename.461.jpeg)

The Register [says](http://www.theregister.co.uk/2014/03/14/cloud_skills_extinction/):

> The rise of the cloud is wiping out the next generation of valuable sysadmins as startups never learn about how to manage data-center gear properly

The thesis goes like this: in the old, pre-AWS days (can you believe that’s only eight years ago?) you and your friends would start a company and code up a demo on your be-stickered MacBooks at the local independent coffee shop. Once you had your demo, you would take it to VCs in order to get funding to buy some servers, host them in a data center somewhere, and start building your infrastructure. This would require professional sysadmins who would gain experience taking a tool to production scale, and so there was good availability of sysadmins who had that experience.

Nowadays, those be-stickered MacBooks might represent *the entire IT estate* of a startup. Everything else runs in the cloud somewhere - probably in AWS. Now this is great from some points of view: by definition, startups don’t know what their adoption rate is going to be, so having AWS’ effectively infinite pool of capacity to fall back on is very useful in case they get Slashdotted[^2] one day. Vice versa, they don’t get stuck paying the bills for an oversized data center if take-off turns out to require a bit more time than they had initially hoped.

So far, so good. The problem is when that startup’s business has more or less stabilised, and they would like to move the more predictable parts of their infrastructure from expensive AWS[^3] to more traditional infrastructure. They do not have the skills in-house to do this because they have never needed to develop them, so they need to hire sysadmins in a hurry.

> This pattern has played out at numerous startups, including ephemeral messaging service Snapchat which started life on Google App Engine and then hired away senior Google cloud employee Peter Magnusson to help it figure out how to move bits of its workload off the cloud.
>
> Similarly, backend-as-a-service company Firebase started out life on a major public cloud but had to shift to bare-metal servers after it ran into performance issues.

Now, if you’re in the position to hire senior Google employees in a hurry, then your startup is doing well and I congratulate you. However, what about all the *other* startups without the sort of public profile that Snapchat enjoys?

Draining the sysadmin talent pool is a real problem because there is no straight career path to get there. Sysadmins have be talented generalists, able to work at different levels of abstractions, pivot rapidly in response to changing technological realities, and react quickly to tactical requests while working towards strategic objectives. You can’t get a degree in any of that, you need to learn by doing. I know, I’ve been there, done that, got the T-shirt[^4]. I caused my mentors a certain number of headaches during the learning process, but I came out of it with valuable experience. Ultimately my poor timing meant that the bubble burst, sysadmins jobs were in short supply, and I had to take my career in different directions, although a certain generalist/tinkerer aspect has been a constant.

Also, sysadmin knowledge is pretty specific. Even if you are able to find a Linux guru who has done it all, partied with Linus and argued ESR to a standstill, it will still take some time to get them hired and up to speed in your environment. Congratulations: now your inability to hire and onboard sysadmins more rapidly is a bottleneck on your business growth. A slowdown in growth is **NOT** what you want in a startup. You want a nice steep growth curve, with no interruptions or even temporary flattenings.

I suspect many business models include an unspoken assumption of “and then we’ll open our own datacenter”. Not many people appear to be thinking about the business risk involved in that step, especially the human factors.

Note: I am *absolutely not* advocating staying away from the public cloud! If a workload is bursty and unpredictable, as most startups are by definition, the public cloud is a very good fit. The same applies to traditional enterprises operating services with those characteristics - even if they have some cultural obstacles to adopting the cloud. On the other hand, a static repository of large binaries, say, or a service with extensive compliance requirements, may well be better off on more traditional infrastructure.

If the premise of the article is true, and traditional sysadmins skills are becoming more rare, it may be tougher than expected to transition to a traditional on-premise or managed-hosting model. Business plans and product roadmaps will need to allow for both the technical aspects and the business risk aspects.

If you are lucky enough to have generalists around, don’t try to pigeonhole them. Look after your sysadmins, and they’ll look after you.

***

In one of those displays of serendipity, I just finished reading [this article](http://www.bostonreview.net/forum/suzanne-berger-how-finance-gutted-manufacturing) over my lunch break. It seems the problem is not limited to IT, but is generalised throughout the economy.

A generalised problem would seem to be harder to solve, but in IT we pride ourselves on being able to break these sorts of deadlocks. What is the solution that combines short-term benefits with long-term ones to the detriment of neither?

[^1]: This is a mature, professional and non-discriminating blog, so nobody will make any jokes about hunting both sysadmins and unicorns using young nubile women as bait.
[^2]: I know, showing my age there!
[^3]: I have a vague memory of a study showing AWS (as a proxy for public cloud in general) could be as much as 25% more expensive over time for certain types of steady-state workloads once you factor in bandwidth. However, I can’t lay my hands on it right now. If I find it, I will update this post.
[^4]: Black, of course, and emblazoned with the following slogan: `select * from USERS where CLUE > 0; 0 rows returned`

