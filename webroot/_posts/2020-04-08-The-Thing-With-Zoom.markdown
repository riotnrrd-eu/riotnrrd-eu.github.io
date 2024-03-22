---
layout: post
title:  The Thing With Zoom 
date:   2020-04-08 
categories:  privacy security Facebook Zoom WebEx 
---

# The Thing With Zoom


Zoom was having an excellent quarantine — until it wasn’t.

This morning’s news is from *Bloomberg*: [Zoom Sued for Fraud Over Privacy, Security Flaws](https://www.bloomberg.com/news/articles/2020-04-08/zoom-sued-for-securities-fraud-over-privacy-security-flaws). But how did we get here?

Here is what’s interesting about the Thing with Zoom: it’s an excellent example of a company getting it mostly right for its stated aims and chosen target market — and still getting tripped up by changing conditions.

![](/images/unknown_filename.432.png)

To recap, very quickly: with everybody suddenly stuck home and forbidden to go to the office, there was an equally sudden explosion in video calling — first for purely professional reasons, but quickly spreading to virtual happy hours, remote karaoke, video play dates, and the like. Zoom was the major beneficiary of this growth, with [daily active users going from 10 million to over 200 million in 3 months](https://venturebeat.com/2020/04/02/zooms-daily-active-users-jumped-from-10-million-to-over-200-million-in-3-months/).

One of the major factors that enabled this explosive growth in users is that Zoom has always placed a premium on ease of use — some would argue, at the expense of other important aspects, such as the security and privacy of its users.

There is almost always some tension between security and usability. Security features generally involve checking, validating, and confirming that a user is entitled to perform some action, and asking them for permission to take it. Zoom generally took the approach of not asking users questions which might confuse them, and removing as much friction as possible from the process of getting users into a video call — which is, after all, the goal of its enterprise customers.

# Doing The Right Thing — Wrong

I cannot emphasise enough that this focus on ease of use is what made Zoom successful. I think I have used every alternative, from the big names like WebEx (even before its acquisition by Cisco!), to would-be contenders like whatever Google’s thing is called this week, to has-beens like Skype, to also-rans like BlueJeans. The key use case for me and for Zoom’s other corporate customers is, if I send one of my prospects a link to a video call, how quickly can they show up in my call so that I can start my demo? Zoom absolutely blew away the competition at this one crucial task.

Arguably, Zoom pushed their search for ease of use a bit too far. On macOS, if you click on a link to a Zoom chat, a Safari window will open and ask you whether you want to run Zoom. This one click is the only interaction that is needed, especially if you already have Zoom installed, but it was apparently still too much — so Zoom actually started *bundling a hidden web server* with their application, purely so that they could bypass this alert.

Sneaking a web server onto users’ systems was bad enough, but worse was to come. First of all, Zoom’s uninstall routine did not remove the web server, and it was capable of reinstalling the Zoom client without user interaction. But what got the headlines was the vulnerability that this combination enabled: a malicious website could join visitors to a Zoom conference, and since most people had their webcam on by default, active video would leak to the attacker.

This behaviour was so bad that Apple actually took the unprecedented step of [issuing an operating system patch](https://www.theregister.co.uk/2019/07/11/apple_removes_zooms_dodgy_hidden_web_server_on_mac/) to shut Zoom down.

![](/images/unknown_filename.433.png)

# Problem solved?

This hidden-web-server saga was a preview run for what we are seeing now. Zoom had over-indexed on its customers, namely large corporations who were trying to reach their own customers. The issue with being forcibly and invisibly joined to a Zoom video conference simply by visiting a malicious web server did not affect those *customers* – but it did affect Zoom’s *users*.

The distinction is one that is crucial in the world of enterprise software procurement, where the person who signs the cheque is rarely the one who will be using the tool. Because of this disconnect, vendors by and large optimise for that economic buyer’s requirements first, and only later (if at all) on the actual users’ needs.

With everyone locked up at home, usage of Zoom exploded. People with corporate accounts used them in the evening to keep up with their social lives, and many more signed up for the newly-expanded free tier. This new attention brought new scrutiny, and from a different angle from what Zoom was used to or prepared for.

For instance, it came to light that the embedded code that let users log in to Zoom on iOS with their Facebook credentials was [leaking data to Facebook even for users without a Facebook account](https://www.vice.com/en_us/article/k7e599/zoom-ios-app-sends-data-to-facebook-even-if-you-dont-have-a-facebook-account). Arguably, Zoom had not done anything wrong here; as far as I can tell, the leakage was due to Facebook’s standard SDK grabbing more data than it was supposed to have, in a move that is depressingly predictable coming from Facebook.

In a normal circumstance, Zoom could have apologised, explained that they had moved too quickly to enable a consumer feature that was outside their usual comfort zone without understanding all the implications, and moved on. However, because of the earlier hidden-web-server debacle, there was no goodwill for this sort of move. Zoom did act quickly to remove the offending Facebook code, but worse was to come.

Less than a week later, another story broke, claiming that [Zoom is Leaking Peoples' Email Addresses and Photos to Strangers](https://www.vice.com/en_us/article/k7e95m/zoom-leaking-email-addresses-photos). Here is where the story gets really instructive.

[twitter url="https://twitter.com/jasonpjason/status/1245013847255035906?s=21" ]

This “leak” is due to the sort of strategy tax that was almost inevitable in hindsight. Basically, Zoom added a convenience feature for its enterprise customers, called Company Directory, which assumes that anyone sharing the same domain in their email address works for the same company. In line with their guiding principle of building a simple and friction-free user experience, this assumption makes it easier to schedule meetings with one’s colleagues.

The problem only arose when people started joining en masse from their personal email accounts. Zoom had excluded the big email providers, so that people would not find themselves with millions of “colleagues” just because they had all signed up with Gmail accounts. However, they had not made an exhaustive list of all email providers, and so users found themselves with “colleagues” who simply happened to be customers of the same ISP or email provider. The story mentioned Dutch ISPs like xs4all.nl, dds.nl, and quicknet.nl, but the same issue would presumably apply to all small regional ISPs and niche email providers.

Ordinarily, this sort of “privacy leak” is a storm in a teacup; it’s no worse than a newsletter where all the names are in the To: line instead of being in Bcc:. However, by this point Zoom was in the full glare of public attention, and the story blew up even in the mainstream press, outside of the insular tech world.

# Now What?

Zoom’s CEO, Eric Yuan, issued a [pretty comprehensive apology](https://blog.zoom.us/wordpress/2020/04/01/a-message-to-our-users/). I will quote the key paragraphs below:

> First, some background: our platform was built primarily for enterprise customers – large institutions with full IT support. These range from the world’s largest financial services companies to leading telecommunications providers, government agencies, universities, healthcare organizations, and telemedicine practices. Thousands of enterprises around the world have done exhaustive security reviews of our user, network, and data center layers and confidently selected Zoom for complete deployment.
>
> However, we did not design the product with the foresight that, in a matter of weeks, every person in the world would suddenly be working, studying, and socializing from home. We now have a much broader set of users who are utilizing our product in a myriad of unexpected ways, presenting us with challenges we did not anticipate when the platform was conceived.
>
> These new, mostly consumer use cases have helped us uncover unforeseen issues with our platform. Dedicated journalists and security researchers have also helped to identify pre-existing ones. We appreciate the scrutiny and questions we have been getting – about how the service works, about our infrastructure and capacity, and about our privacy and security policies. These are the questions that will make Zoom better, both as a company and for all its users.
>
> We take them extremely seriously. We are looking into each and every one of them and addressing them as expeditiously as we can. We are committed to learning from them and doing better in the future.

It’s too early to say what the long-term consequences for Zoom will be, but this is a good apology, and a reasonable set of early moves by the company to repair its public image. To be clear, the company still has a long way to go, and to succeed, it will need to rebalance its exclusive focus on usability to be much more considerate of privacy and security.

For instance, there were [a couple of zero-days bugs found in the macOS client](https://objective-see.com/blog/blog_0x56.html) (since patched in Version 4.6.9) which would have allowed for privilege escalation. These particular flaws cannot be remotely exploited, so they would require would-be attackers to have access to the operating system already, but it’s still far from ideal. In particular, one of these bugs took advantage of some shortcuts that Zoom had taken in its installer, once again in the name of ease-of-use.

![](/images/tweet-1244737672930824193.png)

Installers on macOS have the option of running a “preflight” check, where they verify all their prerequisites are met. After this step, they will request confirmation from the user before running the installer proper. Zoom’s installer actually completed all its work in this preflight step, including specifically running a script with root (administrator) privileges. This script could be replaced by an attacker, whose malicious script would then be run with those same elevated privileges.

Personally I hope that Zoom figures out a way to resolve this situation. The user experience is very pleasant (even after installation!), and given that I work from home all the time — not just in quarantine — Zoom is a key part of my work environment. 

# Lessons To Learn

## 1: Pivoting is hard

Regardless of the outcome for Zoom, though, this is a cautionary tale in corporate life and communications. Zoom was doing everything right for its previous situation, but this exclusive focus made it difficult to react to changes in that situation. The pivot from corporate enterprise users to much larger numbers of personal users is an opportunity for Zoom if they can monetise this vastly expanded user base, but it also exposes them to a much-changed environment. Corporate users are more predictable in their environments and routines, and in the way they interact with apps and services. Home users will do all sorts of unexpected things and come from unexpected places, exposing many more edge cases in developers’ assumptions.

Companies should not assume that they can easily “pivot” to a whole new user population, even one that is attractively larger and more promising of profits, without making corresponding changes to core assumptions about how they go to market.

## 2: A good reputation once lost is hard to regain

A big part of Zoom’s problem right now is that they had squandered their earlier goodwill with techies when they hid a web server on their machines. Without that earlier situation, they might have been able to point out that many of the current problems are on the level of tempests in teacups — bugs to be sure, which need to be fixed, but hardly existential PROBLEMS.

As it happened, though, the Internet hive mind was all primed to think the worst of Zoom, and indeed actively went looking for issues once Zoom was in the glare of the spotlight. In this situation, there is not much to be done in the short term, apart from what Zoom actually did: apologise profusely, promise not to do it again, and attempt to weather the storm.

One move I have not yet seen them make which would be very powerful would be to hire a well-known security expert with a reputation for impartiality. One part of their job would be to act as figurehead and lightning conductor for the company’s security efforts, but an equally important part would be as internal naysayer: the [VP of Nope](201805141024.md), someone able to say a firm NO to bad ideas. Hiding a web server? Bad idea. Shortcutting the installer? Bad idea. Assuming everyone with an email address not on a very short list of mega-providers is a colleague of everyone else with the same email domain? Bad idea.

***

UPDATE: Showing how *amazingly prescient* this recommendation was, shortly after I published this post, Alex Stamos announced that he was joining Zoom to help them "build up their security program":

![](/images/tweet-1247866073682030592.png)

Alex Stamos is of course the ex-CSO at Facebook, who since departing FB has made something of a name for himself by commenting publicly about security and privacy issues. As such, he’s pretty much the perfect hire: high public profile, known as an impartial expert, and deeply experienced specifically in end-user security issues, not just the sort of enterprise aspects which Zoom had previously been focusing on.

I will be watching his and Zoom’s next moves with interest.

***

## 3: Bottom line: build good products

![](/images/tweet-1245352892334108672.png)

Most companies need to review both security and usability — but it’s probably worth noting that a good product is the best way of saving yourself. Even in a post-debacle [roundup of would-be alternatives to Zoom](https://www.theverge.com/2020/4/1/21202945/zoom-alternative-conference-video-free-app-skype-slack-hangouts-jitsi), Zoom still came out ahead, despite being penalised for its security woes. They still have the best product, and, yes, the one that is easiest to use.

But if you get the other two factors right, you, your good product, and your long-suffering comms team will all have an easier life.

***
🖼️ Photos by [Allie Smith](http://alliesmithphotography.com) on [Unsplash](https://unsplash.com)

