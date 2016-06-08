---
layout: post
title: "First day at BSDCan 2016 devsummit"
date: 2016-06-09 00:39:17 +0200
comments: true
sharing: true
categories: freebsd devsummit bsdcan english ottawa
---

Let's begin this new series on [BSDCan 2016](http://2016.bsdcan.org/)!

As usual, we will have two days of both tutorials and [FreeBSD](https://www.FreeBSD.org/) devsummit, a regular event in almost all BSD-related conferences now.

{% img https://assets.keltia.net/blog/blog-13365.jpg "devsummit" "devsummit" %}

{% img https://assets.keltia.net/blog/blog-13366.jpg "devsummit" "devsummit" %}
<!--more-->
The Goat BoF
------------
Like last year, BSDCan kind of unofficially starts with the Goat BoF, the day before the devsummit & tutorials start.  Groff was a bit late this year so I have less pictures :)

While waiting for Groff to arrive, I noticed his little brother watching over us :)

{% img https://assets.keltia.net/blog/goat-13302.jpg "Little goat" "Little Goat" %}

After a few rounds of beer and food (which was greatly needed on my part), Henning was there carrying Groff with him \o/

{% img https://assets.keltia.net/blog/goat-13304.jpg "Henning & Groff" "Henning & Groff" %}

Pictures for yesterday's session are [there](https://assets.keltia.net/photos/BSDCan-2016/Goat%20BoF/index.html).

Devsummit
---------
The agenda for today (and tomorrow) is available [here](https://wiki.freebsd.org/201606DevSummit#Schedule).

You can find most of the slides of today's presentations (and tomorrow's soon) [here](https://assets.keltia.net/photos/BSDCan-2016/Devsummit-slides/index.html).  I think it makes looking at the picture easier, don't you think?

It seems that Hell has frozen over here in Canada because not only we had a very interesting presentation by Microsoft about FreeBSD support in their Cloud offering called Azure but they also sponsored the devsummit!

{% img https://assets.keltia.net/blog/blog-13376.jpg "MS <3 FreeBSD" "MS <3 FreeBSD" %}

To summarize: not only FreeBSD has been supported by Microsoft on Azure in 2014 (with support for Hyper-V and stuff) but they now have it available on the Azure Marketplace, meaning they have engineers to do the support, just like any other supported OS.  While there are many things that could be said about them (just witness the PR disaster that is W10), they are not the same company as before.  We'll see how it goes.

{% img https://assets.keltia.net/blog/blog-13385.jpg "10.3 on Azure" "10.3 on Azure" %}

Next presentation was from Intel about their QuickAssist Driver (and its port to FreeBSD).  QuickAssist is a driver made for high-speed hardware support for cryptography & compression.  It is already supported on Linux and they want to make it on par feature-wise on FreeBSD.

Then lunch \o/

{% img https://assets.keltia.net/blog/blog-8289.jpg "Lunch" "Lunch" %}

The afternoon is divided into working groups as per the schedule, I stayed in DMS1160 for the Toolchain session.

Lots of things going on there as you can see on this agenda:

{% img https://assets.keltia.net/blog/blog-13450.jpg "Toolchain" "Toolchain" %}

We are still struggling with the remains of our ancient toolchain based on GPLv2 tools and we use more and more the external ports-based toolchain, especially for architectures not using Clang.  Sparc is still an issue and we are not decided whether to keep the support for in inside the tree or not.  Progress has been made on both `lld` and `LLDB`.

The day ended with the devsummit dinner with Pizza, softs and beer in the hacking lounge back at the residence (sponsored by Intel this time).

{% img https://assets.keltia.net/blog/blog-13466.jpg "Dinner" "Dinner" %}

Pictures
--------

Like the last few years, I've taken a few pictures :)  Be sure to visit every day for updates!

[BSDCan 2016](https://assets.keltia.net/photos/BSDCan-2016/)

{%footnotes_inline%}
