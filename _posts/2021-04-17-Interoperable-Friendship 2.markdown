---
layout: post
title:  Interoperable Friendship 
date:   2021-04-17 
categories:  social social-media 
---

# Interoperable Friendship


Whenever the gravitational pull of social networks comes up, there is a tendency to offer a quick fix by "just" letting them integrate with each other, or offer export/import capability.

[Cory Doctorow tells an emotional tale in *Wired*](https://www.wired.co.uk/article/social-media-competitive-compatibility) about his grandmother's difficult decision to leave all of her family and friends behind in the USSR, and concludes with this impassioned appeal:

> Network effects are why my grandmother's family stayed behind in the USSR. Low switching costs are why I was able to roam freely around the world, moving to the places where it seemed like I could thrive.
>
> Network effects are a big deal, but it's switching costs that really matter. Facebook will tell you that it wants to keep bad guys out – not keep users in. Funnily enough, that's the same thing East Germany's politburo claimed about the Berlin Wall: it was there to keep the teeming hordes of the west out of the socialist worker's paradise, not to lock in the people of East Germany.
>
> Mr Zuckerberg, tear down that wall.

As appealing as that vision is, here is why interoperability won't and can't work.

![](/images/image.59.png)

Let's take our good friends [Alice and Bob](https://en.wikipedia.org/wiki/Alice_and_Bob), from every cryptography example ever. Alice and Bob are friends on one social network, let's call it Facester. They chat, they share photos, they enter a bunch of valuable personal information. So far so good; information about each user is stored in a database, and it's pretty trivial to export user information, chat logs, and photographs from the system.

Here's the problem: the account data is not the only thing that is valuable. You also want the **relationships** between users. If Alice wants to join a new network, let's call it Twitbook, being able to prepopulate it with her name and profile picture is the least of her issues. She is now faced with an empty Twitbook feed, because she isn't friends with anyone there yet.[^1]

Alice and Bob's relationship on Facester is stored in a data structure called a *graph*; each link between nodes in the graph is called an *edge*. While this structure can be exported in purely technical terms, this is where things start getting complicated.

What if Alice and Bob's sworn enemy, Eve, registers on Twitbook with Bob's name? Or maybe there's simply more than one Bob in the world. How can Twitbook meaningfully import that relationship from Facester?

![](/images/image.60.png)

There are various policies that you could come up with, ranging from terrible to more terrible.

If both Alice and Bob go to a certain amount of effort, entering their Facester profile info on Twitbook and vice versa, the export and reimport will be able to reconcile the data that way — but that's a lot of work and potential for error. What happens if even one of your friends hasn't done this, or gets it wrong? Should the import stop or continue? And does the destination network get to keep that dangling edge? Here in what we still call the real world, Facebook already creates "ghost profiles" for people who do not use its services, but whose existence they have inferred from their surveillance-driven adtech. These user records have value to FB because they can still be used for targeting and can  have ads sold against them.

Alice and Bob's common friend Charlie has chosen not to register for Twitbook because they dislike that service's privacy policy. However, if either Alice or Bob imports their data from Facester into Twitbook, Charlie could still end up with one of these ghost profiles against their wishes. Contact data are not the property of the person who holds them. Back to the real world again, this is the problem that people have with the likes of Signal or [Clubhouse]({% post_url 2021-02-13-Clubhouse-—-But-Why? %}), that prompt users to import their whole address book and then spam all of those people. This functionality is not just irritating, it's also actively dangerous as a vector for abuse.

Another terrible policy is to have some kind of global unique identifier for users, whether this means mandating the use of government-assigned real names, or some global register of user IDs. Real names are problematic for all sorts of reasons, whether it's for people who prefer to use pseudonyms or nicknames, or people who change their name legitimately. Facebook got into all sorts of trouble with their own attempt at a [real-name policy](https://en.wikipedia.org/wiki/Facebook_real-name_policy_controversy), and that was just for one network; you could still be pseudonymous on Twitter, precisely because the two networks are not linked.

People do want to partition off different parts of their identity. Maybe on Facester Alice presents as a buttoned-up suburban housewife, but on Twitbook she lets her hair down and focuses on her death metal fandom. She would prefer not to have to discuss some of the imagery and lyrics that go with that music at the PTA, so she doesn't use the same name and keeps these two aspects of her personality on separate networks. Full interoperability between Facester and Twitbook would collapse these different identities, whatever Alice's feelings on the matter.

![](/images/image.61.png)

Some are invoking the [right to data portability that is enshrined in GDPR](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/individual-rights/right-to-data-portability/), but this legislation has the same problem with definitions: whose data are we talking about, exactly?

The GDPR states (emphasis mine):

> The right to data portability allows individuals to obtain and reuse **their personal data** for their own purposes across different services.

Applying this requirement to social networks becomes complicated, though, because Alice's "personal data" also encompasses data about her relationships with Bob and Charlie. Who exactly does that data belong to? Who can give consent to its processing?

GDPR does not really address the question of how or whether Alice should be allowed to obtain and reuse data about Bob and Charlie; it focuses only on the responsibility of Facester and Twitbook as data controllers in this scenario. Here are its suggestions about third parties’ data:

> What happens if the personal data includes information about others?
>
> If the requested information includes information about others (eg third party data) you need to consider whether transmitting that data would adversely affect the rights and freedoms of those third parties.
>
> Generally speaking, providing third party data to the individual making the portability request should not be a problem, assuming that the requestor provided this data to you within their information in the first place. However, you should always consider whether there will be an adverse effect on the rights and freedoms of third parties, in particular when you are transmitting data directly to another controller.
>
> If the requested data has been provided to you by multiple data subjects (eg a joint bank account) you need to be satisfied that all parties agree to the portability request. This means that you may have to seek agreement from all the parties involved.

However, all of this is pretty vague and does not impose any actual requirements. People have tens if not hundreds of connections within social networks; it is not realistic that everybody get on board with each request, in the way that would work for the GDPR's example of a joint bank account, which usually involves only two people. If this regulation were to become the model for regulation of import/export functionality of social networks, I think it's a safe bet that preemptive consent would be buried somewhere in the terms and conditions, and that would be that.

Tearing down the walls between social networks would do more harm than good. It's true that social networks rely on the gravity of the data they have about users and their connections to build their power, but even if the goal is tearing down that power, interoperability is not the way to do it.

***

UPDATE: Thanks to Cory Doctorow for pointing me at [this EFF white paper](https://www.eff.org/wp/interoperability-and-privacy) after I tagged him on Twitter. As you might expect, it goes into a lot more detail about how interoperability should work than either a short *Wired* article or this blog post do. However, I do not feel it covers the specific point about the sort of explicit consent that is required between users before sharing each others' data with the social networks, and the sorts of information leaks and context collapse that such sharing engenders.

***
🖼️  Photos by [NordWood Themes](http://creativemarket.com/nordwood), [Alex Iby](http://alexiby.com), and [Scott Graham](http://homajob.com) on [Unsplash](https://www.unsplash.com)

[^1]: Or she doesn't follow anyone, or whatever the construct is. Let's assume for the sake of this argument that the relationships are fungible across different social networks — which is of course not the case in the real world: my LinkedIn connections are not the same people I follow on Twitter.

