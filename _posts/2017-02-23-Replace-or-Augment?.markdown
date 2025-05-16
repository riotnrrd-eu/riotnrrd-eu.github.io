---
layout: post
title:  Replace or Augment? 
date:   2017-02-23 
categories:  automation work enterprise 
---

One of the topics that currently exercise the more forward-looking among us is the potential negative impact of automation on the jobs market and the future of work in general. Comparisons are frequently made with the Industrial Age and its consequent widespread social disruption - including violent reactions, most famously the [Luddite](https://en.m.wikipedia.org/wiki/Luddite) and [*saboteur*](https://en.wikipedia.org/wiki/Sabotage#Etymology) movements.

![](/images/unknown_filename.291.png)

Some cynics have pointed out that there was less concern when it was only blue-collar jobs that were being displaced, and that what made the chattering classes sit up and pay attention was the prospect of the disruption coming for their jobs too. I could not possibly comment on this view - but I can comment on what I have seen in years of selling automation software into large companies.

For more than a decade, I have been involved in pitching software that promised to automate manual tasks. My customers have always been large enterprises, usually the Global 2000 or their immediate followers. Companies like this do not buy software on a whim; rather, they build out extensive business cases and validate their assumptions in detail before committing themselves[^1]. There are generally three different ways of building a business case for this kind of software:

*  Support a growth in demand without increasing staff levels (as much);
*  Support static demand with decreasing staff;
*  Quality improvement (along various different axes) and its mirror image, risk avoidance.

The first one is pretty self-evident - if you need to do more than you can manage with the existing team, you need to hire more people, and that costs money. There are some interesting second-order consequences, though. Depending on the specifics of the job to be done, it will take a certain amount of time to identify a new hire and train them up to be productive. Six months is a sensible rule of thumb, but I know of places where it takes years. If the rate of growth gets fast enough, that lag time starts to be a major issue. You can't just hire yourself out of the hole, even with endless money. The hole may also be getting deeper if other companies in the same industry and/or region are all going through the same transformation at the same time, and all competing for the same talent.

If instead you can adopt tooling that will make your existing people more efficient and let you keep up with demand, then it is worth investing some resources in doing so.

That second business case is the nasty one. In this scenario, the software will pay for itself by automating people's jobs, thus enabling the company to fire people - or in corporate talk, "reduce FTE[^2] count". The fear of this sort of initiative is what makes rank and file employees often reflexively suspicious of new automation tools - over and above their natural suspicion that a vendor might be pitching snake-oil.

Personally I try not to build business cases around taking away people's jobs, mainly because I like being able to look myself in the mirror in the mornings (it's hard to shave any other way, for one thing). There is also a more pragmatic reason not to build a business case this way, though, and I think it is worth exploring for its wider implications.

![](/images/unknown_filename.292.png)

## Where Are The Results?

The thing is, in my experience business cases for automation built around FTE reduction have never been delivered successfully - if focused on automation of existing tasks. That is an important caveat, but I will come back to that.

Sure, the business case might look very persuasive - "we execute this task roughly a dozen times a day, it takes half an hour each time, and if you add that up, it's the equivalent of a full-time employee (an FTE), so we can fire one person". When you look at the details, though, it's not quite so simple.

The fact is that people rarely work at discrete tasks. Instead, they spend their time on a variety of different tasks, more or less integrated into a whole process. There is a tension between the two extremes: at the one end you have workers on a repetitive assembly line, while at the other you have people jumping around so much they can never get anything done. Most organisational functions are somewhere in between those two poles.

If automation is focused on addressing those discrete tasks, it absolutely will bring benefits, but those benefits will add up to freeing up existing employees to catch up with other tasks that were being neglected. Every IT department I have ever seen has a long tail of to-dos that keep getting pushed down the stack by higher-priority items. Automation is the force multiplier that promises to let IT catch up with its to-do list.

This sort of benefit is highly tactical, and is generally the domain of point solutions that do one thing and do it well. This will enable the first kind of business case, delivering on new requirements faster. It will not deliver the second kind of business case. The FTEs freed up through automation get redeployed, not fired, and while the organisation is receiving benefit from that, it is not what was built into the assumptions of the project, which will cause problems for its sponsors. Simply put, if someone ever checks the return on the investment (an all too rare occurrence in my experience), the expected savings will not be there.

Strategic benefits of automation, on the other hand, are delivered by bundling many of these discrete tactical tasks together into a new whole.

Realising those strategic benefits is not as straightforward as dropping a new tool into an existing process. Actually achieving the projected returns will require wholesale transformation of the process itself. This is not the sort of project that can be completed in a quarter or two (although earlier milestones should already show improvement). It should also not be confused with a technology implementation project. Rather, it is a *business transformation* project, and must be approached as such.

Where does this leave us?

![](/images/unknown_filename.293.png)

## Go Away Or I Will Replace You With A Very Small Shell Script

In my experience in the field, while tactical benefits of automation are achievable, true strategic improvement through automation can only be delivered by bundling together disparate technical tasks into a new whole. The result is that it is not skilled workers that are replaced, but rather the sorts of undifferentiated discrete tasks that many if not most large enterprises have already outsourced.

This shows who the losers of automation will be: it is the arbitrageurs and rent-seekers, the body-rental shops who provide no added value beyond cheap labour costs. The jobs that are replaced are those of operators, what used to be known as *tape jockeys*; people who perform repetitive tasks over and over.

The jobs that will survive and even benefit from the wave of automation are those that require interaction with other humans in order to determine how to direct the automation, plus of course the specialists required to operate the automation tools themselves. The greatest value, however, will accrue to those who can successfully navigate the interface between the two worlds. This is why it is so important to [own those interfaces]({% post_url 2017-02-14-Own-Your-Interfaces %}).

What might change is the nature of the employment contracts for those new roles. While larger organisations will continue to retain in-house skills, smaller organisations for which such capabilities are not core requirements may prefer to bring them in on a consultative basis. This will mean that many specialists will need to string together sequences of temporary contracts to replace long-duration full-time employment.

This is its own scary scenario, of course. The so-called *gig economy* has not been a win so far, despite its much-trumpeted potential. Perhaps the missing part to making this model work is some sort of universal basic income to provide a base and a safety net between consulting jobs? As more and more of the economy moves in this direction, at least in part due to the potential of automation, UBI or something similar will be required to bridge the gap between the assumptions of the old economy and the harsh realities of the new one.

So, the robots are not going to take our jobs - but they are going to change them, in some cases into something unrecognisable. The best thing humans can do is to [plan to take care of one other](https://www.goodreads.com/quotes/1889-hello-babies-welcome-to-earth-it-s-hot-in-the-summer).

***
Images by [Annie Spratt](http://mammasaurus.co.uk), [Janko Ferlic](https://unsplash.com/@thepootphotographer), and [Jayphen Simpson](http://jayphen.com) via [Unsplash](https://unsplash.com)

[^1]: Well, in theory. Sometimes you lose a deal because the other vendor's CEO took your prospect's entire management team for a golfing weekend in the corporate jet. But we don't talk about that.
[^2]: An FTE is a Full-Time Equivalent: the amount of work expected of one employee, typically over a year, allowing for holidays and so on. Typically that means somewhere between 200 and 220 working days of 8 hours each, so 1600 to 1760 hours in a year. The "FTE cost" of an activity is calculated by taking the time required to perform an activity once, multiplying that by the number of times that activity needs to be performed, and dividing by the FTE rate.