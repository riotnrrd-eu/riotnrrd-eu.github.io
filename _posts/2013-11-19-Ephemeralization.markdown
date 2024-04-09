---
layout: post
title:  Ephemeralization 
date:   2013-11-19 
categories:  cloud digital-life 
---

Working in cloud computing is extremely frustrating. Nobody outside the field understands what you do no matter how much you try to explain, and everybody in it thinks they already do before you get a chance to explain.

One of my favourite metaphors to try to break this impasse is to talk about fleets of aircraft. The Bad Old Way of doing things in IT is a bit like a company operating a huge fleet of private jets, one for each employee that ever needs to travel anywhere. Obviously extravagant and impractical, right? The planes are idle for much of the time while the people are doing whatever they travelled to do, and you can't easily make them bigger if you need to transport a larger team somewhere. The thing is, that's pretty much how we all approached IT until not so long ago: each workload got its own dedicated infrastructure, which was idle much of the time and very difficult to resize or reassign in response to changing requirements. Virtualization didn't really help, except as a band-aid over the problem. 

Cloud computing is more like having lots of different commercial carriers, each with different classes of service, routes, amenities and other offerings, with passengers (workloads) choosing supplier and service based on their requirements of the moment. 

![](/images/unknown_filename.135.jpeg)

As much as it is about anything, cloud computing is about impermanence. When you buy physical hardware, you own it, it's right there. The canonical definition of hardware is "the part that you can kick”. (Software, then, is the part that makes you want to kick the hardware.) These days, people who like their IT to be tangible are [disparaged](http://www.forbes.com/sites/benkepes/2013/10/24/server-huggers-and-henry-t-fords-faster-horse/) as "server huggers". The whole point of cloud computing is that if something breaks you don't worry about trying to fix it, you just get a new one, which will be the same as the original. Randy Bias coined the phrase “[cattle, not pets](http://www.theregister.co.uk/2013/03/18/servers_pets_or_cattle_cern/)": you don't give the servers names and pamper them as individuals, you give them numbers and put them down as soon as it's convenient. 

The dark side of this impermanence, though, is: what happens to the data in this new world of transience? When your cloud provider shuts down, what happens to everything that you entrusted them with over the years? What happens [when data disappears?](http://www.nytimes.com/2011/08/07/opinion/sunday/when-data-disappears.html)

It’s a nightmare for libraries. What do you do if you’re given a chunk of priceless [digital manuscripts](https://www.nla.gov.au/openpublish/index.php/nlasp/article/viewArticle/1321/1607) - stored on totally obsolete media? The trove might include [video games by Timothy Leary and digital drawings by Keith Haring](http://artsbeat.blogs.nytimes.com/2013/09/27/timothy-leary-video-games-unearthed-in-archive/), or [versions of famous Broadway shows](http://artsbeat.blogs.nytimes.com/2012/02/01/tale-of-the-floppy-disks-how-jonathan-larson-created-rent/), or, well, anything really.

On the other hand, the cloud can also be the solution. If you need to read a document created on some obsolete system that you no longer own or can even buy, perhaps you can emulate it in the cloud. [JSMESS](http://jsmess.textfiles.com/) is a project to port the MESS emulator to Javascript so that it will run in a browser. Right now it will emulate thirty-year-old kit with middling results, but as is the way of things, I have little doubt that before too long it will be able to emulate Windows 95 running Word Whatever. 

Why do you care? We are now living through what will doubtlessly be known as a Dark Age to future historians. A relative of mine wrote a book about his experiences in South Africa around the turn of the Twentieth Century. I doubt there are many copies around, but the family has one, and so I was able to read about how my relative was there for the founding of some of the institutions of modern South Africa, and his efforts to make it a better place. 

It is very hard to imagine that happening today. Nobody keeps a physical written diary that could be found in an attic, we write about our daily experiences on Facebook. Even when we do have local documents, they are saved in particular formats that will be very difficult or impossible to read a handful of years from now, never mind a century on. Version requirements, compatibility and dependencies, not to mention digital rights management, will see to that. 

Imagine though if you come across a trove of Grandpa's ancient backups, and you could boot something up right in your browser to read them. You might solve that inheritance dispute, or smile at his old love letters to Grandma. 

Imagine if you're in charge of a business and you suddenly realise you can't access your documents that are more than a few years old. What does that do to your billing, your credibility, not to mention your legal liability? Sure, you can print everything off and ship it to Iron Mountain or wherever, but the latency on accessing data held in that kind of facility would give your average Millenial conniptions. 

If you're a developer or a provider building something for the cloud - which these days means all providers and developers who plan to be around more than a couple of years from now - take this into account. How do users get at their stuff tomorrow, even if you're not around? Sure, you're busy building something cool, but this is foundational. If you build it right, ensuring accessibility in the future should be easy. If it looks too hard, you're probably doing something else wrong. 

If you're a user of cloud services - and once again, that pretty much means "a user" - try to take a moment to look into getting your data back. If I store my photos here, how can I download them? If I create a blog there, how can I save my posts? If my business relies on a certain service, what is my emergency spare backup plan if that service goes away or simply changes in a way that breaks it for me? 

You can't rely on the [Archive Team](http://www.archiveteam.org/index.php?title=Main_Page) to do it for you. If you want permanence, it takes a moment of effort. 

***
Image by [Joeri Romer](http://www.jfrwebdesign.nl/) via [Unsplash](http://unsplash.com/)