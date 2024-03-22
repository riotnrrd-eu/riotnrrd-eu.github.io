---
layout: post
title:  Amazon's Private Cloud 
date:   2018-12-04 
categories:  cloud amazon AWS 
---

# Amazon's Private Cloud


Last week was [AWS re:Invent](https://reinvent.awsevents.com/), and I’m still dealing with the email hangover.[^1] AWS always announce [a thousand and one new offerings and services](https://aws.amazon.com/new/reinvent/) at their show, and this year was no exception. However, there is one announcement that I wanted to reflect upon briefly, out of however many there were during the week.

![|2048x0](/images/IMG_0083.JPG)

[AWS Outposts](https://aws.amazon.com/outposts/) are billed as letting users “Run AWS infrastructure on-premises for a truly consistent hybrid experience”. This of course provoked a certain amount of hilarity in the parts of Twitter that have been earnestly debating the existence of hybrid cloud since the term was first coined.

[twitter url=“https://twitter.com/jamestomkins/status/1068252682404515840?s=21]

On the surface, it might indeed seem somewhat strange for AWS, the archetypal public cloud in most people’s minds, to start offering hardware to be deployed on customers’ premises. However, to me it makes perfect sense.

*Pace* some ten-year-old marketing slogans which have not aged well, most companies do not start out with a hybrid cloud strategy. Instead, they find themselves forced by circumstances to formulate one in order to deal with all of the various departments that are out there doing their own thing. In this situation, the hybrid cloud strategy is simply recognition that different teams have different requirements and have made their own decisions based on those. All that corporate IT can do is try to gain overall visibility and attempt to ensure that all the various flavours of compute infrastructure are at least being used in ways which are sane, secure, and fiscally responsible (the order of the priorities may change, but that’s the list).

Some of the more wild-eyed predictions around hybrid cloud instead expected that workloads would be easily moved, not only between on- and off-premises compute infrastructure, but even between different cloud providers. In fact, it would be so easy that it would be possible to make minute-by-minute assessments of the cost of running workloads with different providers, and move them from one to another in order to take advantage of lower prices.

Obviously, that did not happen.

For the cloud broker model to work, several laws of both economics and physics would have to be suspended or circumvented, and nobody seems to have made the requisite breakthroughs.

To take just a few of the more obvious objections:

## The Speed Of Light

Moving any meaningful amount of data around the public internet still takes time. If you are used to your local 100 Gb-E LAN, it can be easy to forget this, but it is going to be a factor out there in the wild wild Web. This objection was obvious when we were talking about moving monolithic VMs around, but even if you assume truly immutable infrastructure, you are still going to have to shift at least some snapshot of the application state, and that adds up fast – let alone the rate of configuration drift of your “immutable” infrastructure with each new micro-release.

## Transparent Pricing

The units of measure of different cloud providers are not easily comparable. How does the performance of an AWS M5 instance compare to an Azure Dv2-series? Well, you’d better know before you move production over there… And AWS has 24 [instance types](https://aws.amazon.com/ec2/instance-types/), whereas Azure has 7 different [series](https://docs.microsoft.com/en-us/azure/virtual-machines/windows/sizes-general), each with sub-types and options – and let’s not even talk about all the weird and wonderful single-use configurations in your local VMware or Openstack service catalogue! How portable *is* your workload, really?

## Leaving Money On The Table

Or let’s take it from the other side: assume you have carefully architected your thing to use only minimum-common-denominator components that are, if not identical, at least similar *enough* across all of the various substrates they might find themselves running on. By definition, this means that you are not taking full advantage of the more advanced capabilities of each of those platforms. This limitation is not only at the ingredient level; you also have to make worst-case assumptions about the sorts of network bandwidth and latency you might have access to, or the sort of regulatory and policy compliance environment that you might find yourself operating within.

For all of these reasons and more, the dream of real-time cloud pricing arbitrage died a quick death, regardless of whether individual companies might use different cloud providers in various parts of their business.

Amazon Outposts is not that. For a start, despite running physically on the customer’s premises, it is driven entirely from the (remote) AWS control plane. Instead, it has the potential to address concerns about physical location together with associated concerns about latency and legal jurisdiction. Being AWS (with some help from VMware) it avoids the concern about different units of measure. For now, it only goes part of the way to resolving the final question about minimum common denominator ingredients, since at launch it only supports EC2. Additional features are expected shortly, however, especially including various storage options.

So yes, hybrid cloud. Turns out, it’s not only still a thing, but you can even get it from AWS. Who’d have thunk it?

[^1]: I managed to avoid any hangovers of the alcoholic variety; staying well hydrated in Las Vegas is good for multiple purposes. My inbox, however, is a *mess*.

