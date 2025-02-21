---
layout: post
title:  That Old Enterprise Software Business 
date:   2016-07-11 
categories:  HP Mercury enterprise 
---

This is an interesting time in the enterprise software market. The shift to the cloud is causing massive disruption, with storied old names struggling to reinvent themselves, and scrappy startups taking over the world.

One interesting story is that HP Enterprise, or HPE - one of the units that old HP split itself into - is looking into [selling off some of its software assets](http://www.bloomberg.com/news/articles/2016-07-08/hewlett-packard-enterprise-said-to-mull-selling-software-assets). I am especially interested in one of these, namely Mercury, because I worked there for several years.

![](/images/unknown_filename.344.jpeg)

![](/images/unknown_filename.345.png)

![](/images/unknown_filename.346.png)

To recap, [Mercury](https://en.wikipedia.org/wiki/Mercury_Interactive) (née Mercury Interactive) was a leader in automated software testing. Its products covered functional testing (XRunner, WinRunner, QuickTest Professional), load testing (LoadRunner), and test management (TestDirector, later renamed to QualityCenter).

Basically what these tools let you do is to record a user interacting with an application, and then parameterise the recording - i.e. turn it into a little programme that you can replay, so that you can select different menu options and make sure that they all work, or simulate ten thousand users all hitting the app simultaneously and make sure it doesn’t fall down, or whatever.

LoadRunner in particular was the default standard at the time, dominating its market segment. I worked on the functional test products, but because of language coverage, I had at least basic familiarity with the whole product set.

# Out Of The Blue

In 2006, Mercury was trying to bridge that difficult chasm from $1B to $2B in revenue, but was caught up in a wider [stock option backdating scandal](http://seekingalpha.com/article/12090-mercury-and-comverse-strategic-fall-to-the-pink-sheets-merq-cmvt). As its founder was exiled and the stock price cratered, HP swooped in and [bought up the whole shop in a fire sale](http://www8.hp.com/us/en/hp-news/press-release.html?id=169236#.V4ifNpWw2Rs "HP to Acquire Mercury Interactive Corp." ).

*** 

UPDATE: [Christopher Lochhead interviewed Dr Giora Yaron on his excellent *Legends & Losers* podcast about this history](https://overcast.fm/+IUNyYjZK8). Dr Yaron was on the board of Mercury at the time, while Chris himself was the CMO there. It was fascinating to hear the inside account of what happened during that tumultuous time. 

*** 

What happened after that is fairly typical of such acquisitions. Despite some big talk and high expectations, I think it is fair to say that the Mercury products languished within HP - or at the very least failed to evolve with any urgency.

![](/images/unknown_filename.347.jpeg)

# After The Acquisition

This is unfortunately a pattern with technology acquisitions. There is often a honeymoon period, where increased funding enables delivery of long-awaited functionality, but the releases after that get hollowed out into maintenance releases, and even those start coming further and further apart, frustrating customers and insiders alike.

In the case of HP and Mercury, the slow-down was particularly unfortunate because the acquisition came just as enterprise application development was moving from proprietary protocols and GUIs to web applications talking HTTP. Mercury’s powerful and extremely customisable products were arguably overkill for simpler web applications, and a new generation of tools was beginning to emerge that was dedicated for that purpose. Given its singular focus on testing, and based on what I know of the company culture pre-acquisition, I am quite certain that an independent Mercury would have addressed the challenge head on and remade itself for that new world. After all, Mercury was fully aware of web applications, offering services that would simulate user access from locations around the world to have a continuous view on sites’ performance as experienced around the world.

Unfortunately, that’s not what happened under HP stewardship. The Mercury products languished in the Software group, which itself represented only [around 2% of HP revenues](http://h30261.www3.hp.com/~/media/Files/H/HP-IR/documents/reports/2011/hewlett-packard-annual-report-final-pdf.pdf). As often happens in such cases, much of the original talent left, creating a flourishing “alumni” network. I was part of that diaspora, so I can’t talk about the quality of their replacements, but there was certainly a discontinuity, and the Mercury tools never recovered their previous dominance.

![](/images/unknown_filename.348.png)

# Looking On The Bright Side

None of this is to say that the acquisition was not a success by its own lights. HP still uses the Mercury technology in all sorts of places. Many enterprise HP customers did not move to the new technologies with any urgency, and therefore continued to have a business need for Mercury’s powerful tools. This means that the products still throw off enough stable and predictable revenue to make a private equity purchase potentially attractive

HP also adopted the Mercury notion of [Business Technology Optimization](http://www.theregister.co.uk/2005/10/10/mercury_bto/), or BTO. This acted as a framework for many of HP’s other software initiatives, although it seems to have been abandoned more recently.

The failure of this acquisition is a failure of potential. What might an independent Mercury have become if the M2B project had been successful in taking it to $2B in revenue and beyond? What might Mercury have built in the world of the web and the cloud? As is often the case with these acquisitions, there is no way to know.

We do know roughly what the conditions are under which acquisitions succeed or fail. Arguably, the Mercury acquisition was more successful than most in no small part because HP kept the Mercury R&D centre in Israel, somewhat isolated from the rest of the company. This enabled the ex-Mercury staff to keep some sense of their own distinct identity, and keep developing their technology even after the acquisition.

There is an alternative view: that while isolation and even benign neglect may allow for survival of the startup within the acquiring company, they will not build true success. That requires a deeper integration of the startup's mentality into the acquiring company’s culture. Very few company cultures have the strength to be able to integrate a challenging outside vision without triggering an immune reaction of sorts.

The only way to integrate acquired companies - their technology and their culture - successfully, is to have strong executive guidance over a period of years. This has been a long-time failing at HP, to the despair of its longer-serving employees. In the absence of that guidance, benign neglect is maybe all that can be hoped for.