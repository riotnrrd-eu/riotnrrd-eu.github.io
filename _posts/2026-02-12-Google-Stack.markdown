---
layout: post
title: Google's Stack
date: 2026-02-12
categories: Google office work
---

That's it, I'm calling it: Google's apps are no longer "web apps" in any meaningful sense. 

A web app by definition works in any modern web browser. Google Docs no longer does that. If I have to have Chrome open to use Google Docs, how is that different from running the Microsoft Word (or Apple Pages) fat client directly? 

In fact it's probably more RAM-efficient. Each of my Google Docs tabs is consuming just shy of 1.5 GB of RAM. 

I'll just repeat that to let it sink in: ONE AND A HALF GIGABYTES of memory to load a single document. 

![A bloated horse](/images/bloated-horse.jpg)

Meanwhile, Microsoft Word, that paragon of lightweight agility, weighs in at less than 350 MB of RAM per document.

So that's the practical aspect. Then there is the philosophical aspect. [I run Safari rather than Chrome because it still behaves like a web browser, not a runtime for apps, which is what Google appears to think Chrome should be]({% post_url 2025-09-15-Thick-Web-Apps %}). A web app can run wherever any (reasonably modern) web browser can run; it doesn't require a particular rendering engine to be supported on the hardware. Already on iPad, I need the apps for Google Docs, Sheets, and Slides, because the web versions simply don't work. That is not how the Web is supposed to work.

I almost wish Google would just go ahead and ship Google Docs as an [Electron](https://www.electronjs.org) app on MacOS, since that's functionally where we are anyway. Bundling the rendering engine directly with the app that way would at least be more honest.