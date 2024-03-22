---
layout: post
title:  Don't Blame The User 
date:   2019-07-16 
categories:  security 
---

# Don't Blame The User


It would be easy to write a blog post about every single XKCD strip, so I try not to – but [the latest one](https://xkcd.com/2176/) drives at something very interesting in infosec.

![](/images/unknown_filename.101.png)

Some of the default infosec advice that is always given out is to avoid reusing passwords on different sites. This is good advice as far as it goes, but it misses one key aspect. Too many sites force people to create accounts for no good reason (“create an account to use our free wifi”), and so people use throwaway passwords, and reuse them across many of these low-risk sites. In the XKCD example above, if someone cracks the Smash Mouth message boards, maybe they get to reuse the password to gain access to the Limp Bizkit boards, but ideally they won’t get access to Venmo, because that not only has a different, higher-grade password, but is also secured by 2FA[^1].

The good news is that it’s becoming easier than ever to generate secure passwords and avoid reusing them. If you’re an Apple user, the iCloud Keychain is built right into both iOS and macOS, and will generate and remember secure passwords for you, securing them with FaceID or TouchID. There are of course any number of third-party options as well, but the point is that security needs to be *easy*. People who care about security will sign up for [Have I Been Pwned](https://haveibeenpwned.com); general users just trying to get through their day will not.

The first priority is making it work at all, the second is making it usable; regrettable as it may be, security comes after those primary concerns. The easier it is for users to do the right thing, the more likely it is that they will do it. Browbeating them after a breach because they didn’t jump through precisely the right hoops in exactly the right sequence is not helpful. What will help is putting the effort into helping them up front, including in the service design itself.

[Previously]({% post_url 2016-05-24-Security-AND-Usability %}), [previously]({% post_url 2015-01-29-Password-to-the-Ivory-Tower %}).

[^1]: Note, I have no idea whether Venmo actually supports 2FA; not being in the US, I don’t / can’t use it. For “Venmo”, read “online banking” or whatever other high-security example.

