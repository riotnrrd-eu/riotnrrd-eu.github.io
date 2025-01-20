---
layout: post
title: Back to the Private Cloud - Again
date: 2025-01-20
categories: cloud AWS
---

[text]({% post_url  %})

An article titled “[Is private cloud having a moment?](https://www.ciodive.com/news/private-cloud-generative-ai-hybrid-enterprise-it-strategy/737448/)” confounds expectations somewhat by *not* complying with [Betteridge’s Law](https://en.wikipedia.org/wiki/Betteridge's_law_of_headlines). 

Then again, given that the first person mentioned is Broadcom’s CEO, quoting from his speech at VMware Explore, perhaps that is not so surprising. However, the article is more than just a puff-piece for VMware, and there are some useful nuggets to be found inside, such as these two quotes:

> Folks that didn’t have discipline on-prem but went to the public cloud found that it’s far more expensive, because you don’t have the same control levers available to you.

> I’ve spoken to orgs that have redomiciled or repatriated back from the cloud to on-prem and those conversations all boil down to one line: lift and shift is way too expensive. Without the proper work of refactoring applications, the private cloud becomes very attractive.

![Rusty levers; pull one to migrate your legacy VMs to the cloud](/images/david-birozy-t8ajcHr13nU-unsplash.jpg)

I do have to recognise the author here for at least not quoting [DHH](https://world.hey.com/dhh/even-amazon-can-t-make-sense-of-serverless-or-microservices-59625580) yet again!

More seriously, I have seen exactly the same process gap prevent people from taking full advantage of the cloud model. In fact, I have even written about it right here, going back to 2014 in a post titled "[Hunting the Elusive Private Cloud]{% post_url 2014-03-24-Hunting-the-Elusive-Private-Cloud %})":

> there’s a good chance that a substantial proportion of that legacy infrastructure is under- or even entirely un-used. Some studies I’ve seen even show average utilisation below 10%! **This is where they get their elasticity**: between the _measured service_ and the _resource pooling_, they get a much better handle on what that infrastructure is currently used for.

2014, baby! On-premises infrastructure is a different animal than IaaS, let alone consuming serverless SaaS. If you try to treat one like the other, you’re going to have a bad time. 

# Don't Do The Same Things And Expect Different Results

If you just lift-and-shift your old on-prem servers and VMs to a cloud service provider, you’re almost certainly going to pay more. This is not the CSP scamming you; their unit cost of compute is certainly *lower* than your own, due to economies of scale, not to mention all the custom kit they design for themselves. It’s just that the whole model of public cloud is set up around some very different assumptions than your data centre, and if you fight those assumptions and don’t re-architect your applications to take them into account, you should not expect to get the benefits in terms of agility and cost savings that you were expecting. 

Last time this retreat-from-cloud story was going around, Adrian Cockroft (who should know) wrote an [excellent debunking](https://adrianco.medium.com/so-many-bad-takes-what-is-there-to-learn-from-the-prime-video-microservices-to-monolith-story-4bd0970423d4) of the more hysterical reactions. Re-architecting enterprise apps is expensive and time-consuming, yes, but it's also a good thing to do if there is a change in the conditions that you first developed for. There ain’t no such thing as a free lunch. 

The question is whether it’s worth it to go through that painful process in order to get the benefits of agility and, yes, cost-savings that the public cloud promises. Ultimately, only you know the answer to that question, but it is a question that you need to answer *before* starting the project, lest someone else answer it for you later.

An on-premises private cloud is a halfway house, in 2014 as in 2025. You can start building the discipline and the processes to manage public cloud resources by managing your on-premises infrastructure better. In parallel, you should also build new services directly in the public cloud where it makes sense, in order to build internal skills around that. It's not a binary choice between serverless public cloud and monolithic on-premises architecture, it's a gradient, and you need to choose where to position yourself and your various apps and services.

# My Architecture Is Not Your Architecture, But Your Architecture Is Fine

The closing sentiment of that *CIO Dive* article sums it up pretty neatly:

> the real value is in how enterprises utilize their infrastructure, regardless of its formal designation

If your infrastructure has high levels of utilisation, scales with user demand, and the costs match the benefits to company and users, then it doesn’t really matter where it’s hosted, how it's architected, or even what you call it.

![Containers being transported via legacy infrastructure](/images/david-birozy-xIzdx7-2Lbo-unsplash.jpg)

There is one interesting wrinkle, though: it can be surprisingly hard to get a good view across all of your infrastructure. This is hardly a new problem, of course: back when I was a sysadmin, there was a pretty clear dividing line between UNIX and Windows estates; they were managed with different tools by different teams, and even when it was nominally the same tool, the metrics it reported were different enough that it didn’t make sense to compare them. The mainframe of course was its own fiefdom off to one side.

Plus ça change: these days CloudWatch will give you a good view of what is going inside AWS, but it’s blind to Azure, and forget about wiring it up to your on-prem VMs. So now you need an overlay tool that can ingest metrics from all of them, except the different platforms don’t report the same or even easily comparable metrics. And transferring any meaningful amount of data in or out of the cloud, or between different public clouds, can get expensive *fast*.

Remember, we’re not running IT for its own sake: we need the infrastructure in order to offer services that someone needs enough to pay for. Technology alone won’t get us there, and once you start putting yourself in the end-user’s place, the right answer is rarely a monoculture. Even if going all-in with one provider might save the engineering and ops teams some time and effort, that may still not be the right answer if it undermines another part of the value equation.

# So, What Is The Answer? 

Sadly, I don’t have one simple answer to offer — and if somebody offers you one, check your wallet. Instead, we are going to have to work together, look at what you have and what your users need, and what tools you are going to need to wire it all together and make sure it’s working. It’s going to be a combination of processes to take better advantage of what you have already, judicious additions of new capabilities, and the right wrappers to make it all easy to consume.

The one piece of good news is that, in this science-fictional-sounding year of 2025, if you still *have* a data centre, it’s a pretty safe bet that you also have the resources to go through this exercise. And if you don’t think you do, because you’re spending all of them just keeping the lights on? Those are the situations with the biggest wins of all — and no, I am not talking about burning the data centre down for the insurance money!

***

🖼️  Photos by [David Birozy](https://unsplash.com/@ltdbjd) on [Unsplash](https://www.unsplash.com)