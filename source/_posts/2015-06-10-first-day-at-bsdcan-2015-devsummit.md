---
layout: post
title: "First day at BSDCan 2015 - devsummit"
date: 2015-06-10 23:05:44 +0200
comments: true
sharing: true
categories: freebsd devsummit bsdcan english ottawa
---

After the series of articles I did for EuroBSDcon [here](/2014/09/25/first-day-in-sofia/), let's begin this new series on [BSDCan 2015](http://2015.bsdcan.org/)!

As usual, we will have two days of both tutorials and [FreeBSD](https://www.FreeBSD.org/) devsummit, a regular event in almost all BSD-related conferences now.
<!--more-->
The Goat BoF
------------
BSDCan didn't actually started today but a few jours before because, like last year (see the [pictures](http://assets.keltia.net/photos/BSDCan-2014/Goat-BoF/)), we did the "Groff the Goat" {% fnin %}Groff is the name of the goat, it has its own [Twitter account](https://twitter.com/groffthebsdgoat), it was seen in [EuroBSDCon](http://assets.keltia.net/photos/EuroBSDCon-2014/Conference/slides/conference-32885.html) and AsiaBSDCon :){% endfnin %} birds-of-a-feather session at the Royal Oak pub.

Just an excuse for getting the first beers into your system and do the social thing :)

{% img http://assets.keltia.net/blog/blog-08938.jpg "Watching geeks" "Watching geeks" %}

Pictures for yesterday's session are [there](http://assets.keltia.net/photos/BSDCan-2015/Goat%20BoF/).

Devsummit
---------
The agenda for today (and tomorrow) is available [here](https://wiki.freebsd.org/201506DevSummit#Schedule).

{% img http://assets.keltia.net/blog/blog-08981.jpg "devsummit" "devsummit" %}

We started with a very interested presentation by [Nathan Dautenhahn](https://twitter.com/kainospur) about protecting the kernel by creating a nested one that control the {% wp Memory_management_unit "MMU" %} a critical part of the {% wp Virtual_memory "VM" %} subsystem.  The goal is to protect the system from the situations where an attacker has managed to insert code in the kernel" (through an extension for example) and is trying to hide itself there (common with {% wp Rootkit "rootkits" %}).

{% img http://assets.keltia.net/blog/blog-09015.jpg "Nathan" "Nathan" %}

Some slides:

{% img http://assets.keltia.net/blog/devsummit-09018.jpg "high-level arch." "high-level arch." %}

{% img http://assets.keltia.net/blog/devsummit-09023.jpg "priv. separation." "priv. separation." %}

{% img http://assets.keltia.net/blog/devsummit-09025.jpg "services." "services." %}

The entire presentation is available on [Prezi](https://prezi.com/hlylrelpxkfj/nested-kernel-presentation-general-purpose-45-min/).

Then we had a presentation by [Benno Rice](http://assets.keltia.net/photos/BSDCan-2015/Devsummit%20Day%201/content/DSF09054_large.html) on Isilon's usage of FreeBSD, mainly on the way they try to sync their own changes with our main tree.

The afternoon was divided into [working groups](https://wiki.freebsd.org/201506DevSummit#Working_Groups) and I was registered on the [one on configuration files](https://wiki.freebsd.org/201506DevSummit/UCL).  Very interesting discussions on UCL itself first and the way we could move several utilities to UCL instead of their own home-grown format.

UCL is an interesting [library and file format](https://github.com/vstakhov/libucl) written by [Vsevolod Stakhov](http://assets.keltia.net/photos/BSDCan-2015/Devsummit%20Day%201/content/DSF09085_large.html) that able to parse and use several other file formats in addition to its own (like JSON and YAML).  It is already used by [pkgng](https://wiki.freebsd.org/pkgng) used to manage binary packages in FreeBSD.

Hacking lounge
--------------
At the end of all conference days, we have people going into the hacking lounge at the Univertsity residence and, like today, even have dinner there.

{% img http://assets.keltia.net/blog/blog-09098.jpg "Hacking lounge" "Hacking lounge" %}

Of course it had to be pizza {% fnin %}Ok, not always pizza, we will have Thai food tomorrow I believe :){% endfnin %} !

Before:

{% img http://assets.keltia.net/blog/blog-09097.jpg "Geeky food!" "Geeky food!" %}

Almost finished:

{% img http://assets.keltia.net/blog/blog-6643.jpg "Massacre" "Massacre" %}

Of course, some people have to have to play with hardware :)

{% img http://assets.keltia.net/blog/blog-09099.jpg "Hardware hacking" "Hardware hacking" %}

All in all, a very productive day!

Links
-----

- [My pictures](http://assets.keltia.net/photos/BSDCan-2015/)
- [FreeBSD wiki](https://wiki.freebsd.org/201506DevSummit)
- [BSDCan site](http://2015.bsdcan.org/)

Notes
-----
{%footnotes_inline%}
