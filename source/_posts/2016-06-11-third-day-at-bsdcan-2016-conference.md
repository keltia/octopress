---
layout: post
title: "Third day at BSDCan 2016 conference"
date: 2016-06-11 15:54:05 +0200
comments: true
sharing: true
categories: freebsd conference bsdcan english ottawa
---

(followup on [previous article](/2016/06/10/second-day-at-bsdcan-2016-devsummit/))

Dan officially opened the conference as usual, under supervision by [Groff](https://twitter.com/GroffTheBSDGoat) of course, now a regular attendee of all conferences :)

{% img https://assets.keltia.net/blog/blog-13530.jpg "Dan & Groff" "Dan & Groff" %}
 
{% img https://assets.keltia.net/blog/blog-13533.jpg "Groff" "Groff" %} 
<!--more-->
We seem to have a lot of newcomers this year as illustrated by all the people raising their hands.

{% img https://assets.keltia.net/blog/blog-13528.jpg "Newcomers" "Newcomers" %} 

There was some hardware donations during this opening session, with [Shawn Webb](https://twitter.com/lattera) giving away RPi3 to several people like the newest committer in any BSD, the oldest one and so on. TL; DR: Kirk & Rod won one :)

{% img https://assets.keltia.net/blog/blog-13534.jpg "Shawn & Dan" "Shawn & Dan" %} 

Like last year, BSDCan is having an additional track which means 33% more talks \o/

Morning
-------
Of course I can't go to  every talk to as usual, I had to choose.

Started with a talk about what is {% wp Virtual_Extensible_LAN "VXLAN" %}, a way to create lots of VLAN-like kind of network over UDP/multicast.  It was created by VMWare and has been implemented in all the major OS like FreeBSD, OpenBSD and Linux (in addition of ESX and cisco).

{% img https://assets.keltia.net/blog/blog-13547.jpg "VXLAN" "VXLAN" %} 

Next was the Capsicum/Casper talk on what was Capsicum at the beginning and how casper was born, first as a daemon ad next as a library.  Interesting comparisons with `pledge(2)` was well.

{% img https://assets.keltia.net/blog/blog-13558.jpg "Sandboxing" "Sandboxing" %} 

During the lunch break, we had a nice OpenZFS BoF with both [Matthew Ahrens](https://twitter.com/mahrens1) and [AllanJude](https://twitter.com/AllanJude), the former being one of the original authors of ZFS back at Sun.

{% img https://assets.keltia.net/blog/blog-13569.jpg "Matt on SoonInZFS" "Matt on SoonInZFS" %} 

It is exciting to see who ZFS has kept on growing since the fork from Oracle, we will finally have encryption support in OpenZFS \o/

The next talk was about fighting the current streak of Monoculture happening in Tor where most of the nodes (relays and exit ones) are mostly Linux boxes; like in any monoculture, flaws and weaknesses spread faster.  Some of the figures are really bad :(

{% img https://assets.keltia.net/blog/blog-13573.jpg "By OS" "By OS" %} 

{% img https://assets.keltia.net/blog/blog-13574.jpg "Bandwidth monoculture" "Bandwidth monoculture" %} 

Then I had this talk about how PAM became the nightmare it is right from the beginning at Sun to OpenPAM and the other stuff.  [Groff](https://twitter.com/GroffTheBSDGoat) was there as well to supervise Michael Lucas' talk :)

{% img https://assets.keltia.net/blog/blog-13581.jpg "Groff" "Groff" %} 

The end of the day was another talk by [Matthew Ahrens](https://twitter.com/mahrens1) about some performances (up to like 2x faster!) improvements for writes in OpenZFS. This will be upstreamed soon and be in OpenZFS next year or so.
 
{% img https://assets.keltia.net/blog/blog-13585.jpg "OpenZFS" "OpenZFS" %} 

End of day one, pictures as usual [there](https://assets.keltia.net/photos/BSDCan-2016/)

{%footnotes_inline%}
