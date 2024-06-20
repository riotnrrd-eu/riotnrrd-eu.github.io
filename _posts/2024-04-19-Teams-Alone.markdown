---
layout: post
title: Teams, Alone
date: 2024-04-19
categories: Zoom Teams Microsoft Slack enterprise
---

There is a lot going on in tech lately, what with companies like Humane and Apple releasing products that are actually [public betas]({% post_url 2024-04-14-Public-Betas %}). Perhaps it's natural, then, that a relatively lower-profile item of news like [Microsoft unbundling Teams from Office](https://www.reuters.com/technology/microsoft-separate-teams-office-globally-amid-antitrust-scrutiny-2024-04-01/) flew under many people's radar. 

At the same time, Zoom has realised that [its moat is being drained]({% post_url 2022-09-23-Draining-The-Moat %}) and has responded with [the introduction of Zoom Workplace](https://www.zdnet.com/article/zoom-gets-its-first-major-overhaul-in-10-years-powered-by-generative-ai/). Ignore the obligatory-in-2024 references to generative AI; the interesting part of this update is the leap forward in integrated collaboration features. Effectively, the new features attempt to replicate the rich document-based collaboration capabilities that were already in Teams.

These additions promise to make the chat features of Zoom actually useful for the first time since they were introduced. Zoom is of course limited in the capabilities that it can offer, since unlike Microsoft, it does not have its own Office suite, but is limited to working with public standards such as PDF, or its own existing whiteboard tool.

This whole situation is yet another variation on [Zawinski's Law](http://www.catb.org/jargon/html/Z/Zawinskis-Law.html):

> Every video calling app attempts to expand until it has document collaboration. Those apps which cannot so expand are replaced by ones which can.

Arguably, in today's work context video chat is just another feature of a general collaboration app, not a standalone app. In fact the anomaly has been this period in which Zoom, Slack, and Google Docs are distinct tools from separate vendors. 

# Back to the Browser Wars

This evolution from standalone tools to features of integrated platforms is reminiscent of the Browser Wars between Netscape and Microsoft (them again!) back at the turn of the last century. 

![](/images/netscape-3.jpg)

For those who were not around or have forgotten, there was a brief period at the dawn of the consumer Internet when there was a viable market for a commercial web browser. This was possible because consumer operating systems did not include that feature as a matter of course, as they do today. Netscape was doing well with its Navigator product — developed among others by Jamie Zawinksi, who coined the eponymous law that I (mis)quoted above. Then Microsoft introduced Internet Explorer as a built-in feature of its Windows operating system — and this at a time when Windows had something like 95% market share. 

This move immediately made life very difficult for Netscape, who sued Microsoft for anti-competitive behaviour. The trial dragged on for years, and the [result](https://en.wikipedia.org/wiki/United_States_v._Microsoft_Corp.#Settlement) satisfied absolutely nobody. It took long enough to reach that unsatisfactory settlement that it was mostly irrelevant anyway, from Netscape's perspective at least, as the market had moved forwards. Netscape the company was bought by AOL, and the code was released into the open-source world, where it survives today as Mozilla.

A major pushback against Netscape even at the time of the Browser Wars was that a web browser is a necessary component of an OS. This position has become mainstream now, to the point that a platform would today be considered incomplete without a built-in browser.

In the same way, an office suite without collaboration would be equally incomplete as an operating system without a built-in web browser. These days, video chat is commoditised: it's one collaboration feature among many.

But then, what about Chrome?

Internet Explorer won the Browser Wars, even becoming the default on MacOS, displacing Apple's short-lived but interesting [Cyberdog](https://en.wikipedia.org/wiki/Cyberdog) (yes yes, awful name that has not aged well). 

![](/images/adam-curtis.jpg)

\[Adam Curtis voice\] But then something strange happened: Google released its own web browser called Chrome, and it ate Internet Explorer alive. It got so bad that Microsoft ended up releasing its own Chrome-based web browser, called Edge — but even resorting to some pretty egregious dark patterns, and of course the built-in advantage of being the OS default, could not save Edge from Chrome's inexorable advances.

Only on Apple's platforms is there still a meaningful browser competition, partly because Safari is actually a pretty decent web browser, and partly because on iOS and iPadOS, it was until recently the only browser[^1] allowed.

In 2024, the EU forced Apple to open up iOS[^2] to alternative web browsers. On first launching Safari after the relevant OS update, users were presented with a series of screens that gave them the option to either select a new browser, or confirm their choice of Safari. 

![](/images/browser-choice-1.jpeg)
![](/images/browser-choice-2.jpeg)
![](/images/browser-choice-3.jpeg)
![](/images/browser-choice-4.jpeg)

This all seemed fairly uncontroversial to me, but of course people were complaining about [Apple’s dark patterns](https://arstechnica.com/tech-policy/2024/04/report-people-are-bailing-on-safari-after-dma-makes-changing-defaults-easier/). It's still early days — these changes only went live at the beginning of March, just over a month ago at time of writing, and will only affect users who upgrade their iPhone to the latest iOS release, so it makes sense that any change would be a slow burn. So far, the results seem to be large percentage increases on small absolute baselines, reported by the teams behind browsers like Opera (still around?), Vivaldi, and Aloha (who?).

# So, what next?

How does all this history apply to Zoom and Teams? 

Teams has arguably already got all the push it needed from integration with Office. The Teams payload is separating from the Office booster perhaps a little early, while there was still thrust to give — but Microsoft's plan is fairly transparently to avoid another decade of litigation and consent decrees, so they can get on with their other plans.

Zoom is arguably doing the right thing by adding collaboration (properly, as opposed to earlier half-hearted attempts). The problem Zoom has is that the customer base overlaps very significantly with Slack's, which offers all the collaboration its users could possibly want, and has a solid track record of delivering what people want. Slack even has video calls in the shape of Huddles, further proving my point that video calling is a feature, not a platform.

As these platforms converge, they are moving into Microsoft's home turf. Microsoft has never been the best at any one thing, focusing instead on (eventually) being the best overall with the widest coverage. Zoom and Slack on the other hand have always been predicated on being the best of their respective breeds, so this sort of miscegenation is foreign to them.

We have been here before, and I don't think the result is going to be different this time. After some upheaval, Teams will own this market — until something different comes along with incentives that are orthogonal to Microsoft's.

***

[^1]: Technically there were Chrome and Firefox apps available, but they still used Safari to render the actual content. The benefit of using these apps was more about synchronising bookmarks, history, and credentials with a full-blown desktop instance of those browsers.

[^2]: But in an interesting oversight, not iPadOS.