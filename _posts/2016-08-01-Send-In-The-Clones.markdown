---
layout: post
title:  Send In The Clones 
date:   2016-08-01 
categories:  Apple MacOS iOS 
---

# Send In The Clones


Since my [last post]({% post_url 2016-07-11-That-Old-Enterprise-Software-Business %}) rehashing ancient IT industry history seemed to go over well, here’s another one.

In that previous post, I used the story of the HP acquisition of Mercury and its rumoured impending spin-off as a cautionary tale about handling acquisitions correctly. There is never any lack of “fantasy M&A” going on in this industry, but one of the longest-running figures is Apple.

I’ve actually been a Mac user long enough that I can remember when the rumour of the week would be, not about whom Apple should buy, but about *who was going to buy Apple*. Would it be Dell? Would it be Sony? Would it be Silicon Graphics? Would it be Sun? Would it be IBM?

Twenty years later, that catalogue is ridiculous on the face of it. Only one of those companies even still meets the two core criteria, namely a) existence, and b) being a PC manufacturer. However, in the mid-90s, things were not at all rosy at Apple, and management was getting desperate. How desperate? They approved a programme that licensed the MacOS to other manufacturers, who could then make and sell their own fully-legal and -compatible MacOS computers.

As it happened, I had a front-row seat for all of this. In the mid-90s I was still in high school, but given that in Italy high school is a morning-only affair, I took on an afternoon job at the local Apple reseller. Unbeknownst to me, they had also just signed up to be the Italian reseller for [UMAX](https://en.wikipedia.org/wiki/UMAX_Technologies), one of those MacOS clone makers (also known as SuperMac in the US).

![](/images/unknown_filename.304.jpeg)

UMAX had already been around for a while, and had made a name for themselves with a range of scanners that went from consumer-grade to very definitely pro-grade. The most expensive machine I dealt with was a $25k A3 flat-bed scanner with 9600 dpi optical resolution. Photographers and other graphic artists from all over Italy were already dealing with this company, so the value proposition of a cheaper Mac for their work was pretty obvious.

Where things got exciting was when performance of the UMAX machines started to overtake that of contemporary Macs. This was in the days of the Motorola/IBM [PowerPC](https://en.wikipedia.org/wiki/PowerPC) CPU, and Mac performance was already starting to suffer compared to contemporary Intel chips. Therefore, when UMAX brought to market a dual-604e motherboard, available with not one but *two* screaming-fast 200 MHz CPUs, this was big news - not least because they not only undercut the price of the equivalent [PowerMac 9600](https://en.wikipedia.org/wiki/Power_Macintosh_9600), but beat it to market as well.

(Embarrassingly, I blew up the very first one of those machines to come to Italy. It had a power supply with a physical switch to change from 115v US-style power to the full-strength 230v juice we enjoy in Europe. I did check the switch before plugging in the cable, but **BANG**! Turned out, the switch was not properly connected on the inside of the PSU… Luckily, all that had blown was the power supply itself, not the irreplaceable motherboard, and we got it swapped out in double-quick time and nobody ever found out… until now.)

Anyway, this was all great fun for me, still in high school and all, and everyone was doing very well out of the arrangement - except for Apple. The licensing fee for MacOS that they were receiving did not even come close to replacing the profit they missed out on from all the lost sales of Apple hardware[^1]. As soon as Steve Jobs returned to Apple, he killed the programme. UMAX was the last of the cloners to fall, managing to secure the only license to ship MacOS 8 (everyone else’s licenses ended with System 7[^2]), but the writing was on the wall. UMAX switched to making Wintel PCs - a market they since exited, reverting to their core strength of imaging products.

![](/images/unknown_filename.305.jpeg)

Today, a handful of dedicated people still build “hackintosh” computers from commodity parts, and then try to force OS X[^3] to run on them, with varying degrees of success. However, there is no officially sanctioned way of running OS X on any hardware not sold by Apple.

***

So, given this history and the results for Apple, why exactly do people feel the need to advise Apple to license iOS? Both [the Macalope](http://www.macworld.com/article/3102167/ios/seeing-double-twice-the-advice-twice-the-wrong.html) and [Nick Heer of Pixel Envy](http://pxlnv.com/linklog/wadhwa-licensing/) have already done the hard work of eviscerating this wrong-headedness, but I couldn’t resist getting my own blow in.

First of all, iOS runs on its own system-on-a-chip (SoC) - currently, the A9 and A9X. Sure, this is based on the industry-standard ARMv8 architecture, but with substantial refinements added by Apple, which they would presumably be even more reluctant to license than iOS itself.

So let’s say Samsung or whoever either licenses the SoC design, or builds their own (not a trivial exercise in itself), install iOS, and sell the resulting device as the iGalaxy. Where are they going to position this frankenphone? It can’t be priced above Apple’s own offerings unless it brings something novel to the table.

What could that be? Maybe some device that spans the gap between Android and iOS? Well, here too, history can be our guide.

Back in my UMAX days, we did sell one very popular accessory. Basically it was a full-length PCI card with an entire x86 chipset and its own Intel CPU on it. Seriously, this thing was the biggest expansion board I have ever seen - the full width of the motherboard, so wide that it had a special support bracket in the case to prevent it sagging under its own weight. It also had its own CPU fan, of course, so it took up a fair amount of vertical space too. This allowed owners to run Windows on Intel side by side with MacOS on PowerPC, sharing a graphics card and input devices. Mind-blowing stuff in the mid-Nineties!

So in that vein, could a cloner conceivably sell a handset that could run Android apps natively side-by-side with iOS ones? Frankly, I doubt it. These days, it’s easier to emulate another platform, or just carry two phones. Maybe a few developers would be interested, but the market would be tiny.

It used to be the case that if you wanted a large phone (I refuse to call it a “phablet”) you had to go with Android, because iPhones came in one size only. These days, Apple sells phones in a variety of sizes, from the small iPhone SE, through the standard iPhone, up to the iPhone Plus - so I can’t see the form factor being enough of a draw for people to go with a third-party device.

![](/images/unknown_filename.306.jpeg)

The only variable that’s left is price. Any iOS clone manufacturer would have to substantially undercut Apple’s cheapest devices to get sales. To do this, they would cut corners. By giving the device less RAM, or a non-Retina display, or less storage, or whatever, the cloners could lower the price point enough to get the initial sale - but Apple would be stuck with the horrible customer satisfaction issues from running on this below-par hardware.

That last point is particularly problematic because Apple’s entire business model is predicated upon taking, not the *whole* of the smartphone market, but the most profitable slice of it. One important consequence of this is that iOS is also the most profitable market for developers, because iOS users by definition have money to spend on apps. This is a virtuous circle for Apple, as the richer app ecosystem draws more users, which draws more development, and so on.[^4]

If users - many of them first-time users, who are tempted into trying iOS by new low-cost clone devices - have a terrible experience, never buy apps, and replace their iOS device with an Android one as soon as they get the chance, that virtuous cycle turns vicious fast.

And that’s not even getting into the strategy tax Apple would be paying on other decisions. To cite another rumour that’s doing the rounds, could Apple drop the headphone jack from their own devices if there were cloners still manufacturing iOS devices that featured it? Maybe they could - but the decision would be much more fraught.

Bottom line, there is no iOS license fee that the cloners would pay that would also compensate Apple for both lost sales of their own hardware and for the wider market impact.

Apple tried this once, and it nearly killed them.

Can we *please* stop bringing up this idiotic idea now?[^5]

[^1]: For more context from 1997, see [here](https://archive.org/stream/MacWorld_9711_November_1997/MacWorld_9711_November_1997_djvu.txt) and search for “Why Apple Pulled the Plug”.

[^2]: What, you thought confusing name changes to Apple’s operating systems were a new thing? Hah.

[^3]: See what I mean? Are we supposed to call it macOS already, or is it still OS X for now? So confused.

[^4]: And of course Apple takes its cut from the App Store, too.

[^5]: Of course not: when it comes to Apple, we’re always [fighting the same battles]({% post_url 2013-01-15-Platform-wars-are-here-again %}).

                      