---
layout: post
title:  Keeping The Data Lake Clean 
date:   2018-09-25 
categories:  Apple sales Salesforce 
---

# Keeping The Data Lake Clean


One of the biggest problems in data analysis is making sure that your inputs are clean and sane. This holds true whatever you are using to do the analysis, whether it’s the latest fancypants machine-learning, or a roomful of expert humans doing the calculations by hand.

I think it’s useful to keep this perspective in mind when considering [Apple’s recent tie-up with Salesforce](https://www.salesforce.com/blog/2018/09/announcing-salesforce-apple-partnership.html "How Salesforce and Apple Are Improving Developer Tools and Training for All" ). 

![](/images/unknown_filename.204.png)

The first example given by Salesforce is this scenario:

> Imagine a sales rep saying "Hey Siri, Daily Briefing" then hearing an overview of their day.

This scenario encapsulates the dream end-state of all of these integrated CRM systems. Normally, of course, the user requesting an overview is not the sales rep but a manager, whether the person responsible for a region who needs to know whether their team of sales reps is going to hit the regional number, or a higher manager preparing a presentation for the board and hoping very much that the key dashboards are all in the green. 

The problem with such dashboards is the age-old one of Garbage In, Garbage Out. The predictions are only as good as the data they are based on. Unfortunately, the data are not always good, because by and large, sales reps – and I’ve known a few, good, bad, and indifferent – do not particularly enjoy documenting everything they do for someone else. That last clause is important; the good sales reps take a lot of notes and know all sorts of details about their accounts and territories, but the notes are for their own consumption, and the way they are taken and stored make them hard to access. Sometimes this is even by design, especially among “relationship” sales people who see their value mainly in terms of the thickness of their Rolodex[^1]: “if you fire me, I’ll walk and take all my customers with me!”.

![](/images/unknown_filename.203.png)

We all know how well that play worked out for Tom Cruise’s character in *Jerry Maguire*. Regardless, getting the input data is a very real problem. This is why I am much more interested in the second half of that example scenario from Salesforce:

> They can also easily update Salesforce records after a meeting.

Updating opportunities is already pretty easy from the Salesforce mobile app, but sales managers and Sales Ops types have a tendency to over-complicate the process by adding supplementary required fields which must be filled in to save the simple text-based notes and contact info which are the most valuable parts of the process. Added friction in the data-entry stage leads to opportunity details being added in a rush at the end of the quarter, ret-conning against the ultimate outcome of the opportunity rather than documenting facts in near real time.

Adding support for other technologies on the input side has the potential to remove much of that friction. Siri would let reps have a good rant in the car on the way back from the meeting and transcribe all of that into the activity record. Location data would enter the correct office where a meeting was held. Integration with office suites and cloud storage could add the collateral used in a meeting to the opportunity. Each addition of intelligence on the input side would remove a small amount of friction from the opportunity management process, which in turn would help to ensure that the data which all the fancy analyses are based on are at least somewhat factual.

I have no doubt that most of the videos and presentations around the Apple-Salesforce joint technology developments will focus on showing magical *Minority Report*[^2] dashboards, updating in real time, and smiling managers happy with the results being displayed. However, if any of those whiz-bang dashboards are to have utility in the real world, it will be down to the input capabilities in the individual sales reps’ iPhone and Apple Watch, and the technology’s removal of as many excuses as possible not to update Salesforce records.

[^1]: Yes, Rolodex; that’s how dated this way of thinking is.

[^2]: I think I owe Tom Cruise royalties for this article. How much is 50% of no dollars whatsoever, again? I’m sure he doesn’t mind appearing here [for the exposure](https://twitter.com/forexposure_txt), though.

