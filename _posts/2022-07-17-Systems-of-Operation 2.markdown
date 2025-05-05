---
layout: post
title:  Systems of Operation 
date:   2022-07-17 
categories:  devops 
---

# Systems of Operation


I have, to misquote J. R. R. Tolkien, a [cordial dislike](https://askmiddlearth.tumblr.com/post/93871332606/tolkien-wrote-i-cordially-dislike-allegory-cordial) of overly rigid classification systems. The fewer the dimensions, the worse they tend to be. The classic two-by-two grid, so beloved of management consultants, is a frequent offender. I suspect I am not alone, as most such systems quickly get complicated by the addition of precise placement along each axis, devolving into far more granular coordinate systems on at least one plane, rather than the original four simple boxes. But surely the worst of the lot are simple binary choices, this or that, no gradations on the spectrum allowed.

We have perhaps more than our fair share of these divisions in tech — or perhaps it makes sense that we have more than other fields? (That's a joke, because binary) *Anyway*, one of the recurring binary splits is the one between development and operations. That it is obviously a false binary is clear by the fact that these days, the grey area at the intersection — DevOps — gets far more consideration than either extreme. And yet, as it is with metaphors and allegories (back to JRRT!), so it is with classifications: all of them are wrong, but some of them are *useful*.

The Dev/Ops dichotomy is a real one, no matter how blurred the intersection has got, because it is based in a larger division. People tend to prefer either the work of *creation*, architecting and building, or the work of *maintaining*, running and repairing. The first group get visibility and recognition, so certain personality traits cluster at this end of the spectrum — flashy and extrovert, dismissive of existing constraints. At the opposite end, we find people who value understanding a situation deeply, including how it came to be a certain way, and who act within it to achieve their goals.

![](/images/181305.jpeg)

I am trying to avoid value judgments, but I think it is already clear where my own sympathies lie. Someone I have worked with for a long time subscribes to [Isaiah Berlin's analogy](https://en.wikipedia.org/wiki/The_Hedgehog_and_the_Fox): the fox knows many things, but the hedgehog knows one big thing. I am an unashamed fox: I know a little about a lot, I love accumulating knowledge even if I do not have an immediate obvious use for it, and I never saw a classification system I did not immediately question and find the corner-cases of. These traits set me up to be a maintainer and an extender rather than a creator.

I value the work of maintenance; designing a new thing starting with a clean sheet is an indulgence, while working within the constraints of an existing situation and past choices to reach my objectives is a discipline that requires understanding both of my own goals and those of others who have worked on the same thing in the past. In particular, good maintainers extend their predecessors the grace of assuming good intent. Even if a particular choice seems counter-intuitive or sub-optimal, this attitude does the courtesy of assuming there was a good and valid reason for making it, or a constraint which prevented the more obvious choice.

# # Embrace Failure — But Not Too Tightly

There are many consequences to this attitude. One is embracing failure as an opportunity for learning. The best way to learn how something works is often to break it and then fix it — but please don't blame me if you break prod! Putting something back together is the best way to truly understand how different components fit one another and interact with one another in ways that may or may not be planned in the original design. It is also often a way of finding unexpected capabilities and new ways of assembling the same bits into something new. I did both back when I was a sysadmin — broke prod (only the once) and learned from fixing things that were broken.

Embracing failure also does not mean that we should allow it to happen; in fact the maintainer mindset assumes failure and values redundancy over efficiency or elegance of design. Healthy systems are redundant, both to tolerate failure and to enable maintenance. I had a car with a known failure mode, but unfortunately the fix was an engine-out job, making preventative maintenance uneconomical. The efficiency of the design choice to use plastic tubing and route it in a hot spot under the engine ultimately came back to bite me in the shape of a late-night call to roadside assistance and an eye-watering bill.

# # Hyperobjects In Time

There is one negative aspect to the maintainer mindset, beyond the lack of personal recognition; people get awards for the initial design, not for keeping it operating afterwards. Lack of maintenance (or of the right sort of maintenance) is not immediately obvious, especially to hedgehog types. It is not the sort of one big thing that they tend to focus on. Instead, it is more of a hyperobject, visible only if you take a step back and add a time dimension. Don't clean the kitchen floor for a day, it's probably fine. Leave it for a week, it's nasty, and probably attracting pests. I know this from my own student days, when my flatmates explored the boundaries of entropy with enthusiasm.

Hyperobjects extend through additional dimensions beyond the usual three. In the same way that a cube is a three-dimensional object whose faces are two-dimensional squares, a hypercube or tesseract is a four-dimensional object whose faces are all three-dimensional cubes. This sort of thing can give you a headache to think about, but does make for cool screensaver visualisations. In this particular formulation, the fourth dimension is time; deferred maintenance is visible only by looking at its extent in time, while its projection into our everyday dimensions seems small and inconsequential when viewed in isolation.

These sorts of hyperobjects are difficult for hedgehogs to reason about precisely because they do not fit neatly into their two-by-two grids and one big thing. They can even sneak up on foxes because there is always something else going on, so the issues can remain undetected, hidden by other things, until some sort of failure mode is encountered. If that failure can be averted or at least minimised, maintainer foxes can learn something from it and modify the system so that it can be maintained more easily and avoid the failure recurring.

All of these reflections are grounded in my day job. I own a large and expanding library of content, which is continuously aging and becoming obsolete, and must be constantly maintained to remain useful. Leave one document untouched for a month or so, and it's probably fine; the drift is minimal, a note here or there. Leave it for a year, and it's basically as much work to bring it back up to date as it would be to rewrite it entirely. It's easy to forget this factor in the constant rush of everyday work, so it's important to have systems to remind us of the true extent of problems left unaddressed.

![](/images/181729.jpeg)

In my case, all of this rapidly-obsolescing content is research about competitors. This is also where the intellectual honesty comes in: it's important to recognise that creators of competing technology may have had good reasons for making the choices they made, even when they result in trade-offs that seem obviously worse. In the same way, someone who adopted a different technology probably did so for reasons that were good and valid for their time and place, and dismissing those reasons as irrelevant will not help to persuade them to consider a change. This is known as "calling someone's baby ugly", and tends to provoke similar negative emotional reactions as insulting someone’s actual offspring.

Good competitive positioning is not about pitching the One True Way and explaining all the ways in which other approaches are Wrong. Instead, it's about trying to understand what the ultimate goal is or was for all of the other participants in the conversation, and engaging with those goals honestly. Of course I have an agenda, I'm not just going to surrender because someone made a choice years ago — but I can put my agenda into effect more easily by understanding how it fits with someone else's agenda, by working with the existing complicated system as it is, rather than trying to raze it to the ground and start again to build a more perfect design, whatever the people who rely on the existing system might think.

I value the work of maintainers, the people who keep the lights on, at least as much as that of the initial designers. And I know that every maintainer is also a little bit of a designer, in the same way that every good designer is also thinking at least a little bit about maintenance. Maybe that is my One Big Thing?

                              