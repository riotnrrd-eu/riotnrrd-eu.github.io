---
layout: post
title:  Banking in the cloud 
date:   2014-01-15 
categories:  cloud 
---

# Banking in the cloud


Cloud computing is getting to be pretty universal, but there is still an assumption in certain quarters that it’s only for startups, especially public cloud. As the market matures, however, that position gets less and less tenable. If the *CIA* can work things out to run (some of) their applications on Amazon, despite [IBM’s best efforts](http://www.theregister.co.uk/2013/11/08/ibms_cia_cloud_claims_smashed_by_court_opinion/), surely most companies should be able to take advantage of the cloud, right?

Well, apparently [banks should never use the cloud](http://www.computerweekly.com/blogs/outsourcing/2014/01/banks-should-never-use-the-cloud.html), according to ComputerWorld. The post includes this quote, admittedly not from the author but "an unnamed source within banking IT”:

> I would not bank with a firm using the cloud to operate my account or hold my details.

![](/images/unknown_filename.48.jpeg)

In one of those moments of serendipity, the last customer I spoke to was in fact a bank[^1], and they wanted to discuss not only how they could move to private cloud, but how they could run some services in the public cloud and even become a cloud provider themselves for some of their customers.

This bank has been a customer for a very long time, with a large mainframe footprint and a good amount of distributed systems as well. In what is a fairly typical story, their IT environment is quite balkanised, which makes it hard for them to get a good view of what is going on, let alone enforce and document standards and best practices in a uniform manner. 

Obviously introducing cloud into this mix would just risk creating yet another silo; it’s silos all the way down. What the bank is after is unified management, that will span across all their diverse technologies and let them deliver a high level of IT service to their users. 

A key part of managing this sort of heterogeneous environment is knowing what goes where. The example ComputerWorld’s unnamed source uses of cash machines running in the public cloud or something is a perfect counter-example. The idea is to run payment systems and such on extremely reliable systems, almost certainly in-house. However, that sort of infrastructure gets expensive, not to mention the time taken to harden it, audit it regularly, and keep it secure over time. So why use the exact same standard for a marketing web site? Stick that in the public cloud! Put internal development systems on a free hypervisor to save license costs, and so on.

At AWS re:Invent we had two customers[^1] from the banking industry in the booth with us. Remember, that’s banks who are not just using private cloud internally, but actually deploying services to AWS. The reason they were there is to explain how they were not deploying anything willy-nilly to AWS, but setting and enforcing policies.

The cloud is a tool. All you need to do is use it right.

[^1]: Sorry, no names. You know how it is… 

***
Image by [Martin Wessely](http://wesse.ly) via [Unsplash](http://unsplash.com/)

