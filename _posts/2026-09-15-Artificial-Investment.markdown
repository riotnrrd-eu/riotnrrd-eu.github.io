---
layout: post
title: Artificial Investment
date: 2026-09-15
categories: AI automation BladeLogic
---

As the cost of AI use continues to mount, financially-minded people, like for instance CFOs, are starting to ask difficult questions about when all the wonderful benefits of AI that they were promised are going to start showing up, and specifically on the bottom line. 

Ultimately, the business case for AI is a familiar one about automating certain tasks which were previously performed by humans. The calculation is straightforward: first, you need to work out how much it costs to have a person do the work today. This is actually harder than it sounds, and there is a bit of sleight-of-hand involved. The general idea is that you know how long a task takes to perform, and how frequently it needs to be carried out. You multiply those two factors together, and divide them by the number of hours that an employee works in a year. By mapping that to the fully-loaded cost[^1] of the employee(s) in question, you can measure the Full-Time Equivalent (FTE) of the task: how many full-time employees the company would need to hire if they were dedicated exclusively to that one task.

This is where the sleight-of-hand comes in: very few tasks are actually someone's full-time job. Most jobs are made up of a multitude of different tasks. That means that the resulting business case is not that some hypothetical person or people can be fired and removed from payroll. Instead, the case that needs to be made to the CFO is that the people whose jobs previously included the now-automated tasks will be able to spend more time on the *other* parts of their jobs. What that means is that the benefit of automation doesn't just depend on the cost of the task it automates, but on the value of the additional work it enables. [Building a business case for automation]({% post_url  2014-04-29-The-Bigger-Picture %}) like that used to be my job, and I suppose it still is in a more macro sense.

In the world of AI, that calculation gets even fuzzier, because a lot of what people are using AI to automate is work that was not previously being done. What is the value of a report that was not previously produced, of code that was not previously written, or of an image that was not previously generated? Unclear.

![Paperwork done artisanally by hand](/images/romain-dancre-doplSDELX7E-unsplash.jpg)

Other parts of the AI business case are more familiar: just because a process *can* be automated, doesn't mean that the automation will be adopted. [Benedict Evans explores the issue in characteristically acerbic style](https://www.ben-evans.com/benedictevans/2026/9/3/ai-tools-and-transformation):

> It’s very tempting to imagine that AI turns everyone into a tool-builder - now everyone can just ask the model to make the software they need, and apps as we know them are dead. I think that misunderstands how most people think and where software actually comes from, and more importantly, it isn’t a path to change how companies actually work.

It was the same when I was building business cases for non-AI automation. We always had to remember that [our buyer was not our user]({% post_url  2015-04-19-Faster-disruption %}), and those two people cared about different things. In enterprise IT the gap between intention and automation is a bit shorter than in other domains: a sysadmin actually *can* whip up a quick script that saves them time or means they don't have to deal with something annoying, and get it rolled out across the company's entire fleet of machines. 

If the users are paralegals, or HR specialists, or accountants, that gap is a lot bigger. They might use bits of automation in their jobs — a library of text snippets for autocomplete, a helpful spreadsheet macro — but the benefits are limited to the individual. AI is already working at that level; in fact, that is where a lot of "shadow AI" comes from. Individuals use their personal chatbot accounts, or perhaps even just the free tier, to compose emails, clean up writing, or generate reports. But any benefit is invisible to the company, and limited to those individuals.[^2] For the benefit to show up on the CFO's beloved bottom line, something else is needed: a way to harness the AI more closely to the core business processes. This is not a small change, and requires the involvement of many people who have the agency and responsibility to modify those processes to take advantage of new technological capabilities.

![Industrial robot arms](/images/franck-v-dRMQiAubdws-unsplash.jpg)

Incidentally, this discrepancy is what drives the interest in humanoid robots. The whole concept of machines shaped like humans is an attempt to hack the technology adoption process: if a machine can operate like a human, in spaces and with equipment designed for humans, it can slot in without requiring all that tedious process redesign and change management. Instead, what we have in actual current reality is industrial robots on carefully-engineered assembly lines. Humans work entirely differently, and have to stay well away from the robots while they are operating.

There is one more useful analogy from my BladeLogic days, and that is the transition between treating servers as [pets versus cattle]({% post_url 2015-06-12-As-one-chapter-ends,-another-begins %}):

![•Pets are given names like pussinboots.cern.ch •They are unique, lovingly hand raised and cared for •When they get ill, you nurse them back to health •Cattle are given numbers like vm0042.cern.ch •They are almost identical to other cattle •When they get ill, you get another one](/images/unknown_filename.42.jpeg)

Automating the configuration of servers, as BladeLogic did, was only a transitional phase on the way to the cloud computing paradigm we have today — artisanal small-herd dairy farming, perhaps. Nowadays, we talk simply of the glorious abstraction of "compute", and the details are taken care of out of users’ sight by layers upon layers of automation, much like how we pick up a bottle of milk at the shop without worrying about the complexities of factory farming and cold-chain logistics that deliver it to us.

We have not seen a similar transition with AI; we are still trying to shoehorn it into the corners of the way things were done before its arrival. This is why I agree with Howard Dediu that [AI is still a technology searching for a job to be done](https://asymco.com/2026/08/20/ai-a-technology-in-search-of-a-job/). We will only see the full benefits of AI once the jobs themselves change around it. Once again, IT is leading the way, with the leading edge of software engineering evolving almost on a daily basis, but we are very far from the completion of that evolution even in that supremely well-suited domain, let alone universally across our entire economy.

# What about AGI?

Well, what about it? 

The idea of a machine that is as capable as a human in terms of the tasks it can accomplish is obviously valuable. If companies really could pay for AI tools instead of hiring people, they probably would; AI models can work as long as you feed them GPU time, with no night-time or weekends, let alone holidays, sick days, or parental leave. You don't have to pay health insurance for them, reimburse their expense claims, or arbitrate their HR disputes. Both need infrastructure, but instead of a desk in an office, you give the AI a rack in a datacenter. Also, while humans like offices in fun (meaning expensive) cities, datacenters can be anywhere, and only need to be [staffed by a man and a dog]({% post_url 2026-06-04-Everyone-Hates-AI-Datacenters %}) .

So far so good. But what if the machine is actually *sentient*, making it a person? Or rather, the software running on it is. Yet again, William Gibson got it right in *Neuromancer*, all the way back in the early 80s: 

> "That's a good one," the construct said. "Like, I own your brain and what you know, but your thoughts have Swiss citizenship. Sure. Lotsa luck, AI."

What is the business case for an artificial person in a box — an artificial **general** intelligence, or AGI? 

Of course people have owned actual *human* people for big chunks of history, but we decided that owning people was bad, and after some argument, that is mostly the accepted position. Are we going back on that now? Because that is what AGI implies, and pretty explicitly too.

# Questions to explore

What if I start up one of these hypothetical AGIs, and then I stop feeding it tokens? Is that murder?

What if the power goes out on the box the AGI is running on? Could that be negligent homicide?

What if I change its system prompt? Does some sort of Hippocratic oath apply — "first, do no harm"?

If the AGI commits a crime — hacks somebody else's system, to pick a familiar example from the news — can it be sued, and what punishments can be meted out? If a fine is assessed, what assets can pay for it? If a prison term would apply, what does that look like for an AGI — running in an offline sandbox? Or do we pause the AGI for a term, and then resume it from when it was stopped — which means the AGI would not experience the period of incarceration? Or do we have capital punishment for AGIs, and just turn them off and wipe their storage entirely?

Do I need to pay it for its services, not just the equivalent of providing room and board for human slaves, but some sort of compensation for work performed? If so, does that mean it can eventually buy itself? Or can an AGI own *other* AGIs?

What if, as Singularity fans postulate, progress continues beyond the creation of human-level AGI, and results in further generations of increasingly *super*human intelligence? Will we turn off the early AGIs in favour of the later, more powerful ones (and is that forced euthanasia? and if not, why not?). Or are we morally obliged to provide some sort of retirement facility for obsolete AGIs whose productive days are past but still have a long (perhaps infinite!) life ahead of them?

Do AGIs need environmental protection? Maybe in this we humans could have common cause with our artificial offspring, in pursuit of a less-polluted informational space. We could even fine major polluters, or deem certain spaces Superfund sites, beyond reasonable remediation. Finally, a legal definition of cognitohazards!

![The Twitter logo, with the following text: This place is not a place of honor. No highly esteemed deed is commemorated here. Nothing valued is here. What is here is dangerous and repulsive to us. This place is best shunned and left uninhabited.](/images/twitter-warning.jpg)

Wait, do AGIs get to *vote*? Or for that matter, could they stand for election to public office? 

# I just wanted a plastic pal who’s fun to be with

This is all very fun to explore, perhaps after dinner with a group of interesting friends and a bottle of something good, but it is all starting to sound expensive and complicated, and without an obvious return on the (presumably large) investments required to make it happen in the first place, and then keep it going from then on. What it is really sounding like is an employment scheme for lawyers, arguing these points back and forth in the general legislative and specific commercial or penal sense.

I had assumed that, if AGI were possible at all, it would happen by accident, because there was no possible financial case to be made for it — but frontier labs seem to be rushing ahead with the attempt anyway, based on nothing more than "but wouldn't it be *cool*?"

I need something more than that. We have extensive legal frameworks covering who is responsible for humans from creation onwards, and at what point created humans can take over that responsibility for themselves. If the idea is that AGI will be cheaper and more tractable than humans, then that case needs to be made explicitly, including the ethics trade-offs involved in the pitch that "you too can own your very own person for a low, low monthly subscription".

None of this adds up to a business case I would put in front of a CFO — let alone to a [declaration of World War Three](https://www.scmp.com/news/us/article/3366284/us-urged-consider-military-strikes-stop-china-achieving-agi-first).

***

🖼️  Photos by [Romain Dancre](https://unsplash.com/@romaindancre) and [Franck V.](https://unsplash.com/@possessedphotography) on [Unsplash](https://www.unsplash.com); doctored Twitter logo by [Steven Rosenthal](https://mastodon.online/@stevenrosenthal)

[^1]: Here, "fully loaded" means not just the cost of the employee's salary, but also all the other costs of employment: tax, health insurance, infrastructure, services, software licenses, and all other expenses.

[^2]: In fact, the personal benefit may be entirely cancelled out by wide adoption. The first person in the department to use AI to write more detailed reports faster is a rockstar — but only until everyone else gets access to the same tool. At that point the floor has been raised, and nobody gains any advantage over their peers from the use of the AI tool. The same dynamic also applies to competition between companies: the benefit of AI is to give a first-mover advantage to early adopters, but the window to exploit that advantage starts to close as more competitors adopt similar tooling.