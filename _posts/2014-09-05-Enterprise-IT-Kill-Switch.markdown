---
layout: post
title:  Enterprise IT Kill Switch 
date:   2014-09-05 
categories:  byod shadow-IT 
---

# Enterprise IT Kill Switch


California has [passed a law](http://bits.blogs.nytimes.com/2014/08/25/california-governor-signs-law-requiring-a-kill-switch-on-smartphones/ "California Governor Signs Law Requiring a ‘Kill Switch’ on Smartphones" ) mandating kill switches for smartphones:

> A kill switch is software that allows consumers to disable a phone after the device has been reported stolen and reactivate it only with a correct password or personal identification number. Proponents of the bill have argued that wide adoption of this type of antitheft technology would lead to a reduction in phone theft because it would  make it more difficult for criminals to resell stolen phones.

This is all well and good, and if your phone has this functionality available, then you should definitely turn it on now. If stolen smartphones are known to be useless, it will not be worth thieves' while to steal them. Note that this works even if the technology is not perfect. If it turns out that the lock can be bypassed, but doing so is difficult or time-consuming, fences will demand more discount from thieves, making the phones less attractive.

But what is the connection with enterprise IT?

I would be willing to bet that many admins have wished that servers came with kill switches, for instance. Who hasn't had a mis-configured VM running on somebody's desktop hijack DHCP for an entire subnet, for instance? Yes, that one happened to me - although I had some choice words for the OS vendor that chose to make the DHCP server default to on…

Unfortunately, problem servers these days are often not directly under IT's control. This is infamously known as "shadow IT": business units frustrated with the pace or quality of service they get from IT go rogue and obtain service elsewhere. Gartner famously [predicted](http://www.gartner.com/newsroom/id/1862714 "Gartner Reveals Top Predictions for IT Organizations and Users for 2012 and Beyond" ) that 35% of IT spending would be happening outside of the IT department's view by 2015.

Depending on your own definition of shadow IT, this prediction may seem more or less realistic. For instance, does shadow IT include rogue BYOD? The same pressures drive both, but BYOD users generally want to use company services. However, nobody can deny that a non-negligible amount of shadow IT is already taking place.

The question is what to do about it.

I got into a [Twitter exchange](https://twitter.com/dwellington/status/506471050411249665) on that very topic, starting from [this blog post](http://www.itskeptic.org/content/how-deal-shadow-it "How to deal with Shadow IT" ) by the IT Skeptic, Rob England.

![](/images/tweet-506471050411249665.png)

IT departments would *love* to have a "kill switch" for shadow IT. No more rogue users going off and doing their own thing! Back to the good old days of everyone going to IT on bended knee. After all, what alternative did they have - buy their own mainframe? Yeah, right!

Well, the world has changed, and now users *do* have alternatives. The hell of the thing, from the point of view of an IT department, is that users get better quality of IT service at home than they do at work, and this has changed their expectations at work too.

When a user goes around the IT department, that is a signpost to value that is currently not being delivered by the IT department. No matter how easy it gets to do IT, users would rather someone else were doing it. It's just that the level of effort required to do it themselves has fallen below the point where the returns are sufficient to make it worth their while.

![](/images/tweet-506514662750707712.png)

Time was, only the most dedicated people would do the BYOD thing and bring a Mac or a laptop running Linux to work. Now, it's easy enough that pretty much anyone can do it[^1], and the returns are obvious. We are getting to that point with cloud services, especially SaaS.

Now, I do agree with Rob England that *distributed IT* is better than shadow IT. Distributed IT simply means IT that is engaged with the business, instead of skulking in their ivory tower ^W^W darkened basement. Where we differ is on how blame is apportioned.

To my way of thinking, shadow IT is an indictment of the IT department's failure to engage with the business. Users should not go rogue, but let us all recognise that there has been some long-term provocation going on. In fact, IT people are shooting themselves in ***both*** feet by not engaging with the business, because not only are they losing relevance as the users bypass them wherever possible, but they still get held responsible when something breaks or the company hits the front page of the news for all the wrong reasons.

If you are in IT, **talk to your users**, figure out where there are bottlenecks, and help remove them. This is no longer a "my way or the highway" world; users have any number of roads, pathways, railways, navigable rivers, gyrocopters and teleporters to get to where they need to go. You need to prove your value, not just assume that users have no choice.

The good thing is that the rewards are also significant. IT can be a *differentiator*, not just a cost center. Business processes today are entirely computerised, to the point that the performance of IT ***is*** the performance of the business in a very real sense. (If you doubt me, try visiting any office when the power is out or the network is down. I guarantee you that not much business is being transacted.) An engaged IT department - *distributed*, as Rob England puts it - can make a very visible contribution, and stop being lumped with Facilities and janitorial services.

And all you have to do is stop calling them *lusers*…

[^1]: Or bribe someone else relatively cheaply, one time only.

                                                                                                                