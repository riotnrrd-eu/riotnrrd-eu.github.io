---
layout: post
title: For the record
date: 2024-10-16
categories: Apple MacOS Zoom Teams Microsoft
---

When Apple introduced macOS Sequoia, [one change provoked a particular *furore* among Mac power users](https://mjtsai.com/blog/2024/08/08/sequoia-screen-recording-prompts-and-the-persistent-content-capture-entitlement/): a new prompt to give apps permission to access the screen. In an unwelcome instance of Apple following a terrible trend, the prompt has no "allow forever" option; in fact, early betas had it returning after only a week, while the generally available release of Sequoia has the prompt returning after one month.

![Alert requesting screen recording permissions on macOS Sequoia](/images/shottr-permissions-screenshot.png)

You might think, who cares, I don't use a screen recorder or anything like that — but if you use your Mac for work, I guarantee that you use *something* that accesses the screen: Zoom, Teams, Google Meet, or perhaps even WebEx or Chime. I sit in multiple Zoom or Teams meetings every day (and yes, that does get exhausting after a while), so I was not looking forward to yet another permissions dialogue to deal with on a regular basis just to do my job.

Fortunately, Apple seems to have relented somewhat, and in the [release notes for the latest Sequoia beta](https://developer.apple.com/documentation/macos-release-notes/macos-15_1-release-notes#ScreenCaptureKit), we find this note:

> Applications using our deprecated content capture technologies now have enhanced user awareness policies. Users will see fewer dialogs if they regularly use apps in which they have already acknowledged and accepted the risks. 

On the one hand, yay: I use Zoom (all too) regularly, so I should not see this dialogue too often, or perhaps ever, after the first instance. On the other hand, what is the point if regular use is enough to make the warning go away? 

Full-screen access is a big deal, and it is good that Apple is securing this far-reaching permission — but surely requesting the permission at launch is sufficient. If all that is required to silence the notification is for the app to be used regularly enough — such as, for instance, on boot or login — how does that in any way enhance users' security?

There is one theory doing the rounds, and here I have (for once) to disagree with [Nick Heer of *Pixel Envy*](https://pxlnv.com/linklog/screen-recording-alert-changes/), although in fairness he is quoting [Benjamin Brooks of *The Brooks Review*](https://brooksreview.net/2024/10/screen-recording-changes-in-macos/):

> # Because corporate spyware, that’s why.
> 
> John Gruber asks:
> > Why in the world didn’t Apple take regular use of a screen-recording app into account all along?
>
> I think this is the question you ask when you have not used a Corporate Mac in the last 4-5 years. For those who are, you know that companies install applications which take screenshots and screen recordings of certain or all activities being done on the Mac. You know, for security.

I rate *The Brooks Review* on bags, but here I think he is way off. Every corporate Mac I have ever *seen* has some sort of remote meeting software installed, probably several. On the other hand, while they all also have security tools, vanishingly few of those do intrusive things like taking screenshots and screen recordings. This sort of nonsense may be more prevalent outside Europe, where it would be so radioactively illegal that the general counsel would be authorised to throw anyone who even *proposed* such a thing down the closest stairwell, but even when I travel to the US or talk to people from there, I don't hear of this sort of thing **on Macs**.

That last distinction is important: I know perfectly well that these sorts of tools exist and are deployed by companies, but I suspect they are more prevalent in the sorts of lower-paid jobs that don't rate fancy expensive Macs. This is why I don't think employee surveillance (or test proctoring, which is Nick Heer's other example) can be sufficient explanation for Apple walking back the frequency of this notification. Meanwhile, Zoom *et al* are near-universal on corporate Macs, and are going to be correspondingly closer to top of mind for administrators of Mac fleets.

All of this is not to blame the regular Apple pundits: they live in a world of individually-managed Macs, where they frequently do things like recording their own screens that are not typical for most users. Apple, understandably, focuses on the majority of their users. At this point in history, those are no longer the *Think Different* rebels all of us old-school Mac users like to think we are. Corporate buyers make up a huge percentage of Mac sales, and will have a corresponding influence on Apple's product planning — as much as anyone outside Cupertino can, of course.

That influence goes both ways, too: note that Apple is talking about "deprecated content capture technologies" in their note. All of this *Sturm und Drang* with the permissions only applies to apps that do not update to Apple's new preferred mechanism for accessing the screen in the first place. I would guess that corporate-managed Macs would be quite a bit behind the curve on OS upgrades: IT departments are conservative (for good reason!) about pushing major changes like that, and while some users (*raises hand*) will take it upon themselves to upgrade soon after release, most will not know or care. If Zoom updates its software to the new Apple-blessed APIs in the window of time between Sequoia's release and a substantial number of corporate users actually coming into contact with Sequoia, this whole thing will be a storm in a teacup.

The closest equivalent would be Apple dropping the SD card slot from their MacBook Pros: something which many reviewers made a huge issue of at the time, nobody I actually knew cared about, and everybody had forgotten about soon after, to the point that now I can't even find the contemporary blog posts complaining about this *terrible injustice* that Apple had done to its users.

This sort of nonsense is exactly why Apple is slow to respond to user demand: very often, users, and especially the most vocal users, do not actually know what they want or what is good for them.

***

🖼️  Shottr permission screenshot via [Jeff Johnson](https://lapcatsoftware.com/articles/2024/8/10.html) whose excellent apps you should definitely check out.