---
layout: post
title:  Intersections 
date:   2014-02-07 
categories:  tech 
---

A wise person once advised me to try to find my own intersection. 

No, this wasn’t advice about a street map! The idea is that all of us are in various circles, starting from the most inclusive (“human”) and going through increasingly selective ones (“database high-availability expert”, “lutenist”, “olympic athlete”). Very few people can be at the absolute pinnacle of any one field, but if you place well in a few different fields, you have a shot at placing *very* well at the **intersection** of those different circles. I’m not a betting man, but if I were, I would lay good odds against there being many people in the intersection of the three random fields I threw out there!

![](/images/unknown_filename.190.jpeg)

I am still working at getting better at everything I do, and indeed adding new circles if I can, “father of a girl” being the latest. I did have cause to ponder the following question yesterday: what is the intersection of the sets “marketing professional” and “busts out awk at the drop of a hat”?

Context: I was looking back at the past year of (work) blogging, and wanted to see posting frequency, average views per post by author, engagement, and that sort of thing. Our blogging platform does not seem to let ordinary users dump data to file - admins may have that capability, but I don’t. This meant that my first hurdle was getting the data out. 

Predictably, Excel choked when I simply copied from the web page and pasted into a worksheet. Browser developer tools helped me make sure that I was copying just the table and not extraneous `DIV` elements, but the data I wanted were split across multiple pages, and Excel couldn’t handle multiple `TH` table headers, especially in combination with cells spanning multiple rows. 

I ended up pasting the raw HTML into `vim`, cleaning it up so it was all a single `TABLE`, and dropping that into Excel.

Next problem: Excel can’t handle dates.[^1] Despite the dates being in one of the formats Excel claims to recognise (like "February 7, 2014”) I could not for the life of me persuade it to treat that cell as a date, even after trimming the trailing timestamp.

Back to Terminal! A quick romp with `vim` and `awk` produced the following (in case it’s useful to anyone else):

```
	BEGIN {
          FS = ";"
          OFS = ";"
          split("January February March April May June July August September October November December", month, " ")
          {
               for (i in month) {
                    month_nums[month[i]]=i
               }
          }
     }

     {
          split($7, datebits, " ")
          myday = substr(datebits[2], 1, length(datebits[2])-1)
          myyear = substr(datebits[3], 3, 2)
          mymonth = month_nums[datebits[1]]
          likes = substr($3, length($3))
          bookmarks = substr($4, length($4))
          print $1, $2, likes, bookmarks, $5, $6, myday"\/"mymonth"\/"myyear
     }
```

Note that despite the fact I had told Excel to export as CSV, meaning **comma**-separated values, it actually used semicolons as the separator, so I had to set the separator for awk myself with the `FS` and `OFS` variables. Yes, I know it’s probably possible to persuade Excel to do the right thing here, but this was easier and quicker.

This translates my extended "February 7, 2014” date into "7/2/14" format, which Excel seems to be able to digest, now that its food has been chewed for it by awk. I was then able to use fun Excel functions like `FREQUENCY` and `SUMIF` to actually extract and graph the data I was after in the first place.

Fun times. Nearly as fun as that time I had to turn to Ethereal and `rtmpdump` to watch some videos when the online Flash player turned out to be even more brain-dead than is usual for the breed.

***So much for marketing types only knowing PowerPoint…***

[^1]: Well, we knew *that*. If I had a buck for every time I have wanted to murder whoever coded Excel's date-handling routines, I'd be able to afford that Porsche. The reason they are so bad is they work just well enough that you can't treat the dates as strings, without actually, y'know, *working* for date manipulation - hence the whole expedition with `awk`.