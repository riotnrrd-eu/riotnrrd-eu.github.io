---
layout: post
title:  On the humble URL 
date:   2014-05-14 
categories:  tech web 
---

# On the humble URL


I'm very late to the story, but I have some thoughts on the topic of [URLs going away](http://www.nczonline.net/blog/2014/05/06/urls-are-already-dead/ "URLs are already dead" ). Basically, the latest builds of Chrome no longer show the URL at all, following along with a trend which started with Safari on iOS7 hiding everything beyond the site itself by default.  

The thing is, civilians have been using the web this way for ages. Few people type URLs or even truly understand how the things work. This resistance is not limited to HTTP, either. One of my pet peeves is the existence of services like Hightail (YouSendIt) or WeTransfer. Neither really does anything different from FTP, at least the way I see them used. If you ask users of these services, though - and I happen to have one handy in my house - they will tell you that FTP is "too complicated", requiring logins and thinking about complex navigation and permissions.  

<div style="background-color:#fff;display:inline-block;font-family:'Helvetica Neue',Arial,sans-serif;color:#a7a7a7;font-size:11px;"><iframe src="//embed.gettyimages.com/embed/75407052?et=sXuoGjOTR1t2sMJoOECfzQ&sig=nK7tQ6jhAnDMUJr09VGgthGjQriDNyu818OI2KLYYJQ=" width="398" height="648" scrolling="no" frameborder="0" style="display:inline-block;"></iframe><p style="margin:0;"></p><div style="padding:0;margin:-6px 0 4px 10px;text-align:left;"><a href="<http://www.gettyimages.com/detail/75407052>" target="_blank" style="color:#a7a7a7;text-decoration:none;font-weight:normal !important;border:none;">#75407052</a> / <a href="<http://www.gettyimages.com>" target="_blank" style="color:#a7a7a7;text-decoration:none;font-weight:normal !important;border:none;">[gettyimages.com](http://gettyimages.com)</a></div></div>  

To me, writing out an FTP URL like `ftp://username@hostname/directory/file.ext` seems perfectly obvious and natural. When a user receives that URL through email or whatever other mechanism, they can click on it and be taken directly to the file.  

The problem is that while I have *sent* many URLs like that, I can count the number of times I have *received* a URL formatted that way on the fingers of one hand. URLs seem obvious to me because I'm used to thinking of paths that way, but Muggles don't think that way, and don't want to. WeTransfer hides the scary details, and that's what they want.  

My hope is actually that this move leads to the return of separate address and search fields, with the address field hidden by default. That way I could turn the address field back on, and finally be able to connect to `hostname` on my local LAN instead of being sent to a Google search for "hostname".

