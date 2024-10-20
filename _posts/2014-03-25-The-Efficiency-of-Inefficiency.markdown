---
layout: post
title:  The Efficiency of Inefficiency 
date:   2014-03-25 
categories:  cloud tech 
---

# The Efficiency of Inefficiency


Yesterday I wrote about how the value of private cloud is enabled by past inefficiencies: [Hunting the Elusive Private Cloud]({% post_url 2014-03-24-Hunting-the-Elusive-Private-Cloud %}). There is another side to that coin that's worth looking at. Vendors - especially, but not only, hardware vendors - made handsome profits catering to that inefficiency. If your datacenter utilisation rate is below 10%, then 90%+ of your hardware spending is… well, not quite *wasted*, but there are possible improvements there.  

A decade or so ago, all the buzz was about virtualisation. Instead of running one physical server with low utilisation, we would put a number of *virtual* servers on the same bit of physical kit, and save money! Of course that’s not how it worked out, because the ease of creating new virtual servers meant that the things started multiplying like bunnies, and the poor sysadmins found themselves *worse* off, with even more servers to manage instead of fewer!  

<iframe src="//embed.gettyimages.com/embed/6551-000029?et=BPStyAsOwk-mQI-St7dlhQ&sig=v_nEpEoadqBb-J022zvC0Zb9mpGdXFIPyiTHkZNwhKM=" width="400" height="589" frameborder="0" scrolling="no"></iframe>  

Now the promise of private cloud is that all the spare capacity can finally be put to good use. But what does this mean for the vendors who were relying on pushing all that extra tin?  

Well, we don’t know yet. Most private cloud projects are, frankly, still at a very low level of maturity, so the impact on hardware sales is limited so far. One interesting indicator, though, is what happens as *public* cloud adoption ramps up.  

Michael Coté, of 451 Research, [flagged this](http://coteindustries.com/post/80575866513/a-nice-illustration-of-the-problem-shifting-your "A nice illustration of the problem shifting your customer base from on-premises to public cloud") (emphasis mine):  

> Buried in this piece on Cisco doing some public cloud stuff is this little description about how the shift to public cloud creates a strategic threat to incumbent vendors:
> 
>> Cloud computing represented an interesting opportunity to equipment companies like Cisco, as it aggregated the market down to fewer buyers. There are approximately 1,500 to 2,000 infrastructure providers worldwide verses millions of businesses; reducing the buyers to a handful would lower the cost of sales. And, as cloud sales picked up, reducing on-premises equipment spending, those providers would represent an increasing share of sales and revenue.

>> 
>> The problem with this strategy, as companies like Cisco Systems and Juniper Networks discovered, is **the exchange of on-premises buyers to cloud buyers is not one to one**. Cloud providers can scale investments further than any individual enterprise or business buyer, resulting in a lower need for continually adding equipment. This phenomenon is seen in server sales, which saw unit shipments fall 6 percent last year and value fall nearly twice as fast.  

Even if we assume that a company offloading some servers to the public cloud instead of buying or replacing them in its own datacenter is doing so on a 1:1 basis - one in-house physical server replaced by one virtual server in the public cloud - the economics mean that the replacement will be less profitable for the equipment vendor. The public cloud provider will be able to negotiate a much better price per server because of their extremely high purchasing volume - and this doesn’t even consider the mega-players in cloud, who build their own kit from scratch.  

Since I mentioned Cisco, though, I should point out that they seem to be weathering the transition better than most. According to Forrester’s Richard Fichera, [Cisco UCS at five years](http://blogs.forrester.com/richard_fichera/14-03-19-cisco_ucs_at_five_years_successful_disruption_and_a_new_status_quo) is doing just fine:  

> HP is still number one in blade server units and revenue, but Cisco appears to be now number two in blades, and closing in on number three world-wide in server sales as well. The numbers are impressive:
> 
> * 32,000 net new customers in five years, with 14,000 repeat customers
> * Claimed $2 Billion+ annual run-rate

> * Order growth rate claimed in “mid-30s” range, probably about three times the growth rate of any competing product line.  

To me, it looks like the UCS server approach of very high memory density works very well for customers who aren’t at the level of rolling their own servers, but have outgrown traditional architectures. Let’s see what the next five years bring.

                                            