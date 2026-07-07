---
layout: post
title:  Absent Intelligence
date:   2026-07-07
categories:  AI
---

Maybe I was a little harsh when I said that ["AI" models don't have a moat]({% post_url  2026-04-14-Compute-Me-A-Moat %}) — and with all the hype around the big AI IPOs, it's worth revisiting and clarifying that statement. While I stand by my statement that *the models themselves* have no durable differentiation, I do think there is differentiation in the broader AI market — but it's a couple of levels of abstraction away from the models. This is the domain, not of hopeful miners in a gold rush, but of sellers of shovels to the miners — or perhaps even one level further back: operators of hotels, bars, and (why not?) brothels in San Francisco in 1849, say, happy to cater to dirty and dishevelled miners returning from the gold fields.

Large Language Models do have their place, especially in the enterprise. I am far less convinced of the business case for them in the consumer space, but I never claimed to understand the B2C world. On the other hand, maybe I *do* understand it better than I thought — because I know better than to stand up on stage and tell a bunch of new graduates to stop asking questions and jump on the AI rocket ship.

![A rocket ship. It's not supposed to look like that.](/images/blue-origin-explosion.gif)

There is a huge disconnect between those graduates who have been booing commencement speakers that laud AI — and [cheering the comedians who repeat “fuck AI”](https://www.inc.com/jessica-stillman/ronny-chieng-told-harvard-grads-to-destroy-ai-they-cheered/91353239) — and the huge valuation ascribed to Anthropic, OpenAI, and SpaceX. Some say the whole of AI is a bubble, and the students are right and the market is wrong. I am not any sort of investment advisor, and of course something can be utterly bereft of value either technical and social and still be extremely valuable *financially* (ahem crypto ahem), but here is my own theory, for what it may be worse.

# Teaching robots to read the world

Fundamentally, there is a massive difference in both perceived and actual effectiveness between *consumer* AI and *enterprise* AI. There are a few different factors driving this disconnect, but the most important one is simply the availability of data for the AI models to work with. To put it another way, the enterprise world is full of data that is (more or less) easily legible to the AI tools, whereas the consumer world is largely not legible to AI in the same way. Worse, attempts to make the everyday world intelligible to AI come off as straightforwardly creepy, whether it’s [Meta’s pervert glasses](https://futurism.com/future-society/meta-ray-ban-smart-pervert-glasses) or the idea that anyone would actually want something looking over their shoulder at everything they do on their computer.

Meanwhile in the enterprise world we are drowning in data, for lack of ways to query and make use of any more than a small fraction of the information that a company of any size throws off continuously, just by virtue of its operation. Every company I've worked at has a graveyard of dashboards and reports that represent somebody's valiant attempt to make sense — and use — of that flood of information. Whether these are Excel files, Tableau dashboards, or customisations built on top of platforms like Salesforce or Siebel, doesn't really matter. One team, or maybe even just one particular exec, runs their strategy based on a specific view of the data. A different team has a different view. Then a new exec comes in, or a reorg happens, and all the dashboards and reports have to change to match.

AI tools are *great* at putting together those views, especially if you can give them visibility across multiple data stores. Looking at trends in support needs as mapped to profitability used to be a data science project, requiring people and tools. Now? It's a prompt away, and you immediately have access to up-to-date information that can drive better decisions.

Code generation ("vibe coding") is another great example. With software, the now well-known problem of "hallucination" is much reduced: the generated code will either work, or not, and there are existing tools that can validate its correctness. Yes yes, watch out for [nonexistent libraries hallucinated by AI tools which are then squatted by attackers](https://arxiv.org/pdf/2410.06462); you do still need to use your brain, but it's a force multiplier for programming.

*** 

As an aside, can I just say that I don’t understand why the damned things all must have a personality? I don't have a problem with people enjoying a spot of cosplay, but I do object to being made a part of it without my consent being sought. The computer should answer my question and shut up.

![SILENCE, BOT](/images/silence-bot.jpg)

*** 

That is not to say that the world of the enterprise is all happiness and light. Even industry analysts are now saying with their whole chest that [the layoffs being excused in the name of AI are nothing of the sort](https://www.forbes.com/sites/jasonwalker/2026/05/19/the-roi-on-ai-driven-layoffs-is-zero-why-are-leaders-still-doing-it/); the claims that AI *forced* the poor execs to lay off huge swaths of their staffs are just a fig-leaf for plain old incompetence. But there is also much more run-of-the-mill infection by AI brainworms going on.

# The brain worms are starving

I did not share this story at the time because the people involved could probably have identified themselves, but now that (I hope) the statute of limitations has expired, I will pass it on — albeit still without naming names: tech is a small world, and I have no interest in leaving it prematurely.

I was at dinner with a couple of high-powered executives at customer companies — CTO and CIO of their respective companies, which, while not household names exactly, were and are movers and shakers in their particular domains. The conversation inevitably turned to AI, and one of them proudly recounted how, instead of him and his team cloistering themselves in an off-site location for a couple of days to map out their new strategy, he had instead turned to AI. 

After (by his own estimation) a solid four hours of prompting the AI and iterating on the results, he had obtained a twenty-two (22) page document, which was still "not quite right". So he sent this slop to his team for them to "finish up" — and told this story with great satisfaction, implying that AI had brought huge improvements to the process.

Now despite going to Vegas once or twice a year for work for the last many years, I don't gamble, so I don't have objective evidence of how good my poker face is, but I must have managed to keep at least most of my feelings from activating my facial features. Inside, though? I was **screaming**.

Imagine: you are a fairly high-level IT professional, reporting to the C-suite of your employer, and you receive a 22 (twenty-two) page document from your boss, copied to all of your peers, which is claimed to represent the strategic direction for the company. The document is described as directionally correct but needing some work to clear up. What do you do?

The *most efficient* move at this point would be summarily to throw out the doc, schedule an off-site meeting somewhere with a whiteboard and limited cellular reception, and get to work — which is what you would have done before AI stuck its nose into the tent. But now that option is off the table, because the boss has sent you this half-assed effort, and it's on you to shine up the turd to the point that it can be shown in public. Except that you can't be seen to be using resources, because that would undermine the efficiency and consequent savings that AI is bringing to the department. You can't just ignore it, because this effort is going to determine the next few years of your work life. So now you have to resort to piecing together input here and there, working around everyone's day jobs, and try painfully to shoulder this malformed excuse for a strategy over the line. 

And the worst of it is, your boss is going to swan around, telling everyone that he saved the company a bunch of money and time, because he was able to do most of the work himself through the sheer power of his own vision, aided “only” by his AI copilot, with no need for pesky inconvenient human employees.

I did not throw that man into the nearby river, but I was very sorely tempted to do so, on behalf of his team and of all that is good and holy.

![River rapids, perfect for AI bro disposal](/images/dustin-belt-IAmDUa0b5lI-unsplash.jpg)

# It's surprising that people don't hate AI *more*

So, to sum up: many people hate AI because they only encounter manifestations of it that are stupid, evil, or both. A much smaller set of people love AI, because they use it at work and it really does help them — sometimes despite the best efforts of their colleagues, true.

To me, this discrepancy explains most of the AI bubble: there is a solid core of real value, increasingly supported by tangible revenue, but that is obscured by a lot of froth, as well as some regrettable hangers-on trying to attach themselves to the promise of revenue. I would guess that the big IPOs will still go ahead, but at some point in the future, there will be a divergence in the actual outcomes between those that serve the enterprise and those that attempt to capture the consumer. We are already seeing signs of [slowdown of the token burn]({% post_url 2026-06-10-Software-Is-Eating-Itself %}) that supports those outsize valuations.

Part of the reason for the public scepticism when it comes to AI is that a significant proportion of the public advocacy for AI sounds like the exact same sort of shilling we have all heard before, for cryptocurrencies, NFTs, or whatever. Sometimes, it’s even literally the same people. Straight to the moon, baby! 

But even in those extremely grifty cases, there was a solid core of real value. The pharmaceutical industry is now using blockchains — not Bitcoin, but private blockchains — to store data in ways that can be cryptographically proven to be unaltered. The same thing happened with drones, or 3D printers: apart from a few hobbyists, nobody has one in their home — but they are very useful and valuable in particular industrial niches, where they are operated by professionals. Ask the Armed Forces of Ukraine, if you don’t believe me.

I look forward to a time when nobody is talking about AI any more outside of specialised professional domains, and all the attention has moved on to something else. That will mean that AI is finally coming into its own as a mature element of the technology stack. And in the meantime, I will just remind you that ["NO" is a complete sentence](https://buttondown.com/monteiro/archive/how-to-use-no-as-a-complete-sentence/).

***

🖼️  Photos by [Dustin Belt](https://unsplash.com/@dbeltwrites) on [Unsplash](https://www.unsplash.com)