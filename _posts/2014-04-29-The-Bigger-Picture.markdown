---
layout: post
title:  The Bigger Picture 
date:   2014-04-29 
categories:  bladelogic tech 
---

## The Bigger Picture
## Or, Why BladeLogic Isn’t Puppet

***Disclaimer:*** *In case you don’t know already, I work for BMC Software, having joined with the acquisition of BladeLogic. My current role is in marketing for BMC’s cloud computing and data center automation products, including BladeLogic. In other words, if you are looking for a 100% objective take, look elsewhere. The reason this piece is here rather than on a bmc.com site is to make it clear that this is personal opinion, not official corporate communication.*  

At the turn of the last century, life as a sysadmin was nasty and brutish. Your choice was either to spend a lot of time doing the same few things by hand, generally at the command line, or to spend a lot of time writing scripts to automate those tasks, and then even more time maintaining the scripts, all the while being interrupted to do those same things.  

Then along came two automation frameworks, Opsware and BladeLogic, that promised to make everything better. The two tools had somewhat similar origin stories: both were based around cores that came out of the hosting world, and both then built substantial frameworks around those cores. In the end both were bought by larger players, Opsware by HP, and BladeLogic by BMC.  

BladeLogic and Opsware both let sysadmins automate common tasks without scripting, execute actions against multiple servers at once, and assemble sub-tasks together to do full-stack provisioning. There were (and are) any number of differences in approach, many of which can still be traced back to the very beginnings of the two companies, but it’s safe to say that they are the two most similar tools in today’s automation marketplace.  

Yes, *marketplace*. Because in the last decade or so a huge number of automation tools have emerged (or matured to the point of usefulness), mainly in the open-source arena. If you are managing tons of OSS Linux boxes, running an OSS application stack, it makes sense to have an OSS config management tool as well.  

So far, so good. For a while the OSS tools flew under the radar of the big vendors, since the sorts of people willing to download a free tool and hack Ruby to do anything with it tended not to be the same sorts of people with the six- or seven-figure budgets for the big-vendor tools. As is the way of such things, though, the two markets started to overlap, and people started to ask why one tool was free and the other was expensive. This all came to a head when Puppet Labs published a document entitled ["Puppet Enterprise vs BMC BladeLogic"](https://puppetlabs.com/sites/default/files/Puppet_Enterprise_vs_BladeLogic.pdf). Matthew Zito from BMC responded with [An Open Letter to PuppetLabs](https://communities.bmc.com/community/bmcdn/bmc_service_automation/server_configuration_automation_bladelogic/blog/2014/04/28/an-open-letter-to-puppetlabs) on BMC’s site, which led to an exchange on Twitter, storified [here](https://storify.com/dwellington/puppet-vs-bladelogic "Puppet vs BladeLogic · dwellington · Storify").  

### This is the longer response I promised Luke Kanies.  

When I was at BladeLogic, I was in pre-sales, and one of my jobs (on top of the usual things like demos, proof-of-concept activities, and RfI/RfP responses) was to help the sales people assemble the business case for buying BladeLogic. This usually meant identifying a particular activity, measuring how much time and effort it took to complete without BladeLogic, and then proposing savings through the use of BladeLogic. Because *for some unknown reason* prospective customers don’t take vendors’ word for these sorts of claims, we would then arrange to prove our estimates on some mutually-agreed subset of the measured activities.  

We would typically begin by talking to the sysadmins and people in related teams. They had generally spent a lot of time scripting, automating and streamlining, and were eager to tell us that there was no reason to buy what we were selling, because there were no further savings to be made. Any requests could be delivered in minutes.  

The interesting thing is, we would then go around the corner to the users and ask them how long they typically had to wait for requested services to be delivered. The answers varied, but generally in the range of, not minutes, but two to eight *weeks*.  

### *Weeks*, not minutes

Where is that huge discrepancy coming from? Because, depressingly, it’s still the same today, a decade later.  

The delay experienced by users is not caused by the fact that sysadmins are frantically flailing away at the keyboard for a full month to deliver something. Credit us sysadmins (for I am still one at heart) with a bit more sense than that. No, the problem is that there are many many different people, functions and teams involved in delivering something to users. Even if each individual *step* is automated and streamlined and standardised to within epsilon of perfection, the overall *process* is delayed by the hand-offs between the steps, and even more so when the hand-off isn’t clean and something needs to be reworked, or worse, discussed and argued about.  

**That** is the difference between Puppet and BladeLogic. Puppet is trying to address one - or, in all fairness, *several* - of those steps, but BladeLogic is trying to address the entire *process*.  

In a wider sense, this is what BMC is trying to do for all of enterprise IT. "Consumerisation of IT" has become a cliché, but it’s true that in the same way that Puppet has moved from a hobbyist market to the IT mainstream, Dropbox has moved from a home user market to a corporate one, AWS has eaten the cloud, and so on. We are living in a Cambrian explosion of tools and services.  

Enterprise IT departments and the vendors that serve them cannot compete with these tools, and nor should they. The models of the new entrants give them economies - of scale, of attention, of access - that the traditional model cannot touch. The role for enterprise IT is to provide *governance* across the top of this extremely diverse and rapidly evolving ecosystem, and fill in the gaps between those tools so that we deliver the correct end product on time, on spec and on budget[^1].  

Sure, use Puppet - and Chef, and Ansible, and SaltStack, and CFEngine, and your home-grown scripts, and maybe even BladeLogic’s BLpackages. Just make sure that you are using them in a way that makes sense, and that meets the users’ needs. At the end of the day, that’s what we are all here for.

[^1]: Yes, all three. The point of automation is to resolve that dilemma.