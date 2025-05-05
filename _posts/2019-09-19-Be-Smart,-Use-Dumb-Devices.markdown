---
layout: post
title:  Be Smart, Use Dumb Devices 
date:   2019-09-19 
categories:  privacy IoT Facebook 
---

The latest news in the world of Things Which Are Too “Smart” For Their Users’ Good is that [Facebook have released a new device in their Portal range](https://www.theverge.com/2019/9/18/20871173/facebook-portal-camera-price-release-date-availability): a video camera that sits on your TV and lets you make video calls via Facebook Messenger and WhatsApp (which is also owned by Facebook).

![](/images/101237.jpg)

This is both a great idea and a terrible one. I am on the record as wanting a webcam for my AppleTV so that I could make FaceTime calls from there:

![](/images/tweet-1143217474973970433.png)

![](/images/tweet-861965990153912320.png)

In fact, I already do the hacky version of this by mirroring my phone’s screen with AirPlay and then propping it up so the camera has an appropriate view.

Why would I do this? One-word answer: *kids*. The big screen has a better chance of holding their attention, and a camera with a nice wide field of view would be good too, to capture all the action. Getting everyone to sit on the couch or rug in front of the TV is easier than getting everyone to look into a phone (or even iPad). I’m not sure about the feature where the camera tries to follow the speaker; in these sorts of calls, several people are speaking most of the time, so I can see it getting very confused. It works well in boardroom setups where there is a single conversational thread, but even then, most of the good systems I’ve seen use two cameras, so that the view can switch in software rather than waiting for mechanical rotation.

So much for the “good idea” part. The reason it’s a terrible idea in this case is that it’s from Facebook. Nobody in their right mind would want an always-on device from Facebook in their living room, with a camera pointed at their couch, and listening in on the video calls they make. Facebook have shown time and time and time again that they simply cannot be trusted.

An example of why the problem is Facebook itself, rather than any one product or service, is the hardware switch for turning the device’s camera off. The highlight shows if the switch is in the off position, and a LED illuminates… to show that the camera and microphone are off.

![](/images/101251.jpg)

Many people have commented that this setup looks like a classic dark pattern in UX, just implemented in hardware. My personal opinion is that the switch is more interesting as an indicator of Facebook’s corporate attitude to internet services: they are always on, and it’s an anomaly if they are off. In fact, they may even consider the design of this switch to be a positive move towards privacy, by highlighting when the device is in “privacy mode”. The worrying aspect is that this design makes privacy an anomaly, a mode that is entered briefly for whatever reason, a bit like Private or Incognito mode in a web browser. If you’re wondering why a reasonable person might be concerned about Facebook’s attitude to user privacy, a quick read of [just the “Privacy issues” section of the Wikipedia article on Facebook criticism](https://en.wikipedia.org/wiki/Criticism_of_Facebook) will probably have you checking your permissions. At a bare minimum, I assume that entering “privacy mode” is itself a tracked event, subject to later analysis…

# Trust, But Verify

IoT devices need a high degree of trust anyway because of all the information that they are inherently privy to. Facebook have proven that they will go to any lengths to gather information, including information that was deliberately not shared by users, process it for their own (and their advertising customers’) purposes, and do an utterly inadequate job of protecting it.

![](/images/tweet-1116670170980859905.png)

The idea of a smart home is attractive, no question – but why do the individual *devices* need to be smart in their own right? Unnecessary capabilities increase the vulnerability surface for abuse, either by a vendor/operator or by a malicious attacker. Instead, better to focus on devices which have the minimum required functionality to do their job, and no more.

A perfect example of this latter approach is [IKEA’s collaboration with Sonos](https://techcrunch.com/2019/07/25/sonos-and-ikeas-symfonisk-wireless-speakers-are-a-symphony-of-sound-and-design/). The Symfonisk speakers are not “smart” in the sense that they have Alexa, Siri, or Google Assistant on board. They also do not connect directly to the Internet or to any one particular service. Instead, they rely on the owner’s smartphone to do all the hard work, whether that is running Spotify or interrogating Alexa. The speaker just plays music.

I would love a simple camera that perched on top of the TV, either as a peripheral to the AppleTV, or extending AirPlay to be able to use video sources as well. However, as long as doing this requires a full device from Facebook[^1] – or worse, plugging directly into a smart TV[^2] – I’ll keep on propping my phone up awkwardly and sharing the view to the TV.

[^1]: Or Google or Amazon – they’re not much better.
[^2]: Sure, let my TV [watch everything that is displayed](https://www.nytimes.com/2017/02/07/business/vizio-television-vizio-collected-viewers-habits-consent.html) and upload it for creepy “analysis”.[^3]
[^3]: To be clear, I’m not wearing a tinfoil hat over here. I have no problem simply adding a “+1” to the viewer count for **The Expanse** or whatever, but there’s a lot more that goes on my TV screen: photos of my kids, the content of my video calls, and so on and so forth. I would not be okay with sharing the entire video buffer with unknown third parties. This sort of nonsense is why my TV has never been connected to the WiFi. It went online once, using an Ethernet cable, to get a firmware update – and then I unplugged the cable.