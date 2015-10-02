---
layout: post
title: "FreeBSD devsummit in Stockholm — EuroBSDCon 2015"
date: 2015-10-02 09:52:30 +0200
comments: true
sharing: true
categories: freebsd devsummit eurobsdcon english stockholm sweden
---

…and we are back for a new BSD-related conference :)

Now we are talking about the [FreeBSD](/categories/freebsd) [devsummit](/categories/devsummit), taking place two days before the [EuroBSDCon](https://2015.eurobsdcon.org/) conference.  This year, it is in Stockholm, Sweden.

Like last year in [Sofia, Bulgaria](/2014/09/25/first-day-in-sofia/), it is a smaller conference and devsummit compared to [BSDCan](/2015/06/10/first-day-at-bsdcan-2015-devsummit/).  The list of topics is available on the [FreeBSD wiki](https://wiki.freebsd.org/201510DevSummit).

Our hosts this year are the company called [Init](https://www.init.se/), big thanks to them!
<!--more-->
{% img http://assets.keltia.net/blog/devsummit-11284.jpg "Devsummit starting" "Devsummit starting" %}

Packaging base
--------------

This is of course an important subject and we got an update on the work done by `bapt@` on this.  He is working off a branch of current, first with rather big packages that will be probably broken down into small ones later as needed.

See [the agenda](https://wiki.freebsd.org/201510DevSummit/PackagingBase) for the list of things that were discussed.

Callout
-------

I didn't go to the session `hps@`organized on the `callout` subsystem in FreeBSD but here are [some notes](https://etherpad.net/p/Callout2015).

Virtualization
--------------

I didn't go to that one but you can find the [agenda](https://wiki.freebsd.org/201510DevSummit/Virtualization) and some notes taken [here](https://etherpad.net/p/2015DevSummitVirtualization).

Recruiting
----------

This session was to discuss how to invite and get more people working on FreeBSD, a rather important topic.  Here are the [notes](https://etherpad.net/p/2015Dev_Summit_Recruiting) taken during the session.

Embedded
--------

That one went pretty slow, with no real topics pre-defined so we got some updates on how ARM/ARM64 are doing, some of the issues.  Notes [here](https://etherpad.net/p/2015DevSummitEmbedded).

Of course, [Groff](https://twitter.com/GroffTheBSDGoat) the goat joined us on the second day, too busy touring Stockholm on the 1st one I guess :)

{% img http://assets.keltia.net/blog/devsummit-11314.jpg "Groff" "Groff" %}

Roadmap for jails
-----------------

Agenda is [here](https://wiki.freebsd.org/201510DevSummit/Jails).  Topic seems to interest a lot of people for some reason :) See the pano picture:

{% img http://assets.keltia.net/blog/IMG_7170.JPG "Jails" "Jails" %}

We talked about converting `jail.conf` into UCL, some of the grammar is delicate, how to deal with `pkg(8)` itself to install packages inside a jail directly and so on.

Pictures
--------

As usual I have created a gallery for the pictures I'll be taking at the conference ,so heads out to [here](http://assets.keltia.net/photos/EuroBSDCon-2015/) to see them.

{%footnotes_inline%}
