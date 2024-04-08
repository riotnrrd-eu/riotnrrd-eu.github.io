---
layout: post
title:  The Internet of (Insecure) Things 
date:   2017-10-16 
categories:  security IoT 
---

![](/images/unknown_filename.355.jpeg)

Back in 2014, I wrote an article entitled [Why the Blinking Twelves is an Internet of Things problem in the making](http://www.cloudcomputingintelligence.com/comment-blog/item/1696-why-the-blinking-twelves-is-an-internet-of-things-problem-in-the-making). If you’re not familiar with the idiom of the "blinking twelves", allow me to enlighten you:

> Back in the last century, digital clocks with seven-segment displays became ubiquitous, including as part of other items of home electronics such as VCRs. When first plugged in, these would blink "12:00" until the time was set by the user.
>
> Technically-minded people soon noticed that when they visited less technical friends or relatives, all the appliances in the house would still be showing the "blinking twelves" instead of the correct time. The "blinking twelves" rapidly became short-hand for "civilians" not being able to – or not caring to – keep up with the demands of ubiquitous technology.
>
> One of the most frustrating things for techies about the "blinking twelves" was that nobody else seemed to care or even notice the problem that was driving them nuts. How could people not *see* the blinking twelves all around them, and do something about them?
>
> It took Windows for the problem to become obvious. Windows computers, brought a much higher level of technological complexity, the computer needed regular maintenance and people rapidly realised that updates and patches were required at regular intervals if their computers were to remain functional and secure.
>
> The problem that we are facing is that technology has already begun to spread beyond the desktop. Even the most technophobic now carry a phone that is "smart" to a greater or lesser degree and many people treat these devices much like their old VCRs, installing them once and then forgetting about them. However, all of these devices are running 24/7, connected to the public Internet, with little to no management or updates.

In the three years since I wrote that article, the number of Internet-enabled devices has simply exploded. 

![](/images/unknown_filename.356.png)

I know, it’s from [Business Insider](http://www.businessinsider.com/how-the-internet-of-things-market-will-grow-2014-10 "How the 'Internet of Things' will impact consumers, businesses, and governments in 2016 and beyond"), take it with a large grain of salt - but the trend is unarguable.

Here’s the problem: all of those Internet-enabled Things are cheap, and therefore based on existing components, including software. Most software, at least below the level of the specialised RTOSen found in nuclear power plants and the like, is built around the assumption of regular maintenance and updates provided by knowledgeable operators. However, once these Things are deployed in the field, where "in the field" often means the home or office of people who are not IT professionals, it is a given that they will not receive that level of care.

![](/images/unknown_filename.357.png)

When something like [Krack](https://arstechnica.com/information-technology/2017/10/severe-flaw-in-wpa2-protocol-leaves-wi-fi-traffic-open-to-eavesdropping/ "Severe flaw in WPA2 protocol leaves Wi-Fi traffic open to eavesdropping") hits, the odds are good that manufacturers for many devices will already have disappeared without providing patches. Even for devices from more stable vendors who do provide ongoing support, maybe the device is obsolete and replaced by newer versions with incompatible architectures. But even supposing that all the stars align and the patch is available, it will still not be deployed widely - because of the "blinking twelves" problem. Non-specialist owners will not know or care to update their devices, and so the cycle continues.

Our only hope is that we are [saved by our devices' obsolescence]({% post_url 2017-01-07-IoT-Future-Saved-by-Obsolescence %}), as the lack of updates eventually prevents them from functioning at all. Maybe this won’t be the final straw, but soon enough the figleaf in every click-through agreement about the software being "provided as is" and "no warranty of merchantability or fitness for purpose" will be ripped away, in favour of the sorts of consumer protection regulations that these same devices would be subject to if they were *not* Internet-enabled.

The alternative is that in the Smart Home of the Future that we keep being promised, troubleshooting steps really *will* require us to close all the windows, exit, and start what we were doing all over again.

Me, I’ll move to a cabin in the woods. 

***
Photo by [Heather Zabriskie](http://heatherzabriskie.com) on [Unsplash](https://unsplash.com)