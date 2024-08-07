---
layout: post
title:  Security AND Usability 
date:   2016-05-24 
categories:  security 
---

# Security AND Usability


## Sure, blame the user

![](/images/unknown_filename.295.png)

Because there isn’t enough *recent* security news, everyone is all worked up about the [2012 LinkedIn breach](http://www.theregister.co.uk/2016/05/24/linkedin_password_leak_hack_crack/ "LinkedIn mass hack reveals ... yup, you're all still crap at passwords” ). Okay, it’s somewhat newsworthy because some lowlife is now trying to sell the data. All the security vendors have jumped on the bandwagon[^1], but in particular lots of people are mocking the fact that people are using common or easily-guessed passwords:

- 123456
- linkedin
- password
- 123456789
- 12345678

Now a bot has emerged which attempts to reuse known leaked passwords to log in to sensitive sites such as online banking systems. Predictably, the main response has been mockery, with El Reg opining that [If your Netflix password is your banking password, you'll get what you deserve](http://www.theregister.co.uk/2016/05/24/password_reuse_bot_steals_creds_from_crap_sites_logs_in_to_banks/ "Password reuse bot steals creds from weak sites, logs in to banks” ).

This sort of victim-blaming has got to stop. It may be fun in an elitist, look-at-the-lusers sort of way, but it’s not actually advancing the cause of better security. 

Obviously the real villains of the piece are the people exploiting those credentials, but those sorts of people are probably going to be with us until the ultimate heat death of the Universe, so blaming them is not a particularly productive exercise. Law enforcement could and should do more to bring the perps to justice, but that can only ever happen after the fact, when it’s too late for the victims.

Among people we can actually expect to influence, I would start with the banks. Given that people are out there trying to break into banking systems, [because that's where the money is](https://en.wikipedia.org/wiki/Sutton%27s_law ), and given the potential consequences of a breach, the design of those systems must include more advanced security than a simple username and password pair.

For reasons too complicated and boring to relate, I actually have two bank accounts with different institutions in different countries. Both, however, implement two-factor authentication. One has a challenge-response device that works with my ATM card, while the other requires me to make a call from my registered phone number and enter a one-time code. Any bank not implementing something along those lines in 2016 is negligent with their customers’ security. If your bank does not offer two-factor authentication, you should run, not walk, to the exits.

## But what about the (l)users?

Users certainly bear some responsibility for not sharing passwords - but in the real world, there are already far too many services that require me to create an account with a username and a password for no good reason. Log in to comment, log in to review, log in to purchase, log in to make a reservation… No wonder people share passwords between services!

It’s fine to sit in the [ivory tower of security policy]({% post_url 2015-01-29-Password-to-the-Ivory-Tower %}) and blame people for doing this sort of thing, but it’s the reality. At least nowadays most places accept an email address as the user account, so that’s one thing less to remember - without worrying about whether this particular site right here wanted a username of less than eight characters, exactly eight characters, or more than eight characters, or whether somebody had already picked my chosen user name so I made a variant, or whatever.

Passwords themselves are still a problem, though. Logging in via Google, Facebook or Twitter is becoming more common, but there the issue is that I don’t necessarily *want* to share my social ID with every random website that I need to have a one-time interaction with.

The result is that I reuse passwords for unimportant services *all the time*. However, all the important ones are unique - including my LinkedIn password, since my old one was caught up in that 2012 breach. Security needs to be done in layers. If someone gets my Random Website password, that won’t get them into my LinkedIn - and if they get my (new) LinkedIn creds, that still won’t get them anywhere with my online banking.

And here’s a pro tip - for all those one-time, "log in to use our wifi"-type deals, just do like my good friend Annie Onymous, who is always happy to share her email address: ann.onymous@myo.biz.

Stay safe out there.

[^1]: Not that there’s anything wrong with that *per se*; we all take any opportunity to link our wares to current affairs. What I’m objecting to here is the wrong-headed thinking that is exposed in the rush.

             