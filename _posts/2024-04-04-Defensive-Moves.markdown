---
layout: post
title: Defensive Moves
date: 2024-04-04
categories: Redis MongoDB database open-source enterprise
---

The news of the day is that [Redis has changed its licensing](https://techcrunch.com/2024/03/21/redis-switches-licenses-acquires-speedb-to-go-beyond-its-core-in-memory-database/), moving from the nice simple [3-clause BSD license](https://opensource.org/license/BSD-3-clause) to a combination of the [Server Side Public License (SSPL)](https://en.wikipedia.org/wiki/Server_Side_Public_License) first introduced by MongoDB, plus a rev of its own [Redis Source Available License (RSAL)](https://redis.com/legal/rsalv2-agreement/). 

![](/images/kabo-BHJs5TZ-Nt0-unsplash.jpg)

# Some history

A super-simplified narrative of the fate that has consumed many open-source vendors before Redis would go something like this:

- A vendor is running a classic Red Hat-style dual-track strategy, with an open-source "community" release and a closed-source commercial product. The value proposition for the latter is typically based on some combination of added enterprise functionality and official support contracts. 
- The open-source project is picked up by the cloud hyperscalers, who host it themselves, and contribute nothing back to the vendor acting as commercial shepherd of the project.
- The vendor's business quickly goes from being promising (*look at all this community growth that can be monetised!*) to extremely challenging (*why would anyone deal with a subscale vendor when they can get the same experience in a couple of clicks from their current cloud vendor?*). 
- Investors flee and the vendor goes into a death spiral, stabilising (in the best case) as a niche player in a community dominated by the hyperscalers.

The first push back against this state of affairs was arguably when MongoDB changed its license back in 2018, essentially as a defense against encroachment by the cloud hyperscalers. The new license that MongoDB came up with was the SSPL, which is basically the [GNU Affero General Public License (AGPL)](https://en.wikipedia.org/wiki/GNU_Affero_General_Public_License) with a single added clause. That addition was designed to act as a poison pill and prevent the hyperscalers from pulling their usual moves on MongoDB.

The SSPL’s extension to the AGPL is sometimes characterised as requiring would-be service providers to acquire a license from MongoDB (the company) in order to offer MongoDB (the software) as a service. As written, it actually requires any entity hosting the software covered by the license as a managed service to also release under the SSPL any subsidiary software used to operate that service:

> …including without limitation all management software, user interfaces, application program interfaces, automation software, monitoring software, backup software, storage software and hosting software

This clause would effectively require service providers to give away their entire management stack — something that they have been signally unenthusiastic about doing. Instead, the hyperscalers came up with alternative approaches, as we shall see.

![](/images/patrick-tomasso-Oaqk7qqNh_c-unsplash.jpg)

# Reactions

At the time, MongoDB’s relicensing made quite a splash. MongoDB did submit the SSPL for approval as an official open-source license by the Open Source Initiative (OSI), but this approval was not granted and MongoDB eventually withdrew the SSPL from consideration. The rejection was generally assumed to relate to clauses 6 and 9 of [The Open Source Definition](https://opensource.org/osd):

> ### 6. No Discrimination Against Fields of Endeavor
> 
> The license must not restrict anyone from making use of the program in a specific field of endeavor. For example, it may not restrict the program from being used in a business, or from being used for genetic research.

> ### 9. License Must Not Restrict Other Software
> 
> The license must not place restrictions on other software that is distributed along with the licensed software. For example, the license must not insist that all other programs distributed on the same medium must be open source software.

Pleas that the SSPL did not meaningfully restrict *use* of the software, only its *commercialisation as a service*, fell on deaf ears. My own opinion is that the SSPL respects the *spirit* of open-source far more than the clear-cutting approach taken by the hyperscalers, but it’s arguably true that SSPL does effectively “discriminate against fields of endeavor” and therefore falls foul of the *letter* of Clause 6 at least.

The OSI’s objection was moot, however: MongoDB withdrew the SSPL from consideration as an “open-source” license, and has always been very careful to describe its Community edition punctiliously as “source-available”. The most important result had been achieved: MongoDB's nascent Atlas business was now protected from erosion by service providers.

The hyperscalers, unable to offer a native MongoDB service of their own due to the strictures of the SSPL, pivoted to offering their own home-grown implementations of the MongoDB API on top of different data platforms. At the time, my Market Intelligence team at MongoDB and I lampooned these efforts, even going as far as putting up a site with the self-explanatory URL [https://isdocumentdbreallymongodb.com](https://www.isdocumentdbreallymongodb.com)[^1] (also fully compliant with [Betteridge's Law](https://en.wikipedia.org/wiki/Betteridge's_law_of_headlines)). I was later told that our little prank site had actually got as far as Andy Jassy, and he was not amused!

![](/images/absolutvision-uCMKx2H1Y38-unsplash.jpg)

# Hindsight

I think it is fair to say that subsequent events have more than justified MongoDB’s actions. The best proof of the validity of MongoDB’s position is other vendors following suit by licensing their own offerings under the SSPL. 

The most notable vendor to do so was Elastic, in 2021, finally prompting the OSI to [opine officially](https://opensource.org/blog/the-sspl-is-not-an-open-source-license) on whether the SSPL could be considered as an open-source license or not (tl;dr: "no"). Elastic arguably left its move too late, as AWS and others were able to fork the codebase as it stood prior to the relicensing and create the [OpenSearch](https://opensearch.org) distribution, which AWS now uses to power its own services — without contributing back to Elastic, of course.[^2]

In the case of MongoDB, the timing of the relicensing was a huge factor in its success. The fully-managed MongoDB Atlas service had just launched in 2016 on AWS, and in 2017 expanded to Microsoft Azure and Google Cloud. Atlas made for a viable first-party option for MongoDB customers who wanted the platform delivered as a service, instead of having to manage it themselves — but its long-term prospects depended on MongoDB being able to persuade significant numbers of users to migrate to or adopt Atlas who had previously been running or evaluating the Community distribution of MongoDB for themselves, including on IaaS cloud compute resources. The numbers of users setting up on Atlas would be significantly reduced if there were also a way of running MongoDB as a first-party AWS service, as there is today for MySQL or PostgreSQL. 

In other words, MongoDB could not have moved much earlier, because there was no alternative to offer those customers — but could not afford to wait much longer, for fear of seeing its user base erode under it. MongoDB also continued to develop new features at breakneck speed, making it infeasible to fork the Community codebase as it stood at the time of the relicensing and move forwards.

In the [post launching what became the OpenSearch project](https://aws.amazon.com/blogs/opensource/keeping-open-source-open-open-distro-for-elasticsearch/) (notably hosted on AWS' blog), we find this claim:

> At AWS, we believe that maintainers of an open source project have a responsibility to ensure that the primary open source distribution remains open and free of proprietary code so that the community can build on the project freely, and the distribution does not advantage any one company over another. This was part of the promise the maintainer made when they gained developers’ trust to adopt the software.

It is worth pointing out once again that there is only one, singular restriction in the SSPL over the open-source AGPL: not offering the software as a service. My home network devices, for instance, come with a management stack that includes MongoDB Community. **Nothing in the SSPL prevented the vendor from offering this capability.** The only thing companies are prevented from doing is to offer MongoDB services themselves — but they absolutely can build their own services on top of the MongoDB Community edition, and even offer them via the cloud, all without any licensing restrictions or even any payment changing hands.

And now we have Redis’ move, of course. Time will tell whether the results of this relicensing will be more like MongoDB or more like Elastic. Some early reactions are happening already, notably the emergence of [Valkey](https://valkey.io/). Here is how Valkey describes itself: 

> This project was forked from the open source Redis project right before the transition to their new source available licenses.

[Valkey was launched by the Linux Foundation](https://www.linuxfoundation.org/press/linux-foundation-launches-open-source-valkey-community), but is backed by "Amazon Web Services (AWS), Google Cloud, Oracle, Ericsson, and Snap Inc.". The principal contributor to the project, with 185 [commits](https://github.com/valkey-io/valkey/graphs/contributors) as opposed to 22 for the next most prolific as of writing, is [Madelyn Olson](https://www.linkedin.com/in/madelyn-olson-6a5053b6/) — who works at AWS. 

I wouldn't want to imply that this is some sort of false-flag operation: Madelyn Olson was previously a Redis maintainer, and there is a lot of [messy history](https://lwn.net/SubscriberLink/966631/6bf2063136effa1e/) around the governance of the Redis project. An important difference to e.g. MongoDB is that there have been very meaningful external contributions to Redis — something that cannot be said of MongoDB Community, which is predominantly developed in-house by MongoDB employees. Therefore, Redis is arguably trying to alter the terms under which those outside programmers made their contributions, without giving them any way to opt out. And of course, the fact that a long-term core maintainer of the project was also a paid AWS employee does give AWS some stake in the future of the project.

This situation is not quite as simple as that, though. What I wrote above might give the impression that AWS and MongoDB are bitter rivals. In fact, [AWS and MongoDB are great partners](https://aws.amazon.com/partners/mongodb/) (despite occasional irritants, mainly caused by the existence of DocumentDB[^3]). Why? Because Atlas drives enormous consumption of AWS compute resources! As long as AWS consumption is going up, AWS is quite happy to support MongoDB Atlas.

Again, though, we come back to timing. MongoDB was able to establish these facts on the ground which now determine the relationship. AWS learned from that situation, and has not given Elastic or Redis the time to dig such an impregnable moat, reinforced by both technology and business strategy. It remains to be seen how Redis' situation plays out. One interesting aspect will be [Redis' acquisition of Speedb](https://www.speedb.io), which adds NVMe storage as a cheaper alternative to Redis' previous approach that focused on its in-memory architecture.

![](/images/pablo-garcia-saldana-lPQIndZz8Mo-unsplash.jpg)

# Thinking long-term

The issue for the OSI and the open-source insiders generally is that, with every  vendor that switches license to one that is source-available (but not technically "open source"), the OSI loses a little more credibility. Redis is just the latest to make the move, but it won’t be the last.

The real problem for the OSI is that customers simply don't care. In 2018, getting dropped from the Red Hat and Debian distributions was a blow to MongoDB — a survivable one, as it turned out, but a hit nonetheless. In 2024, Redis CEO Rowan Trollope "briefed quite a few customers about this change and encountered zero controversy." 

I might even go further and say that customers care more about the long-term viability of their chosen DBMS vendor than the OSS-endorsed purity of their licensing. If I were choosing a DBMS vendor to partner with — not for a personal hobby project, but for a long-term run-the-company platform — I would absolutely be asking questions about the structure of the business and how it was set up to make sure that vendor would be  developing its product actively for at least 3-5 years. If a vendor did not have control of its own market, that would be a red flag for me. 

There are other options, but none that are good for vendors. When Datastax, the commercial shepherd of the Apache Cassandra project, fell out with the community, the result was a sucking chest wound in that community that was left untreated for the best part of two years, and significantly reduced its position in the market.

Meanwhile, the PostgreSQL community operates basically entirely independently of EDB, leaving that vendor well below the scale of other DBMS vendors that have more control of their ecosystems. This is fine for *users* — PostgreSQL isn’t going anywhere — but it means that *companies* gravitate, once again, to the hyperscalers and their (admittedly very competent) PostgreSQL-based offerings.

This sort of monoculture seems far more antithetical to the spirit of open-source than any stricture imposed by the SSPL. 


[^1]: There is also a companion site at [https://iscosmosdbreallymongodb.com/](https://www.iscosmosdbreallymongodb.com/), lest anyone think we were playing favourites. Google is the odd one out of the Big Three here, not having launched its own MongoDB clone, but their DBMS efforts seem anyway to be focused more on the OLAP side rather than on OLTP.

[^2]: Elastic has pivoted from being a pure-play DBMS vendor and into the security space, a move which seems to be going well, judging by [user reviews](https://www.gartner.com/reviews/market/security-information-event-management/vendor/elasticsearch/product/elastic-security), and which is less subject to encroachment by the hyperscalers — at least for the time being.

[^3]: My personal opinion is that AWS would be better off just dropping DocumentDB. It is quite evidently the least-loved of their many (so many) DBMS offerings, either left off the slide entirely, or jostling for position in twelve-point font at the back of the family picture. I can't imagine it is making meaningful revenue contributions — but it does have fixed costs to develop, as well as constituting an ongoing irritant to an important partnership. Because of the feature lag, I would estimate with a high level of confidence that no significant rework would be required to migrate a running app from DocumentDB to MongoDB. AWS should just endorse Atlas (on AWS) as its document database solution, and move on, washing down that bitter pill with all of the revenue from the increased compute usage coming from those new Atlas users — revenue that would have much better profit margins, once the need to fund development of DocumentDB is removed. But hey, just my opinion.


***


🖼️  Photos by [Kabo](http://www.kabo.co/), [Patrick Tomasso](http://youtube.com/impatrickt), [Pablo García Saldaña](https://www.garciasaldana.com/) and [AbsolutVision](https://www.alterego.swiss/) on [Unsplash](https://www.unsplash.com)