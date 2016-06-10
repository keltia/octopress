---
layout: post
title: "Second day at BSDCan 2016 devsummit"
date: 2016-06-10 02:57:55 +0200
comments: true
sharing: true
categories: freebsd devsummit bsdcan english ottawa
---

Second day of the devsummit at BSDCan. One very important session on the morning, the one about what was finally put into upcoming 11-RELEASE and what we want to have (or at least try to) for release 12.0.  See below.

This is a followup on yesterday's [post](/2016/06/09/first-day-at-bsdcan-2016-devsummit/)

{% img https://assets.keltia.net/blog/blog-13510.jpg "my Group photo" "my Group photo" %}
<!--more-->
What's cookin' for 12?
----------------------
It has become some kind of a tradition during the BSDCan's devsummit to more or less give ourselves a set of goals for the next major release.  But before, as 11.0 is really around the corner, we did a list of what is in 11.0.

The list if always more impressive than many think.  Have a look at the different pictures I got in [the slides section](https://assets.keltia.net/photos/BSDCan-2016/Devsummit-slides/index_2.html); the first two are what we had in mind before really thinking about it, the next two or three are the really long list :)

Next, what we need / want for 12.  The main items being trying to get 12.0 GPL-free and have a proper replacement for the `rc.d` stuff which is showing its age now (whoever thought `systemd` can remove him- or herself out of here, thanks).

You can see the list of interesting things people want, including better external toolchain support and a few things about ZFS like compressed ARC and encryption.

You can find a more readable version [here](https://pad.riseup.net/p/FreeBSD_11_12).

FreeBSD Foundation
------------------
Then we has a short presentation by Deb and Justin about the [FreeBSD Foundation](https://www.freebsdfoundation.org/)

{% img https://assets.keltia.net/blog/blog-13498.jpg "Deb Goodkin" "Deb Goodkin" %}

That was following bu a Q&A session with the core team members present:

{% img https://assets.keltia.net/blog/blog-13504.jpg "Core team" "Core team" %}

After lunch was the traditional developers' photo by David Maxwell (and yours truly, see above).  I'm in the final one do not worry ;-)

{% img https://assets.keltia.net/blog/blog-13507.jpg "People arriving" "People arriving" %}

{% img https://assets.keltia.net/blog/blog-13512.jpg "Photographers" "Photographers" %}

The afternoon for me was more into general hacking & mail.  I began to have a second look at Poul-Henning's ntimed daemon (I hope to replace the ancient and frankly increasingly unsecure ntpd with it as soon as it gets more complete) and ended up writing a manpage for it :) ([GH pull request](https://github.com/bsdphk/Ntimed/pull/32)).

This day ended gloriously with Poutine :)

{% img https://assets.keltia.net/blog/blog-8314.jpg "Smoked meat Poutine" "Smoked meat Poutine" %}

While going back to the hackers' lounge in L140, I tried to get some pictures of the massive sinkhole that appeared very near the Rideau centre Mall yesterday.  This part around the centre has been closed to the public of course — by sheer luck no one was hurt which is almost unbelievable considering the amount of car and bus traffic going there…

{% img https://assets.keltia.net/blog/blog-13520.jpg "Sinkhole 1" "Sinkhole 1" %}

{% img https://assets.keltia.net/blog/blog-13521.jpg "Sinkhole 2" "Sinkhole 2" %}

and I tumbed upon that sign on a well-known pub near ByMarket :)

{% img https://assets.keltia.net/blog/blog-13523.jpg "Sign" "Sign" %}


Pictures
--------
Like the last few years, I've taken a few pictures :)  Be sure to visit every day for updates!

[BSDCan 2016](https://assets.keltia.net/photos/BSDCan-2016/)

{%footnotes_inline%}
