---
layout: post
title:  Mythical Intelligence
date:   2026-04-09
categories:  AI security IoT
---

The current wave of "AI" interest, spawned largely since the public release of ChatGPT, has always had a dark side. The positive side is all about new possibilities enabled by LLMs, whether for individuals or for companies. The dark side talks about [P\(doom\)](https://en.wikipedia.org/wiki/P(doom)), the probability of AI causing some sort of doom, whether through the advent of some sort of super-intelligence that turns us all into paperclips, or more indirectly, through humans using advanced AI capabilities to engineer novel pathogens or whatever.

It's important to note that both sides are still talking about wondrous new capabilities of the technology, which explains the otherwise seemingly contradictory fact that many AI-doomers are also AI industry leaders. The obvious response to an intrinsically dangerous technology would be simply not to develop it, but their answer is instead that the tech will inevitably be developed, and so it is better that they forge ahead with it, since only they can be trusted to be responsible stewards of something so dangerous (and powerful, don't forget powerful).

One of the arguments of AI-doomers is that the models will be able, not just to create new software, but to identify vulnerabilities in existing software. Now [Anthropic has created \(but not released\) Mythos, a model which claims to be able to create and exploit new previously-unknown vulnerabilities](https://www.theregister.com/2026/04/07/anthropic_all_your_zerodays_are_belong_to_us/):

> "AI models have reached a level of coding capability where they can surpass all but the most skilled humans at finding and exploiting software vulnerabilities," the company said.
> 
> Mythos is markedly different from Claude Opus 4.6, which Anthropic only recently said was not very skilled at developing working exploit code. Where Opus 4.6 managed an exploit development success rate of just over zero percent, Mythos Preview generated a working exploit 72.4 percent of the time.

Anthropic has at least been somewhat responsible, in that Mythos has not (yet) been released to the public, but instead is being managed under the auspices of something called [Project Glasswing](https://www.anthropic.com/glasswing):

> Participants include: Amazon Web Services, Anthropic, Apple, Broadcom, Cisco, CrowdStrike, Google, JPMorganChase, the Linux Foundation, Microsoft, NVIDIA, and Palo Alto Networks.

So far so good: I am glad to see companies whose products I rely on in that list, getting early warning about issues in their products, and (one hopes!) rushing to develop patches.

But therein lies, as they say, the rub. Identifying a vulnerability is one thing, fixing it is another, but deploying the fix? That's the big challenge, and it's not one that AI can help with. 

Sure, modern operating systems have auto-update mechanisms — and most civilian users in my experience blithely ignore them, or routinely operate their devices in such a state (overflowing storage, typically) that the automatic updates cannot be received. That's already a huge vulnerability surface that is going to get attacked even more relentlessly just as soon as Mythos (or something just like it) falls into the hands of script kiddies everywhere. This is the [Blinking Twelves Provblem]({% post_url 2017-10-16-The-Internet-of-(Insecure)-Things %})

The problem is bad enough for new systems. If we are entering an era of all bugs being shallow, given enough LLMs, what does that mean for older software? I have an old Mac mini, still perfectly functional as a headless server running various services around the house, but it long ago aged out of receiving OS updates (and more recently, also app updates) from Apple. I guess I'll finally have to get around to migrating it to FreeBSD or something, in the hope that at least I can receive the fixes to the bugs Mythos found — and of course I have the privilege of doing something like that, instead of facing a choice of spending money on a new device, or losing access to the functionality of the existing one. The kids broke the last old iPad we had lying around, so at least that problem has been solved for us, but how many families have an pass-me-down old tablet that is just a cartoon-delivery device?

![An abandoned washing machine in an alley](/images/simon-hurry-HPiqJ1uVnW8-unsplash.jpg)

Finally, literally while typing this, it occurs to me to consider all the embedded devices which I cannot update. My home internet, like most people's, travels through a modem supplied by my ISP that runs some sort of specialised Linux distro which I have no access to. My TVs all run entirely air-gapped (I use AppleTV everywhere), but for most people, their "smart" TV is connected directly to the wifi and still blissfully running the same software it left the factory with. 

TVs are at least visibly "smart" devices. Meanwhile, my washing machine has online features which I find mildly useful. Mainly, it tells me when the wash is done, and if I need to do some sort of specialised wash — trainers, say — I can download instructions from the Internet and send them to the machine directly. Hardly life-changing stuff, I'll admit, but it has some sort of minimal software stack to deliver them, and I have no idea how or even whether I can force an update, even assuming the manufacturer provides one. To be clear, actual day-to-day operations are done from the front panel, so I could cut it off from the wifi, but I'd lose some small convenience by doing so. 

Maybe that P(doom) number just ticked up a little…

***

🖼️  Photo by [Simon Hurry](https://unsplash.com/@bullterriere) on [Unsplash](https://www.unsplash.com)