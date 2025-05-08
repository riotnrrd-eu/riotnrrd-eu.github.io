---
layout: post
title:  Licentious Licensing
date:   2025-05-08
categories: open-source cloud Redis MongoDB database enterprise
---

The *riveting* topic of open-source licensing is back in the news once again, this time because Salvatore Sanfilippo (aka Antirez) has rejoined Redis and [pushed to re-open-source it under the AGPL license](https://antirez.com/news/151), reversing its recent move to the SSPL:

> My feeling was that the SSPL, in practical terms, failed to be accepted by the community. The OSI wouldn’t accept it, nor would the software community regard the SSPL as an open license.

That lack of acceptance has always been the Achille's heel of the SSPL, as I wrote when [Redis first moved to the SSPL]({% post_url 2024-04-04-Defensive-Moves %}):

> Pleas that the SSPL did not meaningfully restrict _use_ of the software, only its _commercialisation as a service_, fell on deaf ears. My own opinion is that the SSPL respects the _spirit_ of open-source far more than the clear-cutting approach taken by the hyperscalers, but it’s arguably true that SSPL does effectively “discriminate against fields of endeavor” and therefore falls foul of the _letter_ of Clause 6 at least.

![Stalls in a bazaar, as yet unlooted](/images/jean-valjean-OiOLKlYGv94-unsplash.jpg)

With Redis now returning to the AGPL over the SSPL, the consensus take is that this is a win for the open-source camp. See for instance [Stephen O'Grady of Redmonk](https://redmonk.com/sogrady/2025/05/06/oss-forward-back/):

> \[Redis'\] decision to return to an open source license was a consequential one and further evidence of a changing trajectory for the \[AGPL\] license and for open source.
> 
> Nor is it just SSPL projects moving to the AGPL. Grafana and MinIO previously moved from Apache licenses to the AGPL in April and May of 2021, respectively. The Zitadel project, meanwhile, did the same in March.

However, right before that snippet comes this one, referring to the Redis relicensing:

> No mention was made of the unique Redis fork [Valkey](https://redmonk.com/sogrady/2024/07/16/post-valkey-world/) in that post, but it appears in the comments and the idea that it had no role in the internal discussions on the license choice is implausible.

I agree that Valkey must have figured quite prominently in Redis' decision process, in the way that a herd of horses disappearing over the horizon figures in the decision on whether to bother closing the barn door again. Despite Stephen's contention that the timing of the launch of Amazon DocumentDB implies that MongoDB's move to the SSPL was unnecessary, I take the exact opposite conclusion:

> MongoDB could not have moved \[to the SSPL\] much earlier, because there was no alternative to offer those customers — but could not afford to wait much longer, for fear of seeing its user base erode under it. 

I have always failed to see the benefits to users of DocumentDB (or the MongoDB interface in Microsoft Azure CosmosDB, or for that matter the new MongoDB interface in Google Firestore). The existence of these offerings only has value because they are right there in the cloud service provider (CSP) dashboard. This is the sort of thing that open-source proponents rightly decry when the topic is the Apple App Store: the walled garden gives incumbents the ability to shut out technically better solutions. In the case of big CSPs, open-source licenses which do not fully account for the economics of SaaS delivery models are reinforcing that walled garden, not opening it up.

Even if we assume Stephen O'Grady is right and the decision to build DocumentDB was driven purely by the strictures of the AGPL, before the SSPL was published, how does DocumentDB help someone self-managing MongoDB Community on Amazon EC2? We have seen open-source communities ripped apart by this sort of choice between only partly compatible distributions. I remain of the opinion that the SSPL is far truer to the spirit of open-source and to actual users than having doctrinal disputes while both cathedral and bazaar are being looted.

Time will tell whether this is indeed the victory of the open-source AGPL versus the source-available SSPL. The answer of what level of protection is sufficient depends very much on what the question is: should a license protect the viability of an open-source project, or the growth rate of a commercial software vendor? Looking at it that way, it's not surprising that we have such radically different responses.

***

🖼️  Photo by [Jean Valjean](https://unsplash.com/@sprang) on [Unsplash](https://www.unsplash.com)