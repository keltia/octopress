---
layout: post
title: "Calife 3.0.5 is out!"
date: 2014-11-10 17:04:24 +0100
comments: true
sharing: true
categories: calife software english c
---

Minor upgrade for [Calife](https://www.keltia.net/programs/calife/), now at 3.0.5.  I updated the GNU utilities `config.guess` and `config.sub` that recognize and help GNU `autoconf` to do its jb.  I also added another {% wp Pluggable_authentication_module PAM %} module for FreeBSD9.x and above, using the default configuration files already present in the system instead of rolling my own (courtesy of [Dag-Erling Smørgrav](http://blog.des.no/)).

It is available on my [Bitbucket](https://bitbucket.org/keltia/calife/downloads) and [Gibhub](https://github.com/keltia/calife/releases) repositories.  There is a `fingerprints` file signed with my {% wp GNU_Privacy_Guard GPG %} key.  Please, check the signature before using the files. BTW, the GPG key is [here](https://www.keltia.net/keys/8BE879B028731E1C.asc)

Soon in the FreeBSD ports tree.

{%footnotes_inline%}
