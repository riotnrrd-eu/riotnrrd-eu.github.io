---
layout: post
title:  False Positive Attitude 
date:   2023-10-06 
categories:  AI LLM 
---

# False Positive Attitude


# Don't Believe The Hype

Yes, I'm still on about "AI"[^1], because the collective id has not yet moved on.

Today, it's an article in *Nature*, with the optimistic title "[AI beats human sleuth at finding problematic images in research papers](https://www.nature.com/articles/d41586-023-02920-y#ref-CR1)":

> An algorithm that takes just seconds to scan a paper for duplicated images racks up more suspicious images than a person.

Sounds great! Finally a productive use for AI! Or is it?

> Working at two to three times \[the researcher\]’s speed, the software found **almost all** of the 63 suspect papers that he had identified — and 41 that he’d missed.

(emphasis mine)

So, the AI found "almost all" of the known positives, and identified 41 more unknowns? We are not told what the precise ratio is of false negatives (known positives that were missed), let alone how many false positives there were (instances of duplication flagged by AI that turned out not to be significant).

These issues continue to plague "AI"[^1], and will continue to do so for the foreseeable future. The mechanisms to prevent these false identifications are probabilistic, not deterministic. In the same way that we cannot predict the output of a large language model (LLM) for a given prompt, we also cannot prevent it from ever issuing an incorrect response. At the technical level, all we can do is train it to decrease the probability of the incorrect response, and pair the initial "AI"[^1] with other systems designed to check its work. Cynically, though, that process takes money and time, and Generative AI is at the Peak of Inflated Expectations *now*, we need to ship while the bubble is still inflating!

# AI Needs A Person Behind The Curtain

Technology, however, is only part of the story. This academic image analysis tool could well end up having real-world consequences:

> The end goal \[…\] is to incorporate AI tools such as Imagetwin into the paper-review process, just as many publishers routinely use software to scan text for plagiarism.

There's the problem. What recourse do you have as an academic if your paper gets falsely flagged? Sure, journals have review boards and processes, but that takes time — time you might not have if you're under the gun for a funding decision. And you could easily imagine a journal being reluctant to convene the review board unless the "AI"[^1] indicated some level of doubt — a confidence threshold set at, say, 70%. If the "AI"[^1] is 90% confident that your graph is plagiarised, tough luck.

The example of plagiarism detection is telling here. Systems such as Turnitin that claim to detect plagiarism in students' work had an initial wave of popularity, but are now being [disabled](https://dailyfreepress.com/2023/09/28/com-responds-to-turnitins-false-ai-detection-rates/) in many schools due to high false-positive rates. A big part of the problem is that, because of the sheer volume of student submissions, it was not considered feasible for a human instructor to check everything that was flagged by the system. Instead, the onus was placed on students to ensure that their work could pass the checks. And if they missed a deadline for a submission because of that? Well, tough luck, was the attitude — until the heap of problems mounted up high enough that it could no longer be ignored.

This is not a failure of LLM technology as such. The tech is what it is. The failure is in the design of the system which employs the technology. Knowing that this issue of false positives (and negatives!) exists, it is irresponsible to treat "AI"[^1] as a black box whose pronouncements should always be followed to the letter, even and including if they have real-world consequences for people.

[^1]: Still not AI.

