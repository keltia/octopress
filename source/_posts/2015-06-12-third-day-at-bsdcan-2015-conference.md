---
layout: post
title: "Third day at BSDCan 2015 - conference"
date: 2015-06-12 17:46:23 +0200
comments: true
sharing: true
categories: freebsd conference bsdcan english ottawa
---

(followup on [previous article](/2015/06/11/second-day-at-bsdcan-2015-devsummit/))

Introduction
------------

BSDCan is having more than 280 people this year and is having an additional track which means 33% more talks \o/

Dan officially opened the conference as usual after playing a bit with the video feed on his phone and we got both of us on the screen :)
<!--more-->
{% img http://assets.keltia.net/blog/blog-09212.jpg "Video fun" "Video fun" %} 

Could not resist taking a nice picture of upcoming keynote speaker Stephen Bourne.

{% img http://assets.keltia.net/blog/blog-09204.jpg "S. Bourne" "S. Bourne" %} 

Then Deb Goodkin took the stage to speak about the [FreeBSD Foundation](https://www.freebsdfoundation.org/), all the conferences and software they are sponsoring.

{% img http://assets.keltia.net/blog/blog-09218.jpg "Deb Goodkin" "Deb Goodkin" %} 

Keynote
-------

{% img http://assets.keltia.net/blog/blog-09224.jpg "S. Bourne" "S.Bourne" %}

Wonderful keynote by Stephen Bourne, Mr. /bin/sh about the history of, guess what?, `/bin/sh`, with a lot of reference to AT&T, BSD and Andy Tannenbaum {% fnin%}Andy is giving the same talk as he did last year at EuroBSDCon in Sofia, see [here](https://2014.eurobsdcon.org/talks-and-schedule/talks/index.html#AndrewTanenbaum){% endfnin %}.

Lots of nice stories and things-to-be-quoted like some did on Twitter…

{% blockquote @Keltounet https://twitter.com/Keltounet/status/609354466538733569 %}
Bourne: “if you touched a source file, you owned it” #BSDCan #QOTD
{% endblockquote %}

{% blockquote @lattera https://twitter.com/lattera/status/609360164492214272 %}
"I didn't believe in goto" -- Steve Bourne at #BSDCan
{% endblockquote %}

{% blockquote @Keltounet https://twitter.com/Keltounet/status/609365420131381248 %}
Bourne: “Even now, I don’t know how to debug shell scripts” #BSDCan #!/bin/sh
{% endblockquote %}

A few screenshots to illustrate the presentation :)

{% img http://assets.keltia.net/blog/blog-09222.jpg "keynote" "keynote" %}
{% img http://assets.keltia.net/blog/blog-09223.jpg "keynote" "keynote" %}
{% img http://assets.keltia.net/blog/blog-09226.jpg "keynote" "keynote" %}

Of course, Groff the Goat is there, helping Stephen for his talk :)

{% img http://assets.keltia.net/blog/blog-09228.jpg "Groff" "Groff" %}

{% blockquote @encthenet https://twitter.com/encthenet/status/609366721959301120 %}
Andy Tanenbaum watching Steve Bourne's keynote. [picture](http://t.co/72JEIth7EY)
{% endblockquote %}

Talks
-----

I'm afraid I missed the first session from Sean Bruno about [embedded package building](https://www.bsdcan.org/2015/schedule/events/532.en.html) with Qemu, talking with Andy Tannebaum and Peter Wemm.

{% img http://assets.keltia.net/blog/blog-09237.jpg "Tannenbaum" "Tannenbaum" %}

I got back into the room for the end of Sean's talk, I did not want to miss John-Mark Gurney's one on [AES-GCM crypto](https://www.bsdcan.org/2015/schedule/events/576.en.html).

{% img http://assets.keltia.net/blog/blog-09248.jpg "Sean" "Sean" %}

John-Mark talked about issues in AES-GCM & AES-ICM modes to OpenCrypto in FreeBSD.

{% img http://assets.keltia.net/blog/blog-09251.jpg "John-Mark" "John-Mark" %}
{% img http://assets.keltia.net/blog/blog-09253.jpg "AES-GCM" "AES-GCM" %}

(sorry, I didn't go to [Andy's talk](https://www.bsdcan.org/2015/schedule/events/597.en.html) in the other room, I've seen it last year in Sofia, see [this article](/2014/09/27/eurobsdcon-conference-begins/) for details).

bhyve BoF
---------

During lunch, there was also a [bhyve](http://bhyve.org/) BoF showing Windows 2012R2 running under it.

{% img http://assets.keltia.net/blog/blog-09254.jpg "Harware" "Hardware" %}
{% img http://assets.keltia.net/blog/blog-09255.jpg "with RDP" "With RDP" %}

Talks (cont.)
-------------

Next was George's talk on [measuring performance in the network stack](https://www.bsdcan.org/2015/schedule/events/528.en.html) in FreeBSD. TL; DR: Benchmarks are *hard*.

{% img http://assets.keltia.net/blog/blog-09261.jpg "George" "George" %}
{% img http://assets.keltia.net/blog/blog-09262.jpg "Hard" "Hard" %}

It is pretty obvious than in multi-core tests, Linux/iptables are way faster than the different BSDs (whether it is pfSense or plain FreeBSD 11).  Expect updates during the upcoming [vBSDCon conference](http://www.verisigninc.com/en_US/internet-technology-news/verisign-events/vbsdcon/index.xhtml) in Washington DC in September.

{% img http://assets.keltia.net/blog/blog-09265.jpg "Ouch" "Ouch" %}

Break
-----

The [FreeBSD Foundation](https://www.freebsdfoundation.org/) is celebrating its 15th Birthday and brought a very nice and large cake \o/  It went pretty fastthough with so many people in the conference…

{% img http://assets.keltia.net/blog/blog-09268.jpg "Cake" "Cake" %}
{% img http://assets.keltia.net/blog/blog-09281.jpg "Almost gone" "Almost gone" %}

Talks (cont.)
-------------

After the break, I went to the [RDMA / Infiniband](https://www.bsdcan.org/2015/schedule/events/586.en.html) by Shany Michaely from Israël. The aim is to transfer large amounts of data with low latency and minimal involvement from the CPU.

{% img http://assets.keltia.net/blog/blog-09288.jpg "Shany" "Shany" %}
{% img http://assets.keltia.net/blog/blog-09290.jpg "Infiniband" "Infiniband" %}

Looks very interesting to get fast transfert rates.

Then on with the last talk of the day, the one by Olivier Cochard-Labbé on [Large-scale plug&play x86 network appliance deployment](https://www.bsdcan.org/2015/schedule/events/555.en.html).

{% img http://assets.keltia.net/blog/blog-09299.jpg "Olivier" "Olivier" %}

Using Nanobsd and OpenVPN along with Ansible for configuration management and deployement. On a very large scale (244 M customers, large international network w/ 700,000 managed devices).

Differences between system and network admins :)

{% img http://assets.keltia.net/blog/blog-09300.jpg "Admins" "Admins" %}
{% img http://assets.keltia.net/blog/blog-09301.jpg "Solution" "Solution" %}

Links
-----

- [My pictures](http://assets.keltia.net/photos/BSDCan-2015/)
- [BSDCan 2015](http://bsdcan.org/2015/)
- [Bhyve](http://bhyve.org/)
- [FreeBSD Foundation](https://www.freebsdfoundation.org/)
- [NanoBSD](https://www.freebsd.org/doc/en_US.ISO8859-1/articles/nanobsd/)
- [OpenVPN](https://openvpn.net/)
- [Ansible](http://www.ansible.com/home/)

Notes
-----
{%footnotes_inline%}
