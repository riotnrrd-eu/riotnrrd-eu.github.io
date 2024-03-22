---
layout: post
title:  Stop doing that. 
date:   2012-12-10 
categories:  tech language google 
---

# Stop doing that.


Generally I prefer apps on my iDevices to web pages or "web apps". I like the offline access to historical data, I like the streamlined navigation, and I like the fact that interesting navigational concepts don't kill Safari with megabytes of JavaScript and CSS.

There is one thing that I *hate* about apps: they all insist on opening web pages inside the app.
Don't do that, not even if John Gruber [likes it](http://daringfireball.net/linked/2012/12/04/gmail-2).

For one thing, Safari has all the cookies, and I don't want to log in to things all over again just because I tapped on a link in an app rather than going through the browser. For another, Reader mode only works in real Safari, not embedded Safari. Finally, all my useful bookmarklets are also only available in Safari; things like "Save to Instapaper", for instance. Even Flipboard, possibly my very favourite iPad app, does this: if you're reading something and you want to bookmark it so that it will persist after you close Flipboard, you have to first "View on Web" and then "Open in Safari". At least these days you can "Read Later" directly from Flipboard without having to back all the way out to Safari, but waiting for developers of other apps to adopt your app is a major stumbling block for adoption of new useful apps.
Images are fine inline, but complete web pages should go to Safari, full stop.
A change will be needed in how Safari manages tabs for this to work. Either it needs a limitless number of tabs, to be managed like the iOS app list, or it needs a warning when opening a new tab will cause an existing one to be closed.

One other feature I want for iOS 7 is a central router for URLs, so that for instance everything to do with twitter.com gets sent to the Twitter app, no matter where it comes from. Some app developers seem to be onboard with this idea; twitter.com now displays a bar along the top of the page offering to open the current view in the native Twitter app, but Google+ and Facebook don't. This leads to the sort of idiocy we see in this screenshot, where clicking on a link in the Google+ iPad app spawns an embedded browser which does not have my G+ ackles.

![](/images/unknown_filename.330.png) 

*No, grazie.* 

This then triggers another rant of mine because Google in their wisdom send you all their content in the local language of wherever their geo-IP code thinks you're located, instead of, oh, for instance **respecting HTTP `Accept-Language` headers.**

At least Google seem to have fixed another pet peeve of mine, where the menu with all the different language options was itself localised. While one of the less-publicised benefits of a classical education is the ability to identify Αγγλικα in the menu when browsing from a beach bar somewhere in the Cyclades, this works less well in Riyadh or Bangkok.

![](/images/unknown_filename.331.png)

*Go on, now find English.*
 
Nowadays there's a nice "Google is also available in English" popup pretty much everywhere, so there's less call for appending `/ncr` to Google URLs. Progress, finally!
The good news is that things are moving in the right direction, as we can see in the examples of Flipboard and Google, but if the Daring Fireball is issuing plaudits for apps that reinvent their own wheel^W browser, maybe continued progress is not a given.

