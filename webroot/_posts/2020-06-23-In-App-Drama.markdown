---
layout: post
title:  In-App Drama 
date:   2020-06-23 
categories:  Apple iOS hey 
---

# In-App Drama


Everyone and their dog has followed the saga of Hey and Apple — but in case you missed some of the twists and turns, [this is a decent recap from The Verge](https://www.theverge.com/2020/6/22/21298552/apple-hey-email-app-approval-rules-basecamp-launch).

My own opinion can be summed up as follows: “Wait, a hundred bucks a year?[^1] For *email*? In 2020? Are you ***insane***?” (We also discussed the Hey saga on [the most recent episode of the *Roll For Enterprise* podcast](https://overcast.fm/+a3gGER2NU).) In fact, I am far more interested in [Bye](https://bye.fyi), the Hey parody that promises to reply to all your email with insults.

That said, there are a couple of different aspects to this story that I think are worth looking at in more detail. One is the PR debacle that this whole saga has been for Apple, and the other is what any of it means for users.

![](/images/unknown_filename.181.png)

# PR Ju-Jitsu

The fact that all this drama went down in the week before WWDC, and at the very same time [the EU opens antitrust investigations into Apple’s App Store practices](https://www.theverge.com/2020/6/16/21292651/apple-eu-antitrust-investigation-app-store-apple-pay), led many to wonder whether this could be some mastermind move to generate the sort of PR money can’t buy for an email app (because, again, email simply is not exciting in 2020. Ahem). 

I don’t buy it. Oh, I am sure that the Hey team chose to launch the week before WWDC very consciously to get more attention, but they could never have expected Apple to approve their initial release, then reject a bug fix, and finally to be so ham-fisted in all of their subsequent moves. To be sure, David Heinemeier Hansson ([DHH on Twitter](https://twitter.com/dhh), Hey and Basecamp cofounder) rode the PR wave masterfully, positioning himself as the David (ha!) to Apple’s Goliath. He was largely successful in this effort, judging by an entirely unscientific survey of my Twitter feed.

On the other hand, I am equally sure that Apple did not deliberately set out to pick a fight with a Twitter loudmouth in the week before the biggest event of their year. It does seem that they have been trying for some time to get more paid apps to use their own in-app-purchase (IAP) mechanism, and the reviewer(s) for Hey didn’t anticipate this level of blowback from one more enforcement decision in what is already a long list.

Apple PR did make some pretty heavy-handed and tone-deaf moves. At one point, [a letter to Hey was apparently released to the press *before* it was sent to Hey](https://www.theverge.com/2020/6/18/21296180/apple-hey-email-app-basecamp-rejection-response-controversy-antitrust-regulation), which is bad enough, but that letter contains language that DHH was easily able to present as a threat to his *other* apps in the App Store, which also do not use IAP:

> Thank you for being an iOS app developer. We understand that Basecamp has developed a number of apps and many subsequent versions for the App Store for many years, and that the App Store has distributed millions of these apps to iOS users. These apps do not offer in-app purchase — and, consequently, have not contributed any revenue to the App Store over the last eight years. We are happy to continue to support you in your app business and offer you the solutions to provide your services for free — so long as you follow and respect the same App Store Review Guidelines and terms that all developers must follow.

To me this is not a threat, merely a statement of fact. Operating the App Store is not free, and Basecamp, by not offering IAP, has not contributed any revenue whatsoever to Apple.

![](/images/unknown_filename.182.png)

# Mob Tactics?

This is the key point: is Apple merely rent-seeking by attempting to extract their 30% cut from developers, or do they actually offer a service that is worth that overhead?

Ben Thompson has consistently been critical of the App Store’s regulations and their enforcement; in fact he goes so far as to consider it [an antitrust issue](https://stratechery.com/2018/antitrust-the-app-store-and-apple/), and [made hay (or Hey) with this story](https://stratechery.com/2020/hey-v-apple-follow-up-shopify-and-walmart-three-follow-ups/):  

> I would go so far as to say that executives in the tech industry are more afraid of Apple in 2020 than they were of Microsoft two decades ago. App Store Review is such an absolute gatekeeper, and the number of ways that Apple can retaliate are so varied and hard to verify, that no one is willing to publicly breathe a word against the company — again, except for Basecamp. I wish I could prove this to you — the stories I have received the last few days tell the tale — but no one is willing to go on the record, to me or to regulators. The risk is too great, because Apple’s level of control, and willingness to use it, is so overwhelming. I wish I were exaggerating, but I’m not.

It’s certainly true that the App Store extracts rent from developers, but the key point is that **it also adds substantial value**. All of the coverage of Hey has focused on Apple and on developers, but I have not seen any significant discussion of the users’ point of view. Customers are more willing to engage with a single trusted intermediary like Apple than with vast numbers of unknown developers. Especially with subscriptions, which are notorious for being easy to start and difficult to impossible to cancel, Apple’s role in the process is invaluable.

The user experience is better *because* of Apple’s aggressive curation of the App Store experience, and users are more willing to take a chance on apps because of that curation, and because of the established trust relationship they already have with Apple.

![](/images/unknown_filename.183.png)

# Friction Is Traction

It’s easy for DHH to say that Apple is interposing itself between him and his customers. He would rather have a direct relationship with them, and keep the 30% for his bottom line. In his view, the App Store and IAP add unnecessary friction to the smooth transmission back and forth. 

Here’s the thing, though: friction is not just a negative. If we remove all *friction*, we also lose all *traction*. Intermediaries like Apple add both friction and traction. The way they justify their 30% cut — the friction that DHH complains about —  is by offering traction: the technical underpinnings of the App Store — hosting, payments, marketing, and so on — but also by enabling developers to take advantage of the trust that Apple has built up with its customers. 

I am happy to have my credit card on file with Apple, so buying an app (or a book, or a film, or music back before I subscribed to Apple Music) is a one-click process. One of the reasons I trust Apple with my credit card is because they let me see and manage my subscriptions in one place, and they let me cancel them and even offer refunds of purchases simply and quickly. I have bought thousands of euros through Apple if you add up apps, books, and media; if I had had to register for each one of those purchases, and ask myself “do I trust this vendor not to scam me or just make my life difficult in some way?”, I would not have bought nearly as much.

The restrictions that Apple imposes on iOS — no side-loading of apps outside the App Store, sandboxing of individual apps, Apple ID login — may annoy developers and power users, but they also lower the barrier to installing new apps, because those apps cannot mess up anything else, either deliberately or on purpose. People who have experienced Windows are trained to be extremely reluctant to install new apps; no such caution is needed on iOS, in large part due to Apple’s oversight. 

None of this is to say that the App Store experience is perfect for users. I could definitely use better search, as scammy developers seem to be winning this round against Apple and have made searching within the App Store almost pointless. The review process itself needs to be *more* aggressive in my opinion; especially with my eldest now using the App Store, I have discovered a whole lot of scammy IAP practices! Even then, though, the parental controls built into iOS beat anything Google offers.

# Hey Hey, Bye Bye

Personally I hope Apple gets a fright and figures out a better way to continue to give me what I like as a user, without developers feeling ripped off. And regardless, there is no way I am dropping ***a hundred bucks a year***[^2] on email.

[^1]: And it turns out, shorter account names cost *even more*: "Ultra-short 2-character addresses like ab@hey.com are $999/year, and 3-character addresses like abc@hey.com are $349/year." I mean, genius business model, charge whatever the traffic will bear and so on, but I just can’t even.
[^2]: In fairness, Hey are hardly the only ones at the super-premium end of the email market. Superhuman charges $30/month to improve your Gmail experience, although [this review is pretty uncomplimentary](https://www.theverge.com/21299681/superhuman-email-app-review-price-gmail-iphone-mac).

