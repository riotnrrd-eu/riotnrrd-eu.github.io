---
layout: post
title:  Adventures in AppleScript 
date:   2014-02-18 
categories:  tech Apple AppleScript
---

Here’s a handy little AppleScript to switch the Bluetooth audio output device on a Mac.

Why do this? Well, partly because I can and it’s fun, but partly because I run a headless Mac Mini, and I’d rather not have to VNC into it just for something this trivial. Since AppleScript can be run from the command line via `osascript`, this little script can easily be triggered from SSH.

The next step is to make an iPhone-optimised web control panel for this and a couple of other equally simple tasks.

```
set theDevice to "HT-CT260”
     
     tell application "System Events" to tell process “SystemUIServer"
          tell (first menu bar item of menu bar 1 whose value of attribute "AXDescription" is "Bluetooth")
               click
               delay 0.2
               tell menu item theDevice of front menu
                    click
                    delay 0.2
                    try
                         click menu item "Connect" of menu theDevice
                         click menu item "Use as audio device" of menu theDevice
                    end try
               end tell
          end tell
     end tell

     tell application "Finder" to activate
```

It wasn’t obvious how to do this, and then I had to do it twice, because I did the development on Mavericks, only to realise that the Bluetooth Preferences pane is different between Mavericks and Mountain Lion… The method above works on both versions though, so it’s all good.

If you need to do this sort of thing from scratch, the Accessibility Inspector in Xcode is your friend. I obviously started out trying to browse menu items off the Finder menu bar by using `UI Elements` directly in the AppleScript Editor. The problem is that this only gives the Apple menu and the basic menus (File, Edit, View, Go, Window and Help), none of the widget menus over to the right. Because they belong to SystemUIServer. Of course.

If you need to use this actual script, you’ll want to set the value of `theDevice` to your own device rather than “HT-CT260”. I didn’t make this script to take inputs, so there’s no downside for me in hardcoding the value. Apart from that, it should be ready to go.