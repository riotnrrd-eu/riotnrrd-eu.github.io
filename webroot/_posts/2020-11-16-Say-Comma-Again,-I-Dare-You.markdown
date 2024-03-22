---
layout: post
title:  Say Comma Again, I Dare You 
date:   2020-11-16 
categories:  microsoft UX 
---

# Say Comma Again, I Dare You


For my sins, I have been working with CSV files in Excel again — and it's giving me an aneurysm, as usual.

If you haven't had the (dis)pleasure, here's how the Import wizard works in Excel. You do File > Import, and choose CSV — so far so good:
![](/images/image.98.png)

Now, make careful note of the explanation: "Text files that contain comma-separated values".

Here is where the insanity begins: the wizard somehow decides that my text is *not* actually comma-delimited, as per the description above, but fixed-width:
![](/images/image.99.png)

I have no idea *how* the wizard arrives at this conclusion, because it does it for every single CSV file I have ever fed it.

Having reassured the wizard that no, I really *do* want my text delimited by characters such as, oh for instance **commas** because this is a file of **comma**-separated values — guess what the default character is that the wizard suggests?
![](/images/image.100.png)

Sure. Tabs. Not **commas**, for the file of (once again) **comma**-separated values. Tabs.

![](/images/CvXscAh.gif)

Now this might look like yet another minor annoyance, merely the latest in a series of papercuts that we have to deal with when we work with computers — but it's also a particularly egregious example of why people hate computers so much.

# Three Reasons Why This Is a UX Disaster

A computer should never ask the user a question to which it can work out the answer. It should have sane defaults, that work for most users most of the time. Finally, it should implement the user's inputs faithfully.

This wizard falls down on all three fronts:
1) It's a CSV file, you should know it's going to be comma-separated; why are you asking me?
2) Given that it's a CSV, the default should be to import the contents as comma-separated values, not tab-separated. Maybe have an Options button somewhere for weird edge cases, but the default flow if the user hits OK on every screen should make sense for the most usual case of a CSV file containing comma-separated data.
3) Gaslighting the user like this on every screen is just not acceptable. I feel like I'm trying to figure out how to avoid signing up to a junk mailing list, not using an ostensibly professional-grade, market-validated piece of software.

If you're writing even a simple program, at some point you're going to have to figure out inputs and what to do with them. Please, I implore you: do better than Microsoft.

