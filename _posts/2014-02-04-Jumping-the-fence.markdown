---
layout: post
title:  Jumping the fence 
date:   2014-02-04 
categories:  iPhone tech geography Facebook 
---

# Jumping the fence


Facebook just released their new iPhone client, an app called [Paper](https://www.facebook.com/paper). It’s quite nice, and gets [good](http://techcrunch.com/2014/02/03/paper-now-available-for-ios-in-the-us-and-it-could-be-a-facebook-replacement/) [reviews](http://www.theatlantic.com/technology/archive/2014/02/the-quiet-upheaval-of-facebooks-new-iphone-app/283477/). 

Bit of a jerk move on the name, mind.

![](/images/tweet-430474352984092672.png)

If you are in the US, you can just [download Facebook Paper][fbp], but if you’re in the rest of the world, you’re out of luck.

Or are you?

There are a few different unofficial ways to get apps onto an iPhone, bypassing these sorts of geographical restrictions: **sideloading**, **changing the country** on your existing iTunes account, or **creating a whole new Apple ID** from scratch.[^1]

# Sideloading

*Sideloading*[^2] means that you install the app from your computer, but without going through iTunes. You will need to have access to the actual app file, so you will need a co-conspirator in the US to get you the app. Your confederate can find these as `.ipa` files in the `iTunes Media/Mobile Applications` subdirectory of their main iTunes directory. 

Once you have the relevant `.ipa` file, you can use the [iPhone Configuration Utility](http://support.apple.com/downloads/#iphone%20configuration%20utility)[^3] to load the app onto your phone. Once you’ve done this, the app should behave normally, including for updates.

# Changing the country

You can change the country of an existing iTunes account quite easily: open the App Store app, scroll all the way to the bottom of the “Featured" tab, tap on your Apple ID, choose “View Apple ID” in the popup, and tap on “Country/Region” to change to the US store.

![](/images/6ccb76a3c4637c995901e9f7571b6497.png)

There is a pretty big downside to this method: your payment details will be reset, which would not be too bad, except that it also loses any recurring subscriptions you have set up. I have a few that I didn’t want to mess this, so I didn’t follow through, and can’t vouch that this method works.

# Creating a new Apple ID

I didn’t want to do this because it seemed like it would be a huge hassle, but it’s actually fairly painless. There is only one wrinkle to be aware of. Apple in their wisdom will not let you create an Apple ID from scratch without setting a means of payment. However, if you sign out from your existing Apple ID, then go to install a free app (such as, oh for instance [Facebook Paper][fbp]), you are prompted to log in with an existing Apple ID or create a new one. If you start the process this way, you will then be able to select “None” for your method of payment.

![](/images/unknown_filename.199.jpeg)

You’ll need an e-mail address that you have not previously used with Apple to complete the registration. Once you have done this, finish downloading Facebook Paper, then log out of your US account and log back in as yourself. 

Facebook Paper should pick up your existing FB credentials saved in iOS and work normally from this point on.

[^1]: Well, or move physically to another country, but that’s a bit beyond the scope of this post. 
[^2]: This is the method I used to load Google+ onto my iPad back when it was iPhone only. Remember when we were all excited about G+?
[^3]: This page is not really up to Apple’s usual standards: all-lower-case title for a start, and a confusing mix of version numbers and platforms all jumbled together with no explanation.

[fbp]: https://itunes.apple.com/us/app/paper-stories-from-facebook/id794163692

     