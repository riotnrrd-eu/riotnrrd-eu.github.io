---
layout: post
title:  Important, But Not Exciting 
date:   2020-09-29 
categories:  automation bladelogic Chef Puppet 
---

# Important, But Not Exciting


I don’t usually do breaking news here, but this story pushes a whole lot of my buttons. Today, VMWare announced their intent to [acquire SaltStack](https://www.vmware.com/company/news/updates/2020/intent-to-acquire-saltstack.html). 

![](/images/unknown_filename.178.png)

I have been following the automation market closely, at least since my time at [BladeLogic](https://findthethread.postach.io/tag/bladelogic). With BladeLogic acquired by BMC, and arch-rival Opsware by HP, much of the action moved to the open-source realm, with Puppet, Chef, Ansible, and SaltStack. Of those four, only Puppet remains as an independent player[^1]; Ansible was [bought by Red Hat](https://www.ansible.com/blog/red-hat) back in 2015, and of course Red Hat were themselves [snapped up by IBM](https://www.redhat.com/en/about/press-releases/ibm-closes-landmark-acquisition-red-hat-34-billion-defines-open-hybrid-cloud-future) a few years later. 

There was a gap after that, but just this month [Chef was bought by Progress](https://www.marketwatch.com/press-release/progress-announces-acquisition-of-chef-2020-09-08) (who?), and now there is this Ansible news.

While merging automation functionality in the shape of Ansible into Red Hat made a lot of sense, the reaction to the Chef acquisition was more one of bemusement. [We discussed the acquisition on a recent episode of the *Roll for Enterprise* podcast](https://anchor.fm/dashboard/episode/ejhiv1), and the only strategic rationale any of us could see for the acquisition was a possible integration with Whats Up Gold, as part of some sort of integrated detection and remediation play. I haven’t seen any further news from that direction, but it’s only been three weeks, so based on my own experience during acquisitions, I wouldn’t necessarily expect anything for a while yet.

## The Action Moves Up The Stack

That theory about the role of automation in the modern infrastructure stack explains both why automation specialists no longer have the sorts of growth prospects (and valuations) that they did fifteen years ago at the time of the BladeLogic and Opsware acquisitions, and why they are being bought up now.

As the interface to software stacks moves further and further away from the bare metal, adding more and more layers of abstraction, the role of automation becomes that of plumbing: it’s important, perhaps crucial, but it’s invisible unless it breaks or fails. Arguably, this is a positive development, signifying the maturity of the automation market. Technology that is visible is cutting-edge and unreliable. There is a reason it’s called the bleeding edge; given the choice, I’d rather it be someone else’s blood getting spilled, while I hold back and learn from their mistakes.

![](/images/unknown_filename.179.png)

Once that exciting technology settles down and becomes better understood, it disappears from our attention. We don’t think about what happens when we flip a switch, because we simply expect the light to come on. Intellectually we understand that there are all sorts of systems in place to make that light come on, that specialists work hard around the clock to look after those systems, and that there is a whole world of complexity around the generation and transmission of electricity, but ultimately all we care about is that it ultimately enables us to reach out and say “let there be light”.

Automation is getting to that point: it’s a must-have, and because it’s a must-have, it’s no longer tenable for everyone to have to roll their own. In the dawn of personal computing, it was reasonable to expect every computer owner to bring their own soldering iron. That was obviously not a setup that could drive mass adoption, and these days, our computers are sealed shut, with no moving parts, let alone user-serviceable ones.

In the same way, back in the dog days of the last millennium, it was reasonable and even expected of me, as a junior sysadmin in training, to bang out a script that would let an Apache web server running on HP-UX authenticate users from a Windows NT domain — because there was no off-the-shelf way to do it. When I had to do add single sign-on to [a project of mine](https://developer.mongodb.com/article/build-newsletter-website-mongodb-data-platform) last year, the SSO part took me one line of config, and I was done with that task and could move on to something more interesting and value-additive.

Automation is no longer something the CIO will care about. It’s expected and built-in, and the action has moved elsewhere. This is a victory: it’s not every software category that lasts long enough to become legacy!

[^1]: VMWare had previously joined a [funding round for Puppet](https://techcrunch.com/2018/06/27/puppet-raises-42m-led-by-cisco-as-its-devops-automation-platform-passes-40000-businesses/); that round was led by Cisco, so it may be that Puppet’s new home is somewhere in Cisco’s Unified Computing division.

***
🖼️ Photo by [Yung Chang](http://yun-chan.com/blog) on [Unsplash](https://www.unsplash.com)

