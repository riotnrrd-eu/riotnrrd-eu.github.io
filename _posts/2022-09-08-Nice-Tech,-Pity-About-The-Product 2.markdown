---
layout: post
title:  Nice Tech, Pity About The Product 
date:   2022-09-08 
categories:  tech Apple technology MacOS BeOS 
---

# Nice Tech, Pity About The Product


Like many IT types, my workspace has a tendency to acquire obsolete technology. When I shared a flat in London with somebody else who lives with the same condition, computers significantly outnumbered people; heck, *operating systems* sometimes outnumbered people, even after our then-girlfriends/now-wives moved in! At one point, we even had an AS/400 desk-side unit that we salvaged, until we realised we really didn't have anything fun to do with it and moved it on again.

In the [big clear-out]({% post_url 2021-12-23-How-I-Work-From-Home %}) last year, I got rid of a bunch of the old stuff — yes, even some of the cables! One item made the opposite journey, though, from the depths of a box inside a cupboard of toner cartridges underneath a monitor so old it still has a 4:3 aspect ratio, to pride of place in my line of sight from my desk chair.

That item is the installation media for a thoroughly obsolete computer operating system from the 90s.

![](/images/110350.jpeg)

# What Even Is BeOS?

BeOS was the brain-child of a bunch of ex-Apple people, including [Jean-Louis Gassée](https://en.wikipedia.org/wiki/Jean-Louis_Gass%C3%A9e), who worked for Apple through the 80s and was instrumental in the creation of the Newton, among other things. While Apple spent the 90s trying and failing to [create a new operating system to replace the aging MacOS](https://en.wikipedia.org/wiki/Copland_(operating_system)), Gassée and his merry band created a brand-new operating system called BeOS. The 90s were probably the last time in history that it was possible to do something like that; the platforms that have emerged since then (iOS and Android) are variations on existing platforms (NeXTSTEP/OS X, which slightly predates BeOS, and Linux respectively).

Initially targeted at AT&T's Hobbit CPUs, BeOS was soon ported to the PowerPC architecture. These were the CPUs that powered Apple computers at the time, the product of an alliance between Apple, IBM, and Motorola. Between them, the three companies hoped to foster the emergence of an ecosystem to rival (or at least provide an alternative to) Intel's dominant x86. In those days, Apple licensed a handful of manufacturers to build [MacOS-compatible PowerPC computers]({% post_url 2016-08-01-Send-In-The-Clones %}), so Be quickly stopped manufacturing their own BeBox hardware and switched to offering the BeOS to people who owned these computers — or actual Apple Macs, I suppose, but even at the time you didn't hear of many people doing that.

This is where BeOS first entered my life. If you can believe it, the way you found out about cool software in those pre-broadband days was to buy a printed magazine that would come with a CD full of demos, shareware, utilities, wallpapers, icon sets, and more. There were a few magazines that catered to the Apple enthusiast market, and in 1997, I happened to pick one up that included Preview Release 2 of the BeOS.[^1]

Luckily for me, I owned a whopping 500MB external SCSI drive, so I didn't have to mess around with reformatting the main HDD of the family computer (which would probably have run all of 2GB at the time, kids!). I was quickly up and running with the BeOS, which absolutely blew away [the contemporary Macintosh operating system](<https://en.wikipedia.org/wiki/Mac_OS_8>).

![](/images/110421.jpeg)

# Why Bother With BeOS?

The performance was the first and most obvious difference between BeOS and MacOS. Just watching GLTeapot spinning around in real time was amazing, especially compared to what I was used to in MacOS *on the same hardware*. Check out [this contemporary review](<https://www.soundonsound.com/people/beos-operating-system-overview>), focusing specifically on BeOS’ multimedia capabilities.

This was also my first exposure to a `bash` terminal, or indeed any command-line interface beyond MS-DOS, and I can safely say that it was love at first sight, especially once I started understanding how the output of one command could be passed to another, and then the whole thing wired up into a script.

BeOS was properly multi-user, in a way that Classic MacOS very definitely wasn't. This factor made me consider it as a full-time replacement for MacOS on the family computer, but the lack of hardware support killed that idea. Specifically, the Global Village Teleport fax/modem which was our connection to the early Internet, running at a *blazing fast* 14.4kbps, did not work in BeOS.

![](/images/110437.jpeg)

This lack was doubly annoying since BeOS shipped with an actual web browser: [NetPositive](https://www.listofpopular.com/computers/list-of-world-best-and-fastest-web-browser-ever/netpositive-for-beos/), one of whose claims to fame was its haiku error messages. At the time, Mac users were stuck between Netscape Navigator, Microsoft Internet Explorer, Apple's almost wilfully obscure Cyberdog, and early versions of Opera.

# What Happened To BeOS?

This is where we get to the point of the story. What killed BeOS was not any sort of issue with the technology. It was leaps and bounds ahead of both dominant operating systems of the day, with massive developer interest.

Unfortunately, Be did not own its own destiny. After failing to sell itself to Apple, Be staggered on for a few more years. Once it became obvious that Apple was going to kill the MacOS clone business which powered the ecosystem of non-Apple PowerPC hardware that BeOS ran on, an x86 port was quickly added. By this point dual-booting operating systems on x86 had become, if not exactly mainstream, at least somewhat common in technical circles. Unfortunately for Be, the second OS (of course after Windows) was almost always Linux. A second commercial operating system was always going to be a hard sell in a world where everyone had already paid for a Windows license as part of the purchase price for their PC, to the point that Be literally couldn't even give it away. In fact [Be actually sued Microsoft over its alleged monopolistic practices](https://money.cnn.com/2002/02/19/companies/beos/index.htm), possibly the last gasp of the [First Browser War](https://en.wikipedia.org/wiki/Browser_wars#First_Browser_War_(1995–2001)) of the late 90s.[^2]

Be was eventually [sold to Palm](https://arstechnica.com/uncategorized/2001/11/2549-2/), and after Palm's own travails, the last vestiges of BeOS disappeared from public view only a few years later.

The lesson here is that **the best technology does not always win** — or at least, does not win unaided. Execution is key, and Be, despite some very agile pivots, failed to execute to the point of making any meaningful dent in the personal-computer-OS market.

What could Be have done differently? It's hard to say, even with the benefit of hindsight. None of the alternative desktop operating systems that sprang up in the late 80s and early 90s have survived. BeOS? Gone. OS/2 Warp? Gone. All the commercial UNIX systems? Gone — but maybe next year will be the year of Linux on the desktop. NeXT? It got acquired by Apple, and the tech is still with us in every current Apple platform — but if Be had been the one to get bought to replace the failed Copland project, NeXT would certainly have been the one to disappear.

That is the one inflection point really worth considering: what if Gassée had managed to negotiate a deal with Apple back then? What would OS X be like today if it were based on BeOS rather than on NeXTSTEP?[^3] And… what would *Apple* be like without Steve Jobs, in hindsight the most valuable part of the NeXT acquisition? There would probably still be a mobile product; one of the key Be employees was [Steve Sakoman](https://en.wikipedia.org/wiki/Steve_Sakoman), godfather of the Newton, so it seems fairly certain that a descendant of some sort would have emerged from a Be-infused Apple. But would it have become the globe-spanning success of the iPhone (and iPad) without Steve Jobs to market it?

One day I would like to own both a BeBox and a NeXTcube,[^3] but for now I just keep that BeOS PR2 CD as a tech industry *memento mori*, a reminder to myself not to get caught up in the elegance of the tech, but always to remember the product and the use cases which that tech enables.

[^1]: I could have sworn it was *MacAddict*, which was definitely my favourite magazine at the time, but [the only references I can find online say it was *MacTech*](https://www.mactech.com/1997/10/08/md1-beos-preview-release-2/), and it's been long enough that I can't be sure.

[^2]: Be's travails did inspire at least one high-profile fan, with Neal Stephenson discussing BeOS in his book-length essay [*In the Beginning... Was the Command Line*](https://en.wikipedia.org/wiki/In_the_Beginning..._Was_the_Command_Line), as well as giving it a cameo in *Cryptonomicon* (alongside "Finux", his gossamer-thin Linux-analogue).

[^3]: Yes, weird capitalisation has always been part of the computer industry.

