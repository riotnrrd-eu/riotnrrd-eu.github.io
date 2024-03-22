---
layout: post
title:  Piercing The Clouds 
date:   2019-05-03 
categories:  cloud green-IT 
---

# Piercing The Clouds


Now here’s an interesting document: ["A Measurement Study of Server Utilization in Public Clouds"](https://048744ef-a-62cb3a1a-s-sites.googlegroups.com/site/huanliu/cgc.pdf?attachauth=ANoY7cqcRXUeqYvNWSH9x3Vvm-iXkXbRKIuerfa_tUMmwJ7-iyWXebFY2tNTo7jv1qy2xUIeSOKGpqCped45Vq-mtncQTtNB1lK6BvAUCLylV_5Xzu_LWZFy5E_E7dmoEI_KAGY8ut6Y25XHE8wJx73d1LqhL-Hb3BFAAweXi63iA7GxppQkx68nNdd24pVtgCEiEs14HxMk&attredirects=1&mc_cid=36229ab033&mc_eid=bd3f162900). Okay, it’s from 2011, but otherwise seems legit. 

![](/images/unknown_filename.277.png)

Basically it’s a study of total CPU utilisation in both AWS and Azure (plus a brief reference to GoGrid, a now-defunct provider [acquired by Datapipe](https://www.forbes.com/sites/mikekavis/2015/01/20/datapipe-acquires-gogrid-as-ma-activity-heats-up/ "Datapipe Acquires GoGrid As M&A Activity Heats Up" ), who in turn were [acquired by Rackspace](https://blog.rackspace.com/rackspace-announces-agreement-acquire-datapipe "Rackspace Announces Agreement to Acquire Datapipe" )). The problem is that very few people out there are doing actual studies like this one; it’s mostly comparisons between on-prem and remote clouds, or between different cloud providers, rather than absolute utilisation. However, it’s interesting because it appears to undermine one of the biggest rationales for a move to the cloud: higher server utilisation. 

![](/images/unknown_filename.278.png)

Note that Y-axis: utilisation is **peaking at 16%**. 

The study’s conclusion is as follows:

> Apparently, the cost of a cloud VM is so low that some users choose to keep the VM on rather than having to worry about saving/restoring the state.

I wonder if this study would bring any substantially different results if repeated in 2019, with all the talk of serverless and other models that are much less dependent on maintaining state. It is plausible that in 2011 most workloads, even in public clouds, were the result of “lifting and shifting” older architectures onto new infrastructure. The interesting question would be, how many of those are still around today, and how many *production* workloads have been rearchitected to take advantage of these new approaches.

This is not just an idle question, although there is plenty of scope for snarkily comparing monolithic VMs to mainframes. Cloud computing, especially public cloud, has been able to claim the mantle of Green IT, in large part because of claims of increased utilisation – more business value per watts consumed. If that is not the case, many organisations may want to re-evaluate how they distribute their workloads. Measuring processor cycles per dollar is important and cannot be ignored, but these days the big public cloud providers are within shouting distance of one another on price, so other factors start to enter into the equation – such as environmental impacts.

***
Image by [Samuel Zeller](http://samuelzeller.ch) via [Unsplash](http://unsplash.com/)

