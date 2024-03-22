---
layout: post
title:  How To Lose Friends and Influence People 
date:   2016-12-15 
categories:  privacy social evernote 
---

# How To Lose Friends and Influence People


I am a huge fan of Evernote. I have used their software for many years, and its many features are key parts of my workflow. I take notes on multiple devices, use tagging to sync between those devices, take snapshots of business cards and let the OCR and the access to LinkedIn sort out the details, annotate images and PDFs, and more.

I should say, I *used* to be a fan of Evernote. They recently made some changes to their privacy policy that have users up in arms. Here is the relevant entry from their changelog:

> Privacy Policy
> 
> January 23, 2017 updates to the October 4, 2016 version:
> 
> We clarified that in building a more personalized Evernote service that can adapt to the way you think and work, a small group of engineers may need to oversee these automated technologies to ensure they are working as intended. Also, we added that we will be using data from other sources to tailor your Evernote experience and explain how you can get more out of your Evernote account. Please see our FAQ for more information on these changes.

[Updates to our legal documents | Evernote](https://evernote.com/legal/changes.php?2017-update#privacy)

This may be fairly inoffensive, but it is worrying to me and to many users. These days, “personalisation" is often code for "gathering data indiscriminately for obscure purposes that may change at any time". This exchange is generally presented as a bargain where users sacrifice (some) privacy to the likes of Google in exchange for free use of their excellent services such as Gmail or Maps.

Evernote's case is different. As a paid app, we users like to assume that we are opting out of that bargain, and paying directly for our services - instead of paying indirectly by authorising Evernote to resell our personal data to advertisers.

In addition, we use Evernote to store data that may be personal, sensitive, or both. Evernote have always had some weasel words in their Privacy Policy about their employees having access to our notes:

* We believe our Terms of Service has been violated and confirmation is required or we otherwise have an obligation to review your account Content as described in our Terms of Service;
* We need to do so for troubleshooting purposes or to maintain and improve the Service;
* Where necessary to protect the rights, property or personal safety of Evernote and its users (including to protect against potential spam, malware or other security concerns); or
* In order to comply with our legal obligations, such as responding to warrants, court orders or other legal process. We vigilantly protect the privacy of your account Content and, whenever we determine it possible, we provide you with notice if we believe we are compelled to comply with a third party’s request for information about your account. Please visit our Information for Authorities page for more information.

So basically, Evernote employees have always had access to our stuff. This part of the privacy policy has not changed substantially, but the changes are worrying (emphasis mine):

* New: Do Evernote Employees Access or Review My Data?
* Old: Do Evernote Employees Access or Review My Notes?

* New: Below are the limited circumstances in which we may need to access or review your account information or Content:
* Old: **As a rule, Evernote employees do not monitor or view your personal information or Content stored in the Service**, but we list below the limited circumstances in which our employees may need to access or review your personal information or account Content:

* New: We need to do so for troubleshooting purposes **or to maintain and improve the Service**;
* Old: We need to do so for troubleshooting purposes;

[Privacy Policy | Evernote](https://evernote.com/legal/privacy.php)
[Privacy Policy - 2017 update](https://evernote.com/legal/privacy.php?2017-update)

![](/images/unknown_filename.162.jpeg)

Now, here is why people are all up in arms. We would like service providers to tread *extremely* carefully when it comes to our personal data, accessing it only when warranted. 2016 has provided plenty of object lessons in why  we are so sensitive; just today I received an email from Yahoo detailing their latest hack. [Yahoo hack: Should I panic? - BBC News](http://www.bbc.com/news/technology-38327169)

In this case, Evernote appear to have made two mistakes. First, they designed and built a new functionality that requires access to users’ personal data and content in order to do… well, it’s not entirely clear *what* they want to do, beyond the fact that it involves machine learning.

Secondly, they completely mis-handled the communication of this change. I mean, they even removed the disclaimer that “As a rule, Evernote employees do not monitor or view your personal information or Content stored in the Service”! How tone-deaf can you get?

It’s also very unclear why they even made this change. In their response to the outrage, they say this:

> We believe we can make our users even more productive with technologies such as machine learning that will allow you to automate functions you now have to do manually, like creating to-do lists or putting together travel itineraries.

[A Note From Chris O’Neill about Evernote’s Privacy Policy](https://blog.evernote.com/blog/2016/12/15/note-chris-oneill-evernotes-privacy-policy/)

The problem is, users are perfectly capable of managing to-do lists and itineraries, and based on an informal sample of Twitter reactions to this new policy, do not see enough value to want to give unknown Evernote employees access to their data.

## An unforced error

This is such a short-sighted decision by Evernote. As one of the few cloud services which is used primarily through fat clients, Evernote is in a privileged position when it comes to pushing processing out to the users’ devices. 

Apple have the same advantage, and do the right thing with it: instead of snooping around in my mail and calendar on the server side, my local Mail app can detect dates in messages and offer to create appointments in Calendar. Also, CloudKit’s sync services are encrypted, so nobody at Apple has access to my data - not even if law enforcement asks.

Evernote have chosen not to take that approach, and have not (yet) clarified any benefit that they expect or promise to deliver by doing so. This mis-step has now caused loyal, *paying* users like me to re-evaluate everything else about the service. At this point, even cancelling the new machine-learning service would not be enough to mollify users; nothing short of a new and explicit commitment to complete encryption of user data - including from Evernote employees! - would suffice.

## Evernote's loss will be someone else’s gain

One possible winner from this whole mess is Bear, a new note-taking app that does use CloudKit and therefore is able to provide that encryption at rest that Evernote does not.

[Bear - Notes for iPhone, iPad and Mac](http://www.bear-writer.com)

The Bear team have even been having some fun on Twitter at Evernote’s expense:

![](/images/tweet-809079850837413888.png)

I composed this post in Bear, and I have to say, it is very nice. I copied it over to Evernote to publish here, but it’s the first crack. Before this mess, I was a vocal advocate of Evernote. Now? I am actively evaluating alternatives. 

Respect your users, yo.

