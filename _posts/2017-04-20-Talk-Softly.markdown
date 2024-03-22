---
layout: post
title:  Talk Softly 
date:   2017-04-20 
categories:  security Apple enterprise 
---

# Talk Softly


With the advent of always-on devices that are equipped with sensitive microphones and a permanent connection to the Internet, new [security concerns](http://www.csoonline.com/article/3190837/security/5-ways-to-keep-virtual-assistants-from-sharing-your-companys-secrets.html "How to keep virtual assistants from sharing your company's secrets" ) are emerging.

> Virtual assistants like Apple’s Siri, Microsoft’s Cortana and Google Now have the potential to make enterprise workers more productive. But do “always listening” assistants pose a serious threat to security and privacy, too?

![](/images/unknown_filename.337.png)

[Betteridge’s Law](https://en.wikipedia.org/wiki/Betteridge's_law_of_headlines) is in effect here. Sure enough, the second paragraph of the article discloses its sources: 

> Nineteen percent of organizations are already using intelligent digital assistants, such as Siri and Cortana, for work-related tasks, according to Spiceworks’ October 2016 survey of 566 IT professionals in North America, Europe, the Middle East and Africa.

A whole *566* respondents, you say? From a survey run by a help desk software company? One suspects that the article is over-reaching a bit - and indeed, if we click through to [the actual survey](https://community.spiceworks.com/research/future-of-it "Future Of It: Hype Vs. Reality" ), we find this:

> Intelligent assistants (e.g., Cortana, Siri, Alexa) used for work-related tasks on company-owned devices had the highest usage rate (19%) of AI technologies

That is a little bit different from what the *CSO Online* article is claiming. Basically, anyone with a company-issued iPhone who has ever used Siri to create an appointment, set a reminder, or send a message about anything work-related would fall into this category. 

Instead, the article makes the leap from that limited claim to extrapolating that people will be bringing their Alexa device to work and connecting it to the corporate network. Leaving aside for a moment the particular vision of hell that is an open-plan office where everyone is talking into the air all the time, what does that mean for the specific recommendations in the article?

> 1. Focus on user privacy
> 2. Develop a policy
> 3. Treat virtual assistant devices like any IoT device
> 4. Decide on BYO or company-owned
> 5. Plan to protect

These are actually not bad recommendations - but they are so generic as to be useless. Worse, when they do get into specifics, they are almost laughably paranoid:

> Assume all devices with a microphone are always listening. Even if the device has a button to turn off the microphone, if it has a power source it’s still possible it could be recording audio.

This is drug-dealer level of paranoia. Worrying that Alexa might be broadcasting your *super secret and valuable* office conversations does not even make the top ten list of concerns companies should have about introducing such devices into their networks.

The most serious threat you can get from Siri at work is co-workers pranking you if you enable access from the lock screen. In that case, anyone can grab your unattended iPhone and instruct Siri to call you by some ridiculous name. Of course I would *never* sabotage a colleague’s phone by renaming him “Sweet Cakes”. Ahem. Interestingly, it turns out that the *hypothetical* renaming also extends to the entry in the Contacts…

The real concern is that by focusing on these misguided recommendations, the focus is taken off advice that would actually be useful in the real world. For instance, if you *must* have IoT devices in the office for some reason, this is good advice: 

> One way to segment IoT devices from the corporate network is to connect them to a guest Wi-Fi network, which doesn’t provide access to internal network resources.

This recommendation applies to any device that needs Internet access but does not require access to resources on the internal network. This will avoid issues where, by compromising a device (or its enabling cloud service), intruders are able access your internal network in what is known as a “traversal attack”. If administrators restrict the device’s access to the network, that will also restrict the amount of damage an intruder can do.

Thinking about access to data is a good idea in general, not just for voice assistants or IoT devices:

> Since personal virtual assistants “rely on the cloud to comprehend complex commands, fetch data or assign complex computing tasks to more resources,” their use in the enterprise raises issues about data ownership, data retention, data and IP theft, and data privacy enforcement that CISOs and CIOs will need to address.

Any time companies choose to adopt a service that relies on the cloud, their attack surface is not limited to the device itself, but also extends to that back-end service - which is almost certainly outside their visibility and control. Worse, in a BYOD scenario, users may introduce new devices and services to the corporate network that are not designed or configured for compliance with organisations’ security and privacy rules.

Security is important - but let’s focus on getting the basics right, without getting distracted by overly-specific cybersecurity fantasy role-playing game scenarios involving Jason Bourne hacking your Alexa to steal your secrets.

