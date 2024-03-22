---
layout: post
title:  Printing Money 
date:   2023-02-03 
categories:  tech printers 
---

# Printing Money


I spent more time than I should have yesterday installing my mother-in-law’s new HP printer, and while I dodged the [more obvious scams](https://www.theatlantic.com/technology/archive/2023/02/home-printer-digital-rights-management-hp-instant-ink-subscription/672913/?ref=galaxy-brain), I was actually shocked at how bad the experience was. There is absolutely no way that a normal person without significant IT experience could do it. And the worst part is that HP are in my experience the *best* — okay, least bad — printer manufacturer out there.

I'm going to document what happened in exhaustive detail because I still can't bring myself to believe some of what happened. It's not going to be a fun post. Sorry. If you want a *fun* post about how terrible printers are, [here's one from The Oatmeal](https://theoatmeal.com/comics/printers).

- The “quick start” guide only showed the physical steps (remove packaging, connect power cord, add paper) and then offered a QR code to scan to deploy an HP app that would supposedly take care of the rest of the process.
- The QR code lead to a URL that 404'd. In retrospect, this was the moment when I should have packed everything back up and shipped it back to HP.
- Instead of following through on that much better plan and saving myself several hits to my sanity, some detective work helped me to identify what the app should be and find it in the Google Play Store (my MiL's computer is a Chromebook; this will be significant later).
- The app's "install new printer" workflow simply scans the local network for printers. Since the step I was trying to accomplish was *connecting the printer to Wi-Fi* (this model doesn't have an on-board control panel, only an embedded web server), this scan was not particularly helpful.
- The app's next suggestion was to contact support. Thanks, app.
- After having checked the box for any additional docs, and finding only reams of pointless legal paperwork documenting the printer's compliance to various standards and treaties, I gingerly loaded up the HP web site to search for something more detailed.
- The HP website's search function resolutely denied all knowledge of the printer model.
- A Google search scoped to the HP web site found the printer's product page, which included an actual manual.
- The manual asked me to connect to the printer's management interface, but at no point includes a step-by-step process. By piecing together various bits of information from the doc and some frantic Googling, I finally work out that I need to:
- Connect to the printer's own ad-hoc Wi-Fi network;
- Print a test page to get its IP address (this step involves holding down the paper feed button for 10 seconds);
- Connect to that IP address;
- Reassure the web browser that it's fine to connect to a website that is INSECURE!!1!
- Not find the menu options from the doc, only some basic information about supplies;
- Panic;
- Note a tiny "Login" link hidden away in a corner;
- Mutter "surely not…"
- Fail to find any user credentials documented anywhere, or indeed any mention of a login flow;
- Connect as "admin" with no password on a hunch;
- Access the full management interface.
- At this point I was finally able to authenticate the printer to the correct Wi-Fi network, at which point it promptly rebooted and then went catatonic for a worryingly long time before finally connecting.
- But we're not done yet! The HP printer app claims to be able to set up the local printer on the Chromebook, but as far as I can tell, it doesn't even attempt to do this. However, we have a network connection, I can read out supply levels and what-not, how hard can this be?
- Despite having Google Cloud Print enabled, nothing was auto-detected, so I created it as IPP (amazingly, this step *is* actually in the docs).
- Time for a test print! The Chromebook's print queue showed the doc as PRINTED, but the printer didn’t produce anything, and as far as I could determine, it never hit the printer's own queue.
- Hang head in hands.
- Verified that my iPhone can see the printer (via AirPrint) and print to it. This worked first time.
- Tried deleting the printer and re-creating it; somehow Google Cloud Print started working at this point, so the printer was auto-detected? The resulting config looked identical to what I created by hand, except with a port number specified instead of just an IP address.
- Does it print now? HAHAHA of course not.
- Repeat previous few steps with increasing muttering (can't swear or throw things because I am in my mother-in-law's home).
- Decide to update software:
- The Chromebook updates, reboots, no change.
- The printer's product page does not show any firmware at all — unless you tell it you are looking for *Windows* software. There are official drivers for various Linux distros, but apparently they don't deserve firmware. There is nothing for macOS, because Apple wisely doesn't allow rando third-party printer drivers anywhere near their operating systems. And of course nothing for ChromeOS or "other", why would you ask?
- Download the firmware from the Windows driver page, upload it to the printer's management UI — which quoth "firmware not valid".
- Search for any checksum or other way to verify the download, and *of course* there is none.
- Attempt to decode the version embedded in the file name, discover that it is almost impossible to persuade ChromeOS to display a file name that long.
- Eventually decide that the installed and downloaded versions are probably the same, despite the installed one being over a year old.
- Give up and run away, promising to return with new ideas, or possibly a can of petrol and a Zippo.

