---
layout: post
title:  The VP of Nope 
date:   2018-05-14 
categories:  work 
---

I have a character in my head, the VP of Nope. This is pure wish-fulfilment on my part: when everyone was in the room taking an utterly wrong and bone-headed decision, I wish there had been someone present who was sufficiently senior to just say "nnnope" and move on.

![](/images/unknown_filename.438.jpeg)

It seems I’m not the only one to feel that way, judging by the reactions to my tweet where I mentioned this:

![](/images/tweet-994264368559910912.png)

(Scoff all you want, but those are pretty big engagement numbers for me.)

The VP of Nope has to be a VP in order not to have to get bogged down in particulars. Software engineers in particular are very susceptible to getting ideas into their heads which are great in a small context, but have all sorts of problems if you take a step back and look at them again in a wider context.

Here’s an example from my own history. I used to work for a company whose products used fat clients – as in, natively compiled applications for each supported platform. This was fine at the time, but web applications were obviously the future, and so it came to pass that a project was initiated to write thin web clients instead. I was part of the early review group, and we were all horrified to find that the developers had opted to write everything in Flex. 

If you are not familiar with Adobe Flex[^1], it had a very brief heyday as a way to write rich web interfaces, but had the very significant drawback of running on top of Adobe’s late, unlamented Flash technology. There were several very significant problems due to that dependency:

- Corporate IT security policies almost *never* allowed the Flash plugin to be installed on people’s browsers. This meant that a Flex GUI was either a complete non-starter, or required exceptions to be requested and granted for every single machine that was going to connect to the application back-end, thereby losing most of the benefits of moving away from the fat client in the first place.
- Thin clients are supposed to be less resource-hungry on the client machine than fat clients (although of course they are much more dependant on network performance). While web browsers were indeed lighter-weight than many fat clients, especially Java-based ones, the Flash browser plugin was a notorious resource hog, nullifying or even reversing any energy savings.
- While Apple’s iPad was not yet nearly as dominant as it is today, when it is the only serious tablet, it was still very obvious that tablets and mobile devices in general were The Future. Every company was falling over its feet to provide some sort of tablet app, but famously, Steve Jobs hated Flash, and articulated why in his open letter, [*Thoughts on Flash*](https://www.apple.com/hotnews/thoughts-on-flash/). All of Steve’s reasons were of course *in themselves* valid and sufficient reasons not to develop anything in Flex, or indeed to require Flash in any way, but the fact that Steve Jobs was committing to never supporting Flash on Apple devices killed Flash *dead* (and there was much rejoicing). Sure, it took a couple of years for the corpse to stop twitching, but the writing was on the wall. 

Building any sort of strategic application in Flex after the release of that letter in April 2010 was a *brain-meltingly idiotic and blinkered decision* – and all of us on the early review programme said so, loudly, repeatedly, and (eventually) profanely. However, none of us had sufficient seniority to make our opinions count, and so the rough beast, its hour come round at last, slouched towards GA to be born into an uncaring world.

![](/images/unknown_filename.439.png)

# This Is Not A Rare Event

I have any number of examples like this one, where one group took a narrow view of a problem, unaware of or even wilfully ignoring the wider context. In this particular case, Engineering had determined that they could develop a thin web client more quickly and easily by using a piece of Adobe technology than by dealing with the (admittedly still immature) HTML5 tools available at the time. Given their internal metrics and constraints, this may even have been the right decision – but it resulted in an outcome that was so wrong as to actively damage the prospects of what had been until then perfectly viable products. 

In such situations, the knock-on effects of the initial fumble are often even worse than the immediate impact, and so it was to prove in this case as well. First, enormous amounts of time, energy, and goodwill were wasted arguing back and forth, and then the whole GUI had to be re-written from scratch a *second* time without Flex, once it became apparent to enough people what a disaster the first rewrite was. Meanwhile, customers were continuing to use the old fat client, which was falling further and further behind the state of the art, since all of Engineering’s effort was being expended on either rewriting the GUI yet again, or strenuously defending the most recent rewrite against its critics. All of this wasted and misdirected effort was a major contributing factor to later strategic stumbles whose far-reaching consequences are still playing out now, nearly a decade later.

This is what is referred to as an *omnishambles*, a situation that is comprehensively messed up in every possible way – and the whole thing could have been headed off before it even began by the VP of Nope, quietly clearing their throat at the back of the room and shaking their head, once.

Their salary would be very well earned.

*** 

Photo by [Vladimir Kudinov](https://unsplash.com/@madbyte) on [Unsplash](https://unsplash.com/search/photos/office?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

[^1]: Originally developed by Adobe, it now seems to be staggering through an unloved half-life as an [open-source project under the umbrella of the Apache foundation](http://flex.apache.org). *Just kill it already! Kill it with fire!*

