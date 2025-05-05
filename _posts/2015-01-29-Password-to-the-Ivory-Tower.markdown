---
layout: post
title:  Password to the Ivory Tower 
date:   2015-01-29 
categories:  security 
---

# Password to the Ivory Tower


My big focus at work lately is the [*SecOps gap*](http://www.bmc.com/blogs/categories/secops-security-compliance/ "SecOps, IT Security & Compliance - BMC Blogs" ), the breakdown in communications between IT Security and Operations groups. The problem here is that the infosec group comes up with some policy that is great in theory, but runs into issues when the poor sysadmins try to apply it. Either the policy is too vague, or it is contradictory, or it would break some application that the line of business depends on, or it is simply too cumbersome and time-consuming to implement properly. 

 ![](/images/unknown_filename.275.jpeg) 

At work I talk about this in the context of enterprise IT, but the exact same thing applies in consumer IT. Case in point: there was recently a breach of Starwood's SPG loyalty programme - see [Brian Kreb's report](https://krebsonsecurity.com/2015/01/password-re-use-fuels-starwood-fraud-spike/ "Password Re-use Fuels Starwood Fraud Spike"). Sure enough, I got an email from SPG entitled "Protect Your Information by Updating Your SPG Password". 

 ![](/images/unknown_filename.274.jpeg) 

SPG should be applauded for being so proactive, and the breach does not seem to be due to any gross negligence on their part. The only thing they might have done differently would be to have more aggressive back-off policies for repeated authentication attempts, but let's not forget that this is a *generalist* site, and one that is probably not used that frequently by most people. Users may legitimately forget their credentials between one login and the next. No, my problem is with Brian Krebs' advice:

> far too many people re-use the same passwords at multiple sites that hold either their credit card information or points that can easily be redeemed for cash. 

Well yes, this is true, and I'm as guilty as anyone - but on the other hand, there are simply **far too many passwords** out there! When every website I visit wants me to create a profile and secure that with a password, of *course* I'm going to reuse those credentials! 

The trick is not to reuse credentials on anything valuable. Don't reuse the credentials for your online banking, for instance - *those* have to be unique. But for every Tom, Dick and Harry who wants a password? They can all get the same one, and that's **if** I don't simply introduce myself as Ann Onymous, with this handy email account at mailinator.com. 

This is why using central login services via Facebook, Twitter or Google is so popular. The problem there is that I don't necessarily want any of that unholy trio tracking my every move, nor do I entirely trust random sites with my Oauth creds, so there's a problem there too. I did like [OpenID](http://openid.net "OpenID" ) as a concept, but it's pretty much dead now in practice. 

### Bottom line

Berating people for poor password security practices won't cut it. We as an industry have to make it easy for people to do the Right Thing, not set up obstacle courses and then point and laugh when people trip over them.

*** 
Image by Keith Misner via [Unsplash](https://unsplash.com)

