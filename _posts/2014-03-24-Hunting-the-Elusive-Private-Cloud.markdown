---
layout: post
title:  Hunting the Elusive Private Cloud 
date:   2014-03-24 
categories:  cloud tech 
---

*While I work for a cloud management vendor, the following represents my personal opinion - which is why it’s published here and not at my work blog.*

It seems that in IT we spend a lot of time re-fighting the same battles. The current example is “private cloud is not a cloud”.

<iframe src="//embed.gettyimages.com/embed/182055970?et=aegK1bCYBkyrFhEVI1izBw&sig=8DtLeiYVs_54q6_X2h4Ks5HcpmuY_Czp7SsXVumtjo4=" width="507" height="407" frameborder="0" scrolling="no"></iframe>

Some might expect me to disagree, but in fact I think there’s more than a grain of truth in that assertion. The problem is in the definition of what is a cloud in the first place.

If I may quote the [NIST definition](http://csrc.nist.gov/publications/nistpubs/800-145/SP800-145.pdf) yet again: *(revs up motorcycle, lines up on shark tank)*

> **On-demand self-service.** A consumer can unilaterally provision computing capabilities, such as server time and network storage, as needed automatically without requiring human interaction with each service provider.
> 
> **Broad network access.** Capabilities are available over the network and accessed through standard mechanisms that promote use by heterogeneous thin or thick client platforms (e.g., mobile phones, tablets, laptops, and workstations).
> 
> **Resource pooling.** The provider’s computing resources are pooled to serve multiple consumers using a multi-tenant model, with different physical and virtual resources dynamically assigned and reassigned according to consumer demand. There is a sense of location independence in that the customer generally has no control or knowledge over the exact location of the provided resources but may be able to specify location at a higher level of abstraction (e.g., country, state, or datacenter). Examples of resources include storage, processing, memory, and network bandwidth.
> 
> **Rapid elasticity.** Capabilities can be elastically provisioned and released, in some cases automatically, to scale rapidly outward and inward commensurate with demand. To the consumer, the capabilities available for provisioning often appear to be unlimited and can be appropriated in any quantity at any time.
> 
> **Measured service.** Cloud systems automatically control and optimize resource use by leveraging a metering capability at some level of abstraction appropriate to the type of service (e.g., storage, processing, bandwidth, and active user accounts). Resource usage can be monitored, controlled, and reported, providing transparency for both the provider and consumer of the utilized service.

The item most people point to when making the claim that "private cloud is not a cloud” is the fourth in that list: *elasticity*. Public clouds have effectively infinite elasticity for any single tenant: even Amazon itself cannot saturate AWS. By definition, private cloud does not have infinite elasticity, being constrained to whatever the capacity of the existing datacenter is.

So it’s proved then? Private cloud is indeed not a cloud?

Not so fast. There are two very different types of cloud user. If you and your buddies founded a startup last week, and your entire IT estate is made up bestickered MacBooks, there is very little point in looking at building a private cloud from scratch. At least while you are getting started and figuring out your usage patterns, public cloud is perfect.

However, what if you are, say, a big bank, with half a century’s worth of legacy IT sitting around? It’s all very well to say “shut down your data centre, move it all to the cloud”, but these customers still have *mainframes*. They’re not shuttering their data centres any time soon, even if all the compliance questions can be answered.

The reason this type of organisation might want to look at private cloud is that there’s a good chance that a substantial proportion of that legacy infrastructure is under- or even entirely un-used. Some studies I’ve seen even show average utilisation below 10%! **This is where they get their elasticity**: between the *measured service* and the *resource pooling*, they get a much better handle on what that infrastructure is currently used for. Over time, private cloud users can then bring their average utilisation way up, while also increasing customer satisfaction.

Each organisation will have its own utilisation target, although 100% utilisation is unlikely for a number of reasons. In the same way, each organisation will have its own answer as to what to do next: whether to invest in additional data centre capacity for their private cloud, or to add public cloud resources to the mix in a hybrid model. 

The point remains though that private cloud is unquestionably “real” and a viable option for these types of customers. Having holy wars about it among the clouderati is entertaining, but ultimately unhelpful.