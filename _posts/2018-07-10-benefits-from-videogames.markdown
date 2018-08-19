---
layout: post
title: The benefits of playing video games
date: 2018-07-10 18:45:07 +0200
description: The state-of-the-art of the benefits of playing video games.
img: videogames.jpg # Add Image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Video games, Teaching]
---

This entry is going to be my **linux diary**, so I can keep on records the stuff I'm doing on the tablet. Well, let's start from the beginning:

## Windows hates me

This change started with the new update of Microsoft OS, **Windows 10**. I wanted to test it on my tablet, an **Asus Transformer T100** , to see how it was going. Even if I read a lot about the lack of privacy it "offers", I was also curious about all the changes like **multi-desktop support** (which both Linux and Macintosh offer since ages) and **Cortana** , which offered a lot of [features](http://www.pcworld.com/article/2874400/windows/windows-10-the-10-coolest-features-you-should-check-out-first.html) that seemed to be useful.

So... I installed it and, as you can imagine, it lasted about 5 days installed. I've found every new thing a **waste** of memory and CPU, and I had to reinstall some drivers like the touch-pad, because it wasn't working correctly. Thankfully, Microsoft offered a **downgrade** to Windows 8.1 if you didn't like Windows 10, so I tried it. Everything went perfect, except for a thing: That new driver which was installed during the time I was trying Windows 10 wasn't downgraded or something like that, and the desktop kept flashing and restarting even if I restarted the OS. That was the moment I gathered strength to **install Ubuntu** on my tablet.

Why **Ubuntu**? Because it's the only _Linux_ **well tweaked** to have almost every single component working. There are some exceptions of parts which aren't working, like the camera, the microphone and the hardware buttons ([GPIO](https://en.wikipedia.org/wiki/General-purpose_input/output)), but the rest is working in a really stable way.

## The start of the journey

Taking this into account, I downloaded [_Asus T100-TA Magic Stick ISO_](http://forum.xda-developers.com/windows-8-rt/win-8-development/live-asus-t100-ta-magic-stick-t3091481), version 1.5, I booted up _Ubuntu_ and I **installed it** with the included tool to do so. I **overwrote** the complete **internal flash memory**, included the UEFI partition. I still have a **backup** in my **external HDD** just in case I want to recover my system as it was a couple of months ago, so I'm not afraid to do so.

First thing I've done with the new OS is **delete Unity**. I hate that desktop environment, so I've installed **XFCE**. To do so, I've used a tool called `tasksel`. I've used the following commands to install it and execute it:

{% highlight shell-session %} 
~ $ sudo apt-get install tasksel
~ $ sudo tasksel
{% endhighlight %}

After this, I've checked `Xubuntu-desktop` and I've unchecked `Ubuntu-desktop`. You have to **wait a couple of minutes** in order to download _XFCE_ and uninstall _Unity_ and other applications related, and then the OS reboots and you have **Xubuntu** totally compatible with your tablet.

## Programs and more programs

Then, I've updated the OS and I've installed some useful programs:

{% highlight shell-session %} 
~ $ sudo apt-get update && sudo apt-get upgrade
~ $ sudo apt-get install libreoffice gdebi-core synaptic aptitude vlc xubuntu-restricted-extras libavcodec-extra rar wireshark
{% endhighlight %}

Also, I've installed **Dropbox** and **Google Chrome** (I don't really like _Chromium_ now, because Google has done a great advance in **memory handling** and _Chromium_ is still a bit slower and big than _Chrome_).

To install _Chrome_ I've used:

{% highlight shell-session %} 
~ $ wget https://dl.google.com/linux/direct/google-chrome-stable_current_i386.deb
~ $ sudo gdebi google-chrome-stable_current_i386.deb
{% endhighlight %}

In order to install _Dropbox,_ I've gone to [dropbox.com/install](https://www.dropbox.com/install) and I've downloaded the `\*.deb` file, and followed the instructions.

And that's everything I've made today. I hope the **touchpad support** becomes **better** and it gives us multi-touch as Windows does. That's the only thing I miss, the ability to scroll pages with the touchpad.

For further information, have a look at our Google+ Group: [https://plus.google.com/communities/117853703024346186936](https://plus.google.com/communities/117853703024346186936)

## (July 2018 Update)

Even though I was really motivated with the change to Linux, I switched it back to Windows after 6 months using Linux for the following reasons:

1. My feeling of the performance wasn't the same as using Windows. Even in 2018, we don't have complete support for this tablet, and we have to take some workarounds in order to have everything working. And there are some things that probably won't work easily, like the camera. 
2. I wasn't using Linux for anything I couldn't do in Windows and I needed some Windows programs for my University courses.

However, I have a constant feeling that maybe I should give it a try again. Will I do it? How knows, but if I do it, I'll keep you informed here ;)