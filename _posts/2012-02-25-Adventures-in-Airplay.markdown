---
layout: post
title:  Adventures in Airplay 
date:   2012-02-25 
categories:  tech Apple 
---

# Adventures in Airplay


I have been trying off and on again to get one of my computers to act as an AirPlay client, that is, so that I could stream content from iPhones and iPads to their screens. The reason is that upstairs I have an AppleTV, but the downstairs TV isn’t able to talk to anything. It’s an older TV – doesn’t even speak HDMI – which is why it was demoted to a backup. However, since it’s just on the other side of a wall from my desk, it’s tethered (via DVI or VGA) to the Windows box.

I used to run [Boxee](https://www.boxee.tv/), and all was well. Boxee has a nice iOS [remote](http://itunes.apple.com/app/boxee-remote/id305171838), which gives my first-gen iPod Touch something to do with itself, and also has an extremely nice feature in a bookmarklet which lets users save videos straight from YouTube or whatever to their Boxee queue. The problem is that Boxee have, in their wisdom, decided to discontinue development of the downloadable version of Boxee in favour of their BoxeeBox hardware. This is a nice enough device, but it’s not worth three AppleTVs in my estimation, especially for a couple of hours’ use a month, which is what I would give it.

Watching local content is as as easy sending iTunes over to the secondary monitor and driving it with the Remote app when I want to watch something, but this doesn’t help with YouTube. There is [Leanback mode](https://www.youtube.com/leanback), but that requires more solutions, like the Remote Mouse app, to drive it.

I tried playing with [Clik](http://clikthis.com/), which is commendably simple: visit the website, it flashes up a QR code; scan the QR code with the [iPhone app](http://itunes.apple.com/app/clik/id495880232), and you can browse videos on the iPhone and play them in the browser window. It doesn’t deal with subscriptions, though, and a big goal of the exercise is to be able to watch videos from the [/Drive](https://www.youtube.com/user/drive) channel, so it’s not ideal.

Next I tried getting one of the computers to act as an AirPlay host. First I tried Windows, simply because the cable already reaches that box, so it requires the least amount of effort. [AirMediaPlayer](http://www.softpedia.com/get/Multimedia/Video/Video-Players/AirMediaPlayer.shtml) is nice and free, but only lets me view photos, not video – it doesn’t even show up as a host in video or audio mode. That seems to be the only free solution, so that’s Windows out.

Next we try the Mac. This is less than ideal because my Mac is a MacBook Air, so it would require connecting two cables (no HDMI, remember?) each time. However, I assumed that in the Apple world someone must have hacked AirPlay. Sure enough, [Erica Sadun had](http://ericasadun.com/category/airplayer/) – but it doesn’t work for me.

Finally I got desperate and tried FreeBSD. The Totem player has a [plugin for AirPlay](http://cgit.sukimashita.com/totem-plugin-airplay.git/), so full of hope I spent quite a lot of time downloading Totem and sorting out its dependencies, then getting Git and its dependencies, and finally found that… it doesn’t work: `Totem-WARNING **: Error, impossible to activate plugin ‘AirPlay Support 1.0.2′`. Joy.

So it looks like that’s it. Unless something changes, I’m going to wait for the [Raspberry Pi](http://www.theverge.com/2012/1/22/2724173/raspberry-pi-xbmc-airplay-1080p) and try that. Any suggestions, drop me a line.