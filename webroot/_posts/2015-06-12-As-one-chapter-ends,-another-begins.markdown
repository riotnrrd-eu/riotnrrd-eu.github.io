---
layout: post
title:  As one chapter ends, another begins 
date:   2015-06-12 
categories:  bladelogic hp BMC Opsware 
---

# As one chapter ends, another begins


I haven’t blogged in ages - which is a *good* thing, I hasten to add! It’s just that I have been drinking from the firehose at my new gig. It’s now more than a month since I started at Moogsoft, and I think I can begin to talk about what it all means. 

I joined Moogsoft from BMC, but it’s important to note that I did not *join* BMC, I wound up there as part of the BladeLogic acquisition. BladeLogic was my first startup, and it was a huge amount of fun, a great learning experience, and probably my period of fastest professional development to date. Before BladeLogic I was at [Mercury](https://en.wikipedia.org/wiki/Mercury_Interactive), but I quit to join BladeLogic, due in no small part to the acquisition by HP[^1]. 

# What is BladeLogic?

Both BladeLogic[^2] Operations Manager (BLOM) and Incident.MOOG are innovative products in their place and time.  BladeLogic, together with Opsware, redefined what server configuration management meant, and both companies went on to be acquired by larger “Big 4” IT vendors: Opsware by HP, and a year or so later, BladeLogic by BMC. 

For a while both products thrived in their new environment, but in the last few years, both have been flagging. There are many reasons for this, from internal politics at both BMC and HP acting as distraction, to the rise of open-source configuration management tools such as Chef and Puppet. However, I wonder if those tools were simply the end of an era. 

This is a known pattern: technologies reach their peak right before they get displaced by their successor technologies. [The speed record for steam engines was set in 1938](https://en.wikipedia.org/wiki/LNER_Class_A4_4468_Mallard#Record), but [a diesel engine had already exceeded that speed in 1936](https://en.wikipedia.org/wiki/DRG_Class_SVT_137), and by the 1950s [diesel locomotives were well on track to replace steam traction](
https://en.wikipedia.org/wiki/Diesel_locomotive#History)[^3]. 

This pattern even agrees with disruption theory: investment continues in the old technology, but it simply becomes overly complex and uneconomical compared to simpler, (initially) low-end competitors. 

# Pets vs Cattle

This disruption is exactly what I see happening now. The BladeLogic model of painstaking management of single servers is still relevant, but mainly for legacy or specialised systems. Much new-build development is already moving to disposable or even stateless VMs or containers, according to the classic “pets vs cattle” model. 

 ![](/images/unknown_filename.42.jpeg) 

In this brave new world, there is very little need to worry about the configuration of your “cattle” containers. Something like BladeLogic is arguably overkill, and users should instead focus on their provisioning process. 

Of course it’s not quite as simple as that. Cloud zealots have been talking about replaceable short-lived cloud servers for a while, but it hasn’t really happened outside of some rather specific situations. The lifetime of VMs in the cloud has often ended up being much longer than this model would suggest, meaning that there is plenty of time for their configurations to drift and to require management in place. Part of the reason for this is that management processes and techniques that are still based on the paradigm of a persistent physical server. Much of this Weltanschauung has been adopted wholesale for virtual and cloud-based servers without much reconsideration. 

There is also the topic of security and policy compliance to be considered. Given long system lifetimes, it is not sufficient to be able to validate that something was *deployed* correctly, as its configuration may have drifted away from that known-good state. The desired state may also change as vendors release updates and patches, or new security vulnerabilities are disclosed. In all of these cases, some mechanism is needed to check for differences between the current live configuration and the required configuration, and to bring the system into compliance with that desired state. 

However, this is now. As Docker and other container-centric infrastructure technologies become more prevalent, and as business functions continue to migrate from legacy to new-build applications, I would expect that that paradigm will evolve to replaceable plug&play infrastructure components, and do so everywhere, not just at the “unicorn” companies. 

# What does it all mean?

Lots of smart people are working hard to enable infrastructure to be managed as code. One of the characteristics of code is that you don’t change it in production, you develop it offline, then release it and don’t change it until you overwrite with a new version. The big variables that I think will affect the speed of the transition to this new model are firstly, the rate of replacement of legacy applications, and secondly, the evolution of IT management processes and culture to take advantage of new tools.

BladeLogic itself has the opportunity to evolve to have a role in the new model, of course. Regardless, BladeLogic was a huge part of my career development - and just huge fun, if I’m honest - so I will be watching development of the IT infrastructure management market intently, but no longer from the front lines.

[^1]: I’d say my fears on that score have been amply borne out.
[^2]: The Wikipedia entry for BladeLogic now redirects to BMC, which is not especially helpful.
[^3]: Sorry - not sorry.

