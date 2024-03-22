---
layout: post
title:  Protect the base 
date:   2014-02-26 
categories:  tech google 
---

# Protect the base


An interesting [story](http://techland.time.com/2014/02/25/gmail-unsubscribe/) in the news today is about Gmail adding an “unsubscribe” link to marketing e-mails. Of course this is not exactly a new feature, having [first launched in 2009](http://gmailblog.blogspot.com/2009/07/unsubscribing-made-easy.html).

Some of the commentary about why Google is doing this seems to me a bit misguided. Someone from Slate on Monocle’s [The Briefing](http://monocle.com/radio/shows/the-briefing/) (sorry, missed the name) characterised this move as Google trying to make Gmail more useful for users and therefore more sticky. 

I think the *actual* reason Google is doing this is to reduce or even eliminate a channel marketers can use to connect with consumers without going through Google. Subscribing to e-mail updates is a direct connection between consumers and brands. Google would rather be the middleman in that transaction, selling AdWords to brands and collecting a toll on all the traffic.

What makes me fairly certain of this analysis is that Gmail’s unsubscribe feature relies on the sender including the `list-unsubscribe` header as per [RFC 2369](http://www.ietf.org/rfc/rfc2369.txt), so it won’t help with spam or with dodgy marketing e-mails in general, only with entirely legitimate and technically correct marketing communications.

I’m not on Team “Everything Google does is evil!”, but that doesn’t stop me from taking a clear-eyed look at what they do.

