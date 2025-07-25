---
layout: post
title:  The Driver Behind The Curtain 
date:   2018-05-25 
categories: cars Uber 
---

Truly autonomous driving is an incredibly hard problem to solve. It would be hard enough in controlled situations, but in uncontrolled ones, where other road users may or may not be respecting the rules of the road[^1], it’s pretty close to being impossible to achieve a perfect solution. The best we can hope for is one that is better than the current state of affairs, with distracted human drivers taking an incredible toll on life.

That is the promise of self-driving cars: get the dangerous, unpredictable humans out of the loop. Getting there, however, is tough. It turns out that the [tragic death of a woman in Arizona due to a failure of an Uber experiment in autonomous driving]({% post_url 2018-03-30-When-Robots-Kill %}) may have been caused by the uncanny valley of *partial autonomy*.

![Volvo self-driving cars lined up on the street](/images/unknown_filename.354.jpeg)

Let’s take it as given that fully-autonomous (Level 5) vehicles are safer than human-driven ones. However, nobody has built one yet. What we do have are vehicles that may on occasion require human occupants to take control, and to do so with very little warning. According to the crash reports, [the Uber driver in the Arizona crash had no more than six seconds’ warning of an obstacle ahead](https://arstechnica.com/cars/2018/05/emergency-brakes-were-disabled-by-ubers-self-driving-software-ntsb-says/), and perhaps as little as 1.3 seconds. 

Contrary to some early reports, the driver was not looking at a smartphone (although more time for our phones is one of the benefits to be expected from *actual* self-driving cars), but at "a touchscreen that was used to monitor the self-driving car software":

> "The operator is responsible for monitoring diagnostic messages that appear on an interface in the center stack of the vehicle dash and tagging events of interest for subsequent review," the \[NTSB\] report said.

# The Uncanny Valley

I wrote about this [uncanny valley problem of autonomous vehicles]({% post_url 2018-03-30-When-Robots-Kill %}) before:

> as long as human drivers are required as backup to self-driving tech that works most of the time, we are actually *worse off* than if we did not have this tech at all.
> 
> In the first known fatal accident involving self-driving tech, [the driver may have ignored up to seven warnings to put his hands back on the wheel](https://www.washingtonpost.com/news/the-switch/wp/2017/06/20/the-driver-who-died-in-a-tesla-crash-using-autopilot-ignored-7-safety-warnings/). That was an extreme case, with rumours that the driver may even have been watching a film on a laptop, but in the Arizona case, the driver may have had only between four and one seconds of warning. If you’re texting or even carrying on a conversation with other occupants of the car, four seconds to context-switch back to driving and re-acquire situational awareness is not a lot. One second? Forget it.

Uber may have made that already dangerous situation worse by [limiting the software’s ability to take action autonomously](https://www.bloomberg.com/view/articles/2018-05-25/uber-s-ghost-in-the-self-driving-machine-exposed) when it detected an emergency condition:

> the automated braking that might have prevented the death of pedestrian Elaine Herzberg had been switched off "to reduce the potential for erratic vehicle behavior." Such functions were delegated to the driver, who was simultaneously responsible for preventing accidents and monitoring the system’s performance.

In other words, to prevent the vehicle suddenly jamming on the brakes in unclear situations like the one in Arizona, where "the self-driving system software classified the pedestrian as an unknown object, as a vehicle, and then as a bicycle with varying expectations of future travel path", Uber simply opted to delegate all braking to the "safety driver" – while also requiring her to "monitor the system’s performance". This situation – distracting the driver who is also expected to take immediate (and correct) action in an emergency – could hardly have been better designed to produce the outcome we saw in Arizona.

This is exactly what [I predicted in my previous post on Uber]({% post_url 2018-03-30-When-Robots-Kill %}):

> Along the way to full Level 5 autonomy, we must pass through an “uncanny valley" of partial autonomy, which is actually more dangerous than no autonomy at all.
Adding the desperate urgency of a company whose very survival depends on the success of this research seems like a very bad idea on the surface of it. It is all too easy to imagine Uber (or any other company, but right now it’s Uber), with only a quarter or two worth of cash in the bank, deciding to rush out self-driving tech that is 1.0 at best.
> It’s said that you shouldn’t buy any 1.0 product unless you are willing to tolerate significant imperfections. Would you ride in a car operated by software with significant imperfections?
> Would you cross the street in front of one?

# What Next?

[Uber has now ceased tests of self-driving cars in Arizona](https://eu.azcentral.com/story/news/local/tempe-breaking/2018/05/23/uber-close-self-driving-operations-arizona/636974002/), but it is continuing the work in Pittsburgh, having already been [kicked out of San Francisco after one of its self-driving cars ran a red light right in front of SFMOMA](http://sfist.com/2017/02/25/self-driving_uber_that_was_caught_o.php). 

Despite these setbacks, it is however continuing work on its other projects, such as [flying taxis](https://www.thelocal.fr/20180524/uber-to-invest-20-million-to-build-flying-taxis-in-france). 

Thats seems perfectly safe, and hardly at all likely to go horribly wrong in its own turn.

![Drone crash during ski race](https://media.giphy.com/media/Yb8aUTrSAEjC/giphy.gif)

##### GIF is of a [drone almost crashing into a skier](https://www.skiracing.com/stories/fis-responds-to-madonna-di-campiglio-drone-crash) during a race in Madonna di Campiglio.

*** 

[^1]: Such as they are, yes, I am familiar with [The Invention Of Jaywalking](https://www.citylab.com/transportation/2012/04/invention-jaywalking/1837/).