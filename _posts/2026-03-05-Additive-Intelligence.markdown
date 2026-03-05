---
layout: post
title:  Additive Intelligence
date:   2026-03-05
categories:  AI work cloud
---

I am not the first to say that we are living through a poorly-written dystopia — but I am not sure everyone realises quite *how* poorly it is written.

The steampunk cliché is that there are individual discrete steam engines everywhere powering every single appliance.

Similarly, the fantasy cliché is that there is magic everywhere (or sometimes magical creatures) applied directly to every single individual task.

And today, the default with “AI” is to have Torment Nexuses, I mean ***LLMs*** all over the place, connected directly to every single endpoint.

We are stuck on this local optimum of everything being a chatbot because ChatGPT was the first GenAI application to break big, so now everything has to follow that exact same pattern.

!["It's time to have a conversation with your data" — source removed to protect the guilty](/images/1730996854628.jpeg)

Nobody who is not utterly deranged wants to "have a conversation with their data" — but we do all have *questions* for our data. The next question is, how do we do that? For instance, SQL queries are by definition questions, and personally I would prefer at least the option of a terse and rigorous syntax sometimes, but most people find the grammar of SQL a little *too* terse and rigorous.

# This is a UX question, not an AI question 

One place where GenAI can be useful is precisely in helping people figure out how to ask those better questions. Today, if you use an enterprise SaaS platform such as Salesforce, you don’t use the out-of-the-box reports and dashboards; you build your own, or you have a Salesforce admin (or a team of them) to build the custom dashboards that you actually use to run your business. Building those dashboards is a specialised skill, requiring a baseline of SQL competence, some specialised Salesforce knowledge, and a good amount of context about how this particular Salesforce instance and sales process are set up. 

Few individual end users have the skills or the access rights to build their own reports — and anyway, not all of the data is in Salesforce! Microsoft remains the number one vendor in business intelligence, not with PowerBI or anything like that, but with good old Excel spreadsheets. And then there are PDFs that come in from outside, and data that was exported in CSV from a different tool, and so on and so forth. 

All of these files go to make up what is called “unstructured data”, to differentiate it from data which is highly structured by definition, living inside databases of various types. The contents of those files are critically important to the operation of the business, but most software tools turn a blind eye to them, because of how difficult and annoying they are to deal with. Now GenAI enables new use cases that incorporate unstructured data directly, without having to first laboriously and lossily apply structure to it.

Now suddenly GenAI makes it feasible for any user to ask questions about **all** their data, spread across structured and unstructured formats, and reconcile it everywhere. That expansion of possibilities doesn’t limit the value of Salesforce as the system of record for the company’s sales operations; if anything, it *enhances* that value by increasing the leverage of that data enormously

In other words, the value of AI-assisted vibe-coding will not be in [building a replacement for the Salesforce platform]({% post_url 2026-02-18-AI-Is-Not-Disruptive %}), but in building more dashboards and ways to understand Salesforce data and cross-reference it with other sources. Sure, it is probably already technically possible to vibe-code up a Salesforce clone — but that is not the value of Salesforce! The software is not particularly sophisticated; it’s basically a front-end for a database.[^1] The value is in everything that has been built around that relatively simple core to turn it into a product.

Expanding that valuable wrapper with GenAI is absolutely transformative, just not in the sort of spectacularly **visible** and in-your-face way that people imagine when they talk about vibe-coding killing SaaS. The winners will not be new discrete products — or maybe they will be lightweight products (thin wrapper apps?) atop whatever becomes the next platform layer.

![A stack of rocks in a forest](/images/fred-robin--ACa2OWKPNk-unsplash.jpg)

# What is the LAMP stack of AI?

In the early days of web apps, it was very difficult even to get to the point where you had all of the infrastructure in place for you to start developing your app. The first wave of dot-com startups had to spend millions of dollars of their seed capital buying hardware from the likes of Sun, Cisco, and Juniper, then spend ages installing and configuring it all, before they could even get to the point of building their app.

Then In the next wave, the industry converged on a few standards which made it easy to build the next layer up where the differentiation and the value were. Virtualisation and then cloud computing made it easy to get the computational capacity. A small number of standard software setups appeared, the most popular of which was LAMP: 

- Linux
- Apache
- MySQL
- PHP

This became a default that, if not quite universal, was common enough that startups could deploy it quickly, find any number of people skilled in working on it, and move on to the parts of the work that they (and their investors and customers) actually cared about.

While the LAMP stack is no longer the ubiquitous standard it once was, the move to cloud computing that it was part of is still rolling. Still today, only around 35% of workflows are in the cloud, depending on who you talk to. Transitions take time, and this one is keeping on rolling; it just doesn’t make the headlines any more. That is the hallmark of a mature technological stack: we don’t talk about the steam engine-driven clockwork mechanisms, or the magical gnomes, but rather about what they enable. A new tool being available "as a service" is not even in the pitch deck.

GenAI has self-evidently not reached that level of ubiquitous maturity yet: it is very much in the headlines and the pitch decks, if indeed it is not the whole things ("X, But With AI!!1!"). There is not yet an obvious LAMP stack of AI that we can all build the Next Big Thing on. In part, this is because one of the notable characteristics of the original LAMP stack is that all the components are open-source; nobody made any money directly by selling them. Some money was made either by packaging the LAMP stack itself and offering it as a service, or by offering consulting around it — but the big money was made further up the stack, by people who built new and valuable products on top of the commoditised LAMP stack. The customers of those products did not have to know or care about how they were built or where they ran; they were in it for the outcome that those technologies enabled.

Right now in AI we are still at the equivalent stage of arguing about the abstruse merits of one Linux distribution over another. The market will be mature when we no longer argue about this model over that model, or about exactly how they get access to data — but about what we do with them in order to deliver value for users.

***

🖼️  Photos by [Fred Robin](https://unsplash.com/@ntxr) on [Unsplash](https://www.unsplash.com)

[^1]: And can we talk about that GUI for a moment? For how long have Salesforce users been invited to switch to the Lightning experience? The length of that transition should illustrate just how important change management is as a discipline. Users do not like the GUI they spend a lot of their work hours in to change under them, and they really do not like having to recreate customisations they put in place laboriously to help them do their work.