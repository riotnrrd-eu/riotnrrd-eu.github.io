---
layout: post
title: Migrating — Again
date: 2024-03-25
categories: admin evernote
---

# Migrating — Again

Yes, the blog has moved — [again]({% post_url 2013-10-06-Easiest-blog-platform-ever %}. This time it's running on Github Pages, which is billed as being an easy and free way of hosting Markdown, but turns out to have a number of issues in practice if you are trying to migrate an existing blog there, even if it was already written in Markdown.

Evernote had been going downhill for a while, so I had moved almost all my note-taking to Obsidian. I was still running my blog through Postach.io, though, because it was up and running and still worked fine for me. However, [Evernote's new owners](https://evernote.com/blog/evernote-next-move-joining-bending-spoons) rug-pulled the free tier, limiting it to 50 notes. This blog goes back to 2012 and has way more than 50 notes, so that was a problem. To their credit they didn't actually delete anything, but they did block users with more than 50 notes from creating any new ones.

This happened back in November, so I started investigating my options. Evernote does have a robust set of export tools, so I was able to dump everything out to the filesystem — and that was where the real work started. 

Github Pages uses Jekyll, which includes categories in its post URLs, and also has a specific filename convention. These two changes together meant that every internal link was broken, and not in a way that could easily be fixed with a quick find/replace. I dusted off my *very* rusty sed skills to script up some logic that would go through the files, identify links, and try to work out the new naming format, including Jekyll's internal headers. 

Then I had to do something similar with images, including renaming images that had spaces in their filenames — something i had never had to worry about when I was just pasting them into Evernote.

The final challenge that I had was another case of a platform getting bought up and rug-pulled, namely Twitter. Postach.io had (has) a nice feature to embed tweets, but I am feeling increasingly uncomfortable about the future of X-formerly-known-as-Twitter, to the point that I have moved off it entirely for my own purposes — and so have [many others]({% post_url 2023-04-14-Twitter-of-Babel.html %}). This meant that I had to go through all my embeds and replace them with screenshots. I was able to automate the majority of this, but a number of those posts were no longer live. I was able to capture a majority of those from the Internet Archive, but some had not been captured there at all, so sadly I had to remove those entirely.

I was able to cover the majority of these situations through scripting, but then I had to make one last laborious manual pass to handle corner cases — things like occasional smart quotes, or a tendency Evernote had for a time to encapsulate URLs in angle brackets. Somehow Postach.io was able to digest these so I had never noticed what was going on, but Jekyll choked, so all of these had to be fixed too, together with other miscellaneous broken links and typos.

So that's why it all took so long, basically.

# Acknowledgements

I was finally ready to go live, but stumbled on setting up DNS. Serendipitously, I found my old comrade Sean Berry in the acknowledgements to Cory Doctorow's excellent book [The Bezzle](https://craphound.com/bezzle/).

![](/images/bezzle-US-cover-large.jpg)

I messaged him to congratulate him, and we got chatting. The topic of my DNS troubles came up, so Sean very kindly offered to rubber-duck my config. To cut a long story short, we once again proved the two core maxims of IT. One, it was indeed DNS, and two, it was fixed by basically turning it off and on again.

So, thanks to Sean, we are now live once again, albeit with a very basic default skin. Next time I have a burst of creativity I will try to come up with something slightly more appealing, but for now, at least everything should work (but do let me know if not!).