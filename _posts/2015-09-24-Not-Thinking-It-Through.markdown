---
layout: post
title:  Not Thinking It Through 
date:   2015-09-24 
categories:   
---

# Not Thinking It Through


Dear web programmers, input validation is important. We can all agree on this. 

 ![|500x280](/images/unknown_filename.247.gif) 

*Lazy* input validation, however, just leads to user frustration. 

My “favourite” examples are phone numbers and IBAN codes. In both cases, spaces are irrelevant to the result, so kindly take the extra thirty seconds to rule out spaces from your character count. Otherwise, when I copy & paste - or simply *type* - the code in human-legible format, broken down with spaces, and your validation fails or the code simply truncates the input to the maximum allowable length, I will wish you all sorts of ill. 

The same goes for non-numeric characters in phone numbers. How do you want me to enter an international phone number? Should I assume that your international code is 00? I **know** that is not valid everywhere. Meanwhile, any human or dialling software understands + as “replace this with the appropriate international dialling code”. 

I occasionally enter * or # in a telephone number field to go directly to a particular extension or to preselect options in a phone tree. I also do the same with email, adding “+foldername” to direct email straight to a particular folder in my inbox. It’s a sad commentary on the general quality of software that I am pleasantly surprised when something actually accepts these. 

*** 
Image via [DevOps Reactions](http://devopsreactions.tumblr.com/post/126327534452/the-day-before-the-deadline-2)

