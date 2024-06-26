---
layout: post
title:  The curve points the way to our future 
date:   2016-05-06 
categories:  cloud devops tech enterprise docker 
---

# The curve points the way to our future


![](/images/unknown_filename.351.png)

Just a few days ago, I wrote [a post]({% post_url 2016-05-03-Multimodal-IT %}) about how technology and services do not stand still. Whatever model we can come up with based on how things are right now, it will soon be obsolete, unless our model can accomodate *change*.

One of the places where we can see that is with the adoption curve of Docker and other container architectures. Anyone who thought that there might be time to relax, having weathered the virtualisation and cloud storms, is in for a rude awakening.

## Who is using Docker?

Sure, the latest [Docker adoption survey](https://goto.docker.com/rs/929-FJL-1/images/Docker-Survey-2016.pdf) still shows that most adoption is in development, with 47% of respondents classifying themselves as "Developer or Dev Mgr", and a further 15% as "DevOps or Release Eng". In comparison, only 12% of respondents were in "SysAdmin / Ops / SRE” roles.

Also, 56% of respondents are from companies with fewer than 100 employees. This makes sense: long-established companies have [too much history]({% post_url 2014-08-06-Australia %}) to be able to adopt the hot new thing in a hurry, no matter what benefits it might promise.

What does happen is that small teams within those big companies start using the new cool tech in the lab or for skunkworks projects. Corporate IT can maybe ignore these science experiments for a while, but eventually, between the pressure of those research projects going into production, and new hires coming in from smaller startups that have been working with the new technology stack for some time, they will have to figure out how they are going to support it in production.

## Shipping containers

If the teams in charge of production operations have not been paying attention, this can turn into [Good news for Dev, bad news for Ops](https://www.moogsoft.com/whats-new/docker-good-news-dev-bad-news-ops/ ), as my colleague Sahil wrote on the official Moogsoft blog. When it comes to Docker specifically, one important factor for Ops is that containers tend to be very short-lived, continuing and accelerating the trend that VMs introduced. Where physical servers had a lifespan of years, VMs might last for months - but containers have been reported to have a lifespan *four times shorter* than VMs.

That’s a *huge* change in operational tempo. Given that shorter release cycles and faster scaling (up and down) in response to demand are among the main benefits that people are looking for from Docker adoption, this rapid churn of containers is likely to continue and even accelerate. 

VMs were sometimes used for short-duration tasks, but far more often they were actually forklifted physical servers, and shoe-horned into that operational model. This meant that VMs could sometimes have a *longer* lifespan than physical servers, as it was possible for them simply to be forgotten.

Container-based architectures are sufficiently different that there is far less risk of this happening. Also, the combination of experience and generational turnover mean that IT people are far more comfortable with the cloud as an operational model, so there is less risk of backsliding.

![](/images/unknown_filename.352.png)

## The Bow Wave

The legacy enterprise IT departments that do not keep up with the new operational tempo will find themselves in the position of the military, struggling to adapt to new realities because of its organisational structure. Armed forces set up for Cold War battles of tanks, fighters and missiles struggle to deal with insurgents armed with cheap AK-47s and repurposed consumer technology such as mobile phones and drones.

In this analogy, shadow IT is the insurgency, able to pop up from nowhere and be just as effective as - if not more so than - the big, expensive technological solutions adopted by corporate. On top of that, the spiralling costs of supporting that technological legacy will force changes sooner or later. This is known as the "bow wave" of technological renewal:

> "A modernization bow wave typically forms as the overall defense budget declines and modernization programs are delayed or stretched in the future," writes Todd Harrison of the Center for Strategic and International Studies. He continues: "As this happens the underlying assumption is that funding will become available to cover these deferred costs." These delays push costs into the future, like a ship’s bow pushes a wave forward at sea.

(from [here](http://warontherocks.com/2016/04/the-bow-wave-and-the-military-balance/ "THE BOW WAVE AND THE MILITARY BALANCE" ))

## What do we do?

The solution is *not* to throw out everything in the data centre, starting from the mainframe. Judiciously adapted, upgraded, and integrated, old tech can last a very long time. There are B-52 bombers that have hosted [three generations from the same family](http://www.dailymail.co.uk/news/article-2430802/David-Welsh-B-52-Air-Force-Capt-Daniel-Swoop-Welch-piloting-plane-father-flew-Cold-War-grandfather-flew-Vietnam.html "Patrolling the skies for 50 years in the world's most long-lived bomber: Air Force captain pilots a B-52 - just like his father and GRANDFATHER" ). In the same way, ancient systems like SABRE have been running since the 1960s, and still (eventually) underpin every modern Web 3.0 travel-planning web site you care to name.

What is required is actually something much harder: thought and consideration. 

Change is going to happen. It’s better to make plans up front that allow for change, so that we can surf the wave of change. Organisations that wipe out trying to handle (or worse, resist) change that they had not planned for may never surface again.

                                           