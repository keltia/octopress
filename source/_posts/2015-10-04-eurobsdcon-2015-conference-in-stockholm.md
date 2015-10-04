---
layout: post
title: "EuroBSDCon 2015 conference in Stockholm — Day 1"
date: 2015-10-04 09:38:22 +0200
comments: true
sharing: true
categories: freebsd conference eurobsdcon english stockholm sweden
---

This is a followup post on the one about the [EuroBSDCon](/categories/eurobsdcon) [FreeBSD](/categories/freebsd) [devsummit](/categories/devsummit) that you can find [here](/2015/10/02/freebsd-devsummit-in-stockholm-eurobsdcon/).

This conference is dedicated to the late [Paul Schenkeveld](https://assets.keltia.net/photos/PaulS/) who passed away a the beginning of the year.  Paul was President of the EuroBSDCon Foundation and a friend to us all.
 
{% img https://assets.keltia.net/blog/paul-11394.jpg "Farewell Paul" "Farewell Paul" %}
<!--more-->

The conference has three different tracks so I will not be able to report on all of there but one must know that all talks are taped and are/will available on [Youtube](https://2015.eurobsdcon.org/live-streaming/) for live-streaming.

Keynote
-------

[Paul Vixie](https://twitter.com/paulvixie) was invited to do the keynote and he delivered a nice piece of his own history along with Internet, ISC and Bind-related bits of course.  Quite funny indeed.

{% img https://assets.keltia.net/blog/paulvixie-11408.jpg "Bind 8 is DEAD!" "Bind 8 is DEAD!" %}

## Day 1

The first talk I selected was Andrew Turner's one on the ARM64 architecture (also called ARMv8) which representes the next step for FreeBSD's embedded systems support.  It is interesting to see how architecture can get so much better when you are not constrained by something like backward compatibility (Intel, I'm looking at you!).

Then after lunch, [John-Mark Gurney](https://twitter.com/encthenet) takled about his work at Netflix on how to improve the throughput of crypto code, something that is of course interesting both to Netflix and the [FreeBSD Project](https://www.FreeBSD.org/) as crypto is getting used more and more.

{% img https://assets.keltia.net/blog/jmg-11429.jpg "John-Mark Gurney" "John-Mark Gurney" %}

[Michael Dexter](https://twitter.com/michaeldexter) was next to speak about the various virtualization options available to FreeBSD, from jails to finally [Bhyve](http://bhyve.org/).  He announced that from that day on, all versions of Windows (starting at 7) were finally supported in Bhyve…

After the coffee break, I went to see [Jordan Hubbard](https://twitter.com/omgjkh) talk about [NextBSD](http://nextbsd.org/).  The fine folks at [IX Systems](https://www.ixsystems.com/) are picking stuff from OS X in order to push FreeBSD into the 21st Century where you have dynamic devices, embedded systems with parts going off and on at any time.  This is important for all BSDs with libraries like `libdispatch`(for heavy threading), ASL and maybe even `launchd`.

{% img https://assets.keltia.net/blog/jkh-7202.jpg "libdispatch" "libdispatch" %}

The last talk for the day was Scott Long's one on disk performance and how he improved the `mps` driver with multi-queue support and other stuff as [Netflix](https://www.netflix.com/) surely can use the additional bandwidth :)

Last part of the day was the Social Event at the National Musem of Natural History in which we watch a nice (albeit sad) movie called the "Coral Reef Adventure" in the [iMAX theatre](http://www.cosmonova.se/english/visitthemuseum/cosmonova/aboutcosmonova.5715_en.html).  Then we had a nice dinner at the Restaurant Fossilen inside the museum.

{% img https://assets.keltia.net/blog/museum-7208.jpg "Geeks!" "Geeks!" %}

Pictures
--------

As usual, all pictures are available [there](https://assets.keltia.net/photos/EuroBSDCon-2015/).

{%footnotes_inline%}
