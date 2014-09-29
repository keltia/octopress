---
layout: post
title: "EuroBSDCon Conference begins!"
date: 2014-09-27 14:02:27 +0300
comments: true
categories: conference sofia eurobsdcon english
---

Very busy day today at the [EuroBSDCon 2014](http://2014.eurobsdcon.org/) conference in Sofia, Bulgaria as I had to chair one entire track from morning to evening.

That means assuring the speakers are there on time, introducing each of them in a few words and managing questions after the talk is finished (while managing the time of course).
<!--more-->
To be honest, I choose to chair this session mostly because it had all the sessions I wanted to attend so it was mixing pleasure and work :)

Interesting keynote on [FreeBSD: the next 10 years](http://2014.eurobsdcon.org/talks-and-schedule/talks/#JordanHubbard) by [Jordan Hubbard](http://en.wikipedia.org/wiki/Jordan_Hubbard), old-time BSD hacker, FreeBSD founder, former Apple executive for MacOS X and now CTO at [iX systems](http://ixsystems.com/), home of [PC-BSD](http://www.pcbsd.org/) and [FreeNAS](htto://www.freenas.org/).

TL; DR: be open to new hardware & software features, mobile computing and embedded are more important than desktop right now.

{% img http://assets.keltia.net/photos/EuroBSDCon-2014/Conference/medium/conference-32882.jpg 'Jordan Hubbard' 'Jordan Hubbard Keynote' %}

[Kris Moore]() talked about the new tools they have developped in [PC-BSD](http://www.pcbsd.org/) to deal with advanced features of [ZFS]() (automated and scheduled snapshot, use of Grub for having an encrypted zfs-on-root system with onely one pool and so on.).

[Kirk](http://mckusick.com/) gave us an interesting talk on [ZFS](http://en.wikipedia.org/wiki/ZFS) internals implementation, something we do not see often (who has not seen Matt Ahrend's talk yet? :)) so thanks Kirk.

{% img http://assets.keltia.net/photos/EuroBSDCon-2014/Conference/medium/conference-32891.jpg 'Kirk McKusick' 'Kirk ZFS' %}

Next talk was John-Mark Gurney's talk about optimizing [GELI](http://en.wikipedia.org/wiki/Geli_(software\)) performance, while keeping sane and readable code, something which is not always easy when dealing with crypto code.  Lots of interesting bits here even though I've heard the talk before at [BSDCan](http://bsdcan.org/).

Emmanuel Dreyfus then talked about [FUSE](http://en.wikipedia.org/wiki/FUSE) enhancements [NetBSD](http://www.netbsd.org/) have done, especially with the link to [PUFFS](http://www.netbsd.org/docs/puffs/), the FS framework they have been using for a long time.

Then an interesting session on using [Lua](http://en.wikipedia.org/wiki/Lua_(programming_language\)) as an extension language for the NetBSD Packet Filter (NPF).  Quite a few questions on security and memory management, not sure they have all be answered.

 Andy Tanenbaum (yes, THE Andrew S. Tanenbaum himself) was next (and the last session) to talk about a few students and he reimplemented [Minix3](http://en.wikipedia.org/wiki/MINIX#MINIX_3){% fnin %}Yes I'm linking to the WP page and not the actual `http://www.minix3.org/` site because it seems broken at the moment.{% endfnin %} using the NetBSD userland.  Minix3 is a very interesting OS that does many things completely different.  Being a small micro-kernel (only 13k LOC) enables it to be very modular with most of its features actually running in userspace, which makes upgrades very easy and live (yes, including the filesystem).

 Awesome presentation, I'm really happy we got him on board at the conference.

 {% img http://assets.keltia.net/photos/EuroBSDCon-2014/Conference/medium/conference-32915.jpg 'Andrew S. Tanenbaum' 'Andy Tanenbaum Minix3' %}

Great way to end this first day of talks.

As usual, more pictures [there](http://assets.keltia.net/photos/EuroBSDCon-2014/Conference/index.html).

{%footnotes_inline%}
