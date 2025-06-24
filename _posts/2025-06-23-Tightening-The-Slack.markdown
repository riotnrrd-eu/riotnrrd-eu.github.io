---
layout: post
title: Tightening The Slack
date:   2025-06-23
categories: Zoom Slack Salesforce Teams Microsoft Google work office
---

Slack is in the news, because parent company [Salesforce has updated Slack's Terms of Service to block access via API](https://www.computerworld.com/article/4005509/salesforce-changes-slack-api-terms-to-block-bulk-data-access-for-llms.html).

The main change in the [new Slack ToS](https://slack.com/intl/en-gb/terms-of-service/api) is around the Discovery API and Data Access API. These had previously been used by a number of third-party vendors, including Glean[^1], to enable various search features that integrated Slack with other data sources.

Slack has been part of the standard "startup tech stack" together with Zoom and Google Docs, and I have long said that this situation was unstable due to a combination of competition from integrated suites (notably Microsoft's) and individual vendors in that stack trying to grab a bigger piece of the pie by locking out other vendors. For instance, Zoom has been trying desperately to get anyone to use its new document-management features.

Back in 2020, [I called it]({% post_url 2020-12-23-Tech-and-distribution %}):

> Slack tried to kill email, but ended up becoming email — and as I wrote back in 2016, email has a long head start and is just generally much better at being email:
> 
>> most would-be email killers are walled gardens, consisting of a service that is tightly integrated with its client app and does not allow third-party clients. This makes it much harder for innovation to happen, because there is only one provider, and they deliver only the functionality that they want and can build. **If you want a feature to be added to Slack, you can’t build your own Slack client; you have to petition Slack to do it, and they choose whether to implement that feature or not.**
> 
> In the end, Slack, like email, became a feature. This is why the real benefit for Salesforce in its acquisition of Slack is consolidation and the end of modular, piecemeal acquisitions of SaaS products by companies.

(Emphasis added)

Here we have that strategy playing out. Salesforce does not want companies purchasing modular piecemeal SaaS products that can integrate with Slack data; it wants all that data to stay inside the extended Salesforce platform. And [Zoom and Google are doing the same thing]({% post_url 2024-04-19-Teams-Alone %}), of course:

> Zoom is arguably doing the right thing by adding collaboration (properly, as opposed to earlier half-hearted attempts). The problem Zoom has is that the customer base overlaps very significantly with Slack’s, which offers all the collaboration its users could possibly need, and has a solid track record of delivering what people want. Slack even has video calls in the shape of Huddles, further proving my point that video calling is a feature, not a platform. And then of course there is Google, which keeps trying to get people to use Meet (or whatever it’s called this month) to collaborate inside Google Docs.

![Pass the popcorn](/images/georgia-vagim-ny-lHmsHYHk-unsplash.jpg)

It's going to be interesting to watch this fight play out, but right now, I can't see any way this does not work out in Microsoft's favour. If you want an integrated suite with document management and collaboration, including both text and video chat, they have the deepest set of functionality. Google will pick up some of the market, on the basis of Docs and Meet being good enough, while Zoom will fight its corner based on the investments companies have made in specialised hardware in all of their meeting rooms. Then again, that used to be WebEx's moat…

And Salesforce? On paper, they have a strong position: a huge user base for Slack, and obvious synergies with their other products, including both integration platforms: Mulesoft, and [more recent acquisition, Informatica](https://www.theregister.com/2025/05/27/salesforce_snaps_up_informatica_for/). I do wonder, though, how much user goodwill might matter here.

Slack had always been one of those "shadow IT" tools that users would adopt on their own and official corporate IT would be forced to recognise and accomodate later. This grassroots adoption was due in no small part to Slack's wide use in open-source communities, something that Salesforce continued to support for a while post-acquisition. That benevolence appears to be at an end, though, with Salesforce revoking the free enterprise plans for the [Cloud Native Computing Foundation](https://www.cncf.io/blog/2025/06/16/cncf-slack-workspace-changes-coming-on-friday-june-20/) and the [Kubernetes project](https://www.kubernetes.dev/blog/2025/06/16/changes-to-kubernetes-slack-2025/).

Salesforce is a master of the bundle strategy, so I am sure the plan over there is to compensate for any slowdown in grassroots adoption by including it in literally every sales campaign. The main Salesforce app is, uh, not the most user-friendly thing in the world, while Slack is well positioned to become not just the way users talk to each other, but how they talk to their IT stack. 

I am sure that goal looks great on a strategy deck, but it's going to be a lot harder to achieve if the only services that can integrate fully with Slack are built by Salesforce itself. Then we are back to where we started with Slack:

> If you want a feature to be added to Slack, you can’t build your own Slack client; you have to petition Slack to do it, and they choose whether to implement that feature or not.

***

🖼️  Photos by [Georgia Vagim](https://unsplash.com/@georgiavagim) on [Unsplash](https://www.unsplash.com)


[^1]: Full disclosure: Glean is a partner of my current employer, SnapLogic.