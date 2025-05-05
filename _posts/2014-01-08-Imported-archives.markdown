---
layout: post
title:  Imported archives 
date:   2014-01-08 
categories:   
---

# Imported archives


I finally managed to import my old Wordpress blog into Evernote and upload the posts here. I managed to keep the dates, too, so the archives now stretch back into the past, all the way to posts that were originally created on Posterous before *that* went away.

Some of my favourite posts are below:

+ [All Software Sucks](http://findthethread.postach.io/all-software-sucks)
+ [The joy of making up words](http://findthethread.postach.io/the-joy-of-making-up-words)
+ [Collisions](http://findthethread.postach.io/collisions)
+ [On Piracy](http://findthethread.postach.io/on-piracy)

***
To import your own Wordpress blog into Evernote you will need [this script](https://github.com/adammorris/Luis-Rei-Wordpress-to-Evernote/blob/master/wordpress.py) and a way to run Python. If you have a Mac, you’re already fine. 

First export your posts from Wordpress. You’ll find the export and import options under “Tools" in your blog admin area. Then you’ll want to run the script. Launch Terminal, cd to wherever you saved the script, and run it like so:

     `python wordpress.py -o evernote wordpress.xml`

Replace `evernote` with the directory where you want your Evernote notebook created, and `wordpress.xml` with the name of your own exported XML file from Wordpress. This will result in a directory full of `.enex` files. Import the directory into Evernote (File > Import Notes).

You will still need to do some manual clean-up, especially of links between posts. Also some of the formatting can get messed up, and a few images got lost in my export and I had to re-add them manually into Evernote. It’s still better than doing it by hand!

