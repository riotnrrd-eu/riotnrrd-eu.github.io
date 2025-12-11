---
layout: post
title: Granular Identity
date: 2025-12-11
categories: privacy UX
---

There are many good and excellent reasons to live in Italy, but one that is often overlooked in favour of food, wine, architecture, history, landscapes, culture, *deep breath*… is our digital ID system.

No, wait, come back!

In Italy there have been [national identity cards](https://en.wikipedia.org/wiki/Italian_electronic_identity_card) for everyone since basically forever. Okay, yes, civil libertarians, they were in fact introduced by the Fascists, but hear me out here. For a start, they are not technically speaking mandatory, and citizens are not obliged to carry them. However, the assumption that they are available and that everybody (to a first approximation) has one makes many situations which require identification much easier.

# Going Online

Over the last few years, they have switched from the old paper format to a plastic card, and more recently that has been augmented with an online electronic ID system. I think countries (*ahem* UK *ahem*) which get hysterical at the mere prospect of possibly considering the adoption of national ID cards could benefit from taking a look at Italy's system.

For a start, it's not a question of every busybody in the government down to the last provincial dog-catcher having access to everyone's personal information. When you log in to a service, you are presented with a list of all of the information which that service is requesting about you. 

![Granularity in action: name, rank, and serial number — and nothing else](/images/granularity.png)

As you can see, the list is pretty minimal: ID code, tax ID (this is a standard code in Italy used to verify entitlement to public services), and my contact info. And this is to sign in to my medical records, at that.

These sorts of granular controls[^1] are key to user trust in services. It's one thing for Google to store all my email and search records; it's quite another for them to use those however they want. If I were to log in to a site with my Google ID, I would like to see a screen like this one, explaining exactly what information about me the website is going to receive from Google. Instead, I log in via Apple ID with the "hide my email" option.

# A Helping Hand — If You Need It

There is another aspect to the thoughtful design of the Italian electronic ID, or SPID to its friends. This is a system which is designed to be accessible to everyone: all citizens and residents will need to use a SPID at some point. This universal mandate drives some pretty stringent usability requirements. However, one user's helpful assistance is another's annoying irritant. An older person without much digital literacy might require a lot of hand-holding, while digital natives can figure out what is after all a pretty simple website by instinct, and find too much signposting intrusive.

Here is how the health records system manages that dilemma:

![Assistance level slider](/images/GUI-help-controls.png)

When you first log in to this system, everything is turned on, and it gives you a guided walk-through of everything as if you had never seen or operated a website. But users can turn that assistance down, or entirely off.

When I log in, I experience blessed quiet in the UI, with nothing jumping out at me to tell me about the new whatever that has just been added to the user experience — just as God and Jakob Nielsen intended.

![Fog at Dover](/images/Hovercraft_Dover.jpg)

# Fog In Channel, Continent Cut Off[^2]

This whole system is not quite the [benevolent Big Brother]({% post_url 2013-10-23-Why-can't-Big-Brother-ever-lift-a-finger-to-help-out %}) I have wished for in the past, but it's getting pretty close.

This is why I have very little time for the reflexive British panic every time a national ID card for the UK is proposed. Of course it is possible to design such a system poorly, gathering too much information and sharing it willy-nilly with far too many US corporations for no good reason — except that it's supposed to be "innovative" somehow. I would also fully expect the current or any probable future UK government to try to do just that. But the alternative is… what? Keep on identifying yourself with a utility bill, like you're in a Dickens story or something? This is the 21st century: a more serious identity system is required, and examples of well-designed ones exist.

But of course the innate British chauvinism (bordering on xenophobia) kicks in whenever anyone suggests that it might be possible to learn something by looking beyond the UK's borders. This attitude was exemplified for me during the first Covid lockdowns, when I was already shut up at home in Italy — and British colleagues were still going to events at the Excel, suggesting that the NHS would surely manage where the disorganised Italian health service had failed.

Or there were the Pendolino high-speed trains which British train operators bought from Italy — and then ran on rails first laid down by Robert Stevenson with his own bare hands, complaining all the time about rubbish Italian trains. Of course the trains ran fine on the dedicated high-speed rail network which had been built out in Italy.

At this point of history, I would suggest that the UK should embrace its status as a mid-tier European power, with lots to learn from its peers on the Continent.

*** 

🖼️  Photos by [Roland Arhelger](https://commons.wikimedia.org/wiki/User:Roland_Arhelger) via [Wikimedia](https://commons.wikimedia.org/wiki/File:Hovercraft_Dover.jpg)

[^1]: Granularity is also alive and well in France: I was just at the APIdays event in Paris, and heard a fascinating talk about the French government's [DataGouv](https://www.data.gouv.fr) platform, which has the same ideas at its core.
[^2]: Yes yes, the story is probably [apocryphal](https://barrypopik.com/blog/fog_in_channel); let me have my fun, okay?