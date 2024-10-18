---
layout: post
title: That old open-source business
date: 2024-10-18
categories: Wordpress MongoDB open-source cloud
---

The whole Wordpress / WP Engine / Wordpress.org saga has brought the question of how to combine open-source ideals with running a business back into the headlines.

The story is fairly involved, but [this summary](https://www.computerworld.com/article/3564788/about-that-brawl-between-the-wordpress-co-founder-and-wp-engine.html) seems fairly complete and well-balanced. The key aspect from my perspective is that Matt Mullenweg, Wordpress CEO, is not going after any of the many, many organisations that are *using* Wordpress for their own purposes. He is specifically going after WP Engine, who has made a business of *hosting* Wordpress, for pay, and pretty transparently surfing on the wave of interest in Wordpress, even down to their actual name. Whether or not the "WP Engine" name rises to the level of being an actual trademark violation is a question that is above my pay grade, but nobody could claim with a straight face that it was not chosen to align the platform closely with Wordpress.

Wordpress is hardly the first organisation to have to deal with conflicts between open-source ideals (and licenses) on the one hand, and hard-nosed business on the other. I wrote about [MongoDB and Redis relicensing to the SSPL]({% post_url 2024-04-04-Defensive-Moves %}), and some of the factors driving that choice:

> - A vendor is running a classic Red Hat-style dual-track strategy, with an open-source “community” release and a commercial product on top. The value proposition for the latter is typically based on some combination of added closed-source enterprise functionality and official support contracts.
> - The open-source project is picked up by the cloud hyperscalers, who host it themselves, and contribute nothing back to the vendor acting as commercial shepherd of the project.
> - The vendor’s business quickly goes from being promising (look at all this community growth that can be monetised!) to extremely challenging (why would anyone deal with a subscale vendor when they can get the same experience in a couple of clicks from their current cloud vendor?).
> - Investors flee and the vendor goes into a death spiral, stabilising (in the best case) as a niche player in a community dominated by the hyperscalers.

In the case of Wordpress, substitute WP Engine (and [their backers, Silver Lake](https://www.silverlake.com/portfolio/wp-engine/)) for the cloud hyperscalers, and we see basically the same mechanism. The problem is *not* that individuals or companies are running open-source Wordpress to host their own blogs; that is part of the ecosystem, and indeed a sign of success for an open-source project. The business plan for Wordpress, though, is pretty obviously to fund open-source development efforts by offering managed, hosted Wordpress for users who don't want to be responsible for their own infrastructure. By paying for such a service, these users subsidise all the non-paying users who are willing to trade their own time and resources to host their own Wordpress instances without paying a license fee.

Something small-scale like a regional ISP offering that service to its local users is an acceptable drain on the pool of paying users. A well-capitalised and private-equity-funded competitor is not. Unfortunately, under the terms of the GNU General Public License under which Wordpress is released, there is not really any recourse against what I would term abuse of the open-source model, hence this ugly public fight.

# Add context to taste

As in the case of the SSPL, open-source purists object to *any* restrictions being placed on the end-user of the code. I do see where they are coming from, but I suspect at least part of this intransigence comes from a specific moment in time: namely, the late Nineties and early Oughts, also known as the era of "[embrace, extend, and extinguish](https://en.wikipedia.org/wiki/Embrace,_extend,_and_extinguish)". In those highly confrontational times, some on the FOSS side embraced the "poison pill" narrative, and actively sought out ways to make it impossible for commercial vendors to put the open-source genie back into the bottle.

However, as in so many other aspects, the rise of cloud computing has changed the landscape. This is no longer a world where we have to worry about Microsoft bundling open-source offerings with Windows to sell more boxed CDs. The major threat to open-source ecosystems is parasitical entities that host open-source tools in the cloud. If open-source is to survive as a business model, it must have reasonable revenue streams — and commercial hosting is one of the biggest. A license that prevents commercial hosting, while preserving the other freedoms, is much closer to the spirit of open-source than a PE-funded entity that hides behind the letter of the GPL to keep its own costs down. 

![SOS](/images/marcel-eberle-pZKCj9h10nI-unsplash.jpg)

Matt Mullenweg does appear to be pretty tone-deaf in his actions, but I do not think he is wrong in his overall instincts — and by reflexively opposing him, open-source partisans find themselves with some pretty unlikely — and unsavoury — bedfellows. Once again, I suggest that the ideals of open-source are much better served by addressing this issue than by focusing on the shibboleth of existing licenses. We should work together constructively to identify a framework that distinguishes between individuals and companies using open-source code for their own purposes, and hosting it for profit, and addresses those separately. 

The agreement should come first, and the legal language of the license second — otherwise, it becomes difficult to talk about *any* changes to the license, for fear that once one clause has been altered, all of the others are up for grabs. If instead there is a broad agreement that some types of usage are acceptable, and others are not, codifying that in one or several licenses becomes easier. 

Should these hypothetical new licenses be defined as "open source"? I remain of the opinion that excluding freeloaders does not meaningfully restrict the openness, but I recognise that others feel strongly about *absolute* openness being key to the community. If another term is required, may I suggest Sustainable Open Source? And yes, the SOS acronym is very deliberate — because unless we come to some sort of agreement, I worry that one more on-ramp to large-scale adoption will be severed, and we will all be poorer for it.

***

🖼️  Photos by [Marcel Eberle](https://unsplash.com/@marcel_eberle) on [Unsplash](https://www.unsplash.com)