---
layout: post
title:  Feeping creatures 
date:   2014-01-21 
categories:  tech 
---

# Feeping creatures


If you’ve ever found yourself alone in a datacenter, with the white noise of the cooling fans lulling you into complacency, you may have caught a movement out of the corner of your eye, or thought you heard something go “feep” back in the rows and racks of machinery. You didn’t dream it; there *are* creatures back there, wandering around and occasionally *feep*ing softly to each other.

![](/images/unknown_filename.140.jpeg)

*From the [Feeping Creatures](http://feepingcreatures.tumblr.com/image/65359656922) Tumblr*

Actually, the truth is far more prosaic. “Feeping creatures” is just a spoonerism for “creeping features”, a disease of software products where they sprout features for no good reason. This would not normally be a problem, except for the pesky relationship between code and bugs. Basically, the more features and code you put in, the more bugs you will have.[^2]

> If debugging is the process of removing software bugs, then programming must be the process of putting them in. *-- Edsger Dijkstra*

However, even assuming your code is perfect, with no bugs whatsoever, the rapidly multiplying creatures, all feeping away madly to each other, are probably not doing your users any good. Implementing features that users don’t want or can’t use is a bad idea *even if those features are implemented correctly*.

> Without requirements or design, programming is the art of adding bugs to an empty text file. *-- Louis Srygley*

Users by and large don’t *want* features. I’m a nerd, and I geek out on new features, but most people are not like me.[^1] Most people don’t know how to find [geotags in Instagram](http://parislemon.com/post/74043316441/where-is-this-geotagged-place-wonders-instagram) and ask for locations in comments. My own wife sits watching YouTube videos on her phone screen or in a default-sized window, rather than full-screening or streaming them to the big TV with AirPlay. She’s not multi-tasking, she just *can’t be bothered* to start messing around with features.

The same thing happens with enterprise tools. These are famously infested with hordes of creatures, their incessant feeping deafening users. In fact, people have to be *forced* to use these tools, and if there is any workaround, they will take it in a shot.

![](/images/unknown_filename.139.jpeg)

If people can’t find the feature or use it once they have found it, it’s not useful. Get rid of it and/or figure out another approach.

People have a certain model of what they want to get done with your tool. Since it’s rather unlikely that the models will be the same from one person to the next, one of two things will have to change: either the model they have in their heads, or the usage model for the tool you built.

Guess what? Almost everyone will try to figure out a way to use your tool in a way that makes sense for them. Hardly anyone will Read The Fine Manual, or watch the video walkthrough you made, or access the wiki. Most will try to bash your tool into submission, and in the process develop a hatred for you and your tool that will last for years after they have moved to another job to get away from the tool.

![](/images/unknown_filename.141.jpeg)

Adding features may *feel* like you’re helping the users, but it’s not. Make a tool that does one thing well - and make sure that one thing is what your users wanted, and that they can actually get it done.

[^1]: This is only one of many reasons why I stay the heck away from working on consumer products.
[^2]: More on the [bugs per line of code ratio](http://mayerdan.com/ruby/2012/11/11/bugs-per-line-of-code-ratio/). I’ve seen this first-hand: remember, I used to work for a software-testing outfit, and still have many friends in that industry.

