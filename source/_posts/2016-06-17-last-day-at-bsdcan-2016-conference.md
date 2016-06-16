---
layout: post
title: "Last day at BSDCan 2016 - conference"
date: 2016-06-17 00:31:53 +0200
comments: true
sharing: true
categories: freebsd conference bsdcan english ottawa
---
(followup on [previous article](/2016/06/11/third-day-at-bsdcan-2016-conference/))

The last day of BSDCan is always special: all talks start at 10AM instead of the usual 9AM to account for the preceding night, generally filled with beer and food for some reasons :)  It is also when the famous auction is taking place.  During the closing session, Dan will auction a few items and the money given to the Ottawa Mission charity.  He does that also with PGcon, the equivalent of BSDCan for [Postgresql](https://www.postgresql.org/).

{% img https://assets.keltia.net/blog/blog-13656.jpg "Auctioning" "Auctioning" %}

But for now, the talks!
<!--more-->
Talks
-----
I started with an interesting talk about a different way to test a given software package (in that case, the FreeBSD kernel): instead of testing for what we know works, we will try to make the kernel crash by doing the unexpected.  When that is achieved, we try to insolate the reason and thus find the bug.

{% img https://assets.keltia.net/blog/blog-13607.jpg "Kernel fuzzing" "Kernel fuzzing" %}

Then, one of most interesting talk for me today.  Rod Grimes is one of founders of the FreeBSD project, after creating the famous 386BSD Patchkit with {% wp Jordan_Hubbard "Jordan Hubbard" fr %}, Terry Lambert and Nate Williams.  David Greenman coined the name "FreeBSD" and they started it.  Rod Grimes gave us the history of these early days and I'm a sucker for this kind of talk :)

{% img https://assets.keltia.net/blog/blog-13615.jpg "Rod Grimes" "Rod Grimes" %}

The thing is, I was there like many 386BSD users both on the mailing-lists and the Usenet newsgroups and it was nice to hear this from himself.  The talk was so popular it had to be moved into the larger room to fill everyone (despite the excellent talks at the same time, sorry guys!) :)

After lunch, I attended the talk from Bernard Spil about the state of OpenSSL/LibreSSL, the latter being a fork of OpenSSL by the OpenBSD guys.  [Miod Viallat](https://twitter.com/MiodVallat), Bob Beck and others started a very large and much needed cleanup of the ancient codebase.  Who needs VAX code now?  Or code for some never-released big-endian i386 (yes, the code for this did exist).

{% img https://assets.keltia.net/blog/blog-13626.jpg "Versions" "Versions" %}

Bernard is working on upgrading the OpenSSL in [HardenedBSD](https://www.HardenedBSD.org/) and [FreeBSD](https://www.FreeBSD.org/) to LibreSSL.

The next talk was by Saen Chittenden who has been working on facilitating build managements for creating images with tools such as [Vagrant](https://www.vagrantup.com/) and [Packer](https://packer.io/), pushing them to some cloud like Digital Ocean or AWS and using tools like [Puppet](https://www.puppet.com/) or [Ansible](https://www.ansible.com/) to manage them.

The idea of reproducible builds has been floating around for some time now and other OSS projects like [Debian Linux](https://debian.org/) have started to implement them.  [Ed Maste](https://twitter.com/ed_maste) talked about the status of reproducible build in FreeBSD, both on the base and ports sides.  

{% img https://assets.keltia.net/blog/blog-13636.jpg "TODO in base" "TODO in base" %}

Then… THE AUCTION!
------------------

Every BSDCan (at least from 2005 which was the first one I attended) had had the auction and it is always a fun moment at the end of the conference.  This year, the fine folks at [iXsystems](https://www.ixsystems.com/) donated a 8-drive FreeNAS-based TrueNAS system!  One of the items this year was a towel made by the [RIPE NCC](https://www.ripe.net/) for {% wp Towel_Day "Towel Day" %} :)

{% img https://assets.keltia.net/blog/blog-13681.jpg "Auctioning" "Auctioning" %}

George Neville-Neil also had a special item to auction: one of the rare FreeBSD Foundation shirt while he was wearing it which leads up to… him taking the shirt off in front of everybody :)  The pictures are on my site (see below) and I got some success with my tweet about it {% fnin %}[Here it is :)](https://twitter.com/Keltounet/status/741763867471155201){% endfnin %}

The [FreeBSD Foundation](https://www.freebsdfoundation.org/) then gave gifts to four people that have done great things to FreeBSD: there was Rod Grimes of course with Warren Block (for his work on documentation), Brian Dewery (for his work on build management) and Gleb Smirnoff (security stuff).

{% img https://assets.keltia.net/blog/blog-13671.jpg "Brian, Rod and Warren" "Brian, Rod and Warren" %}

Our dear friend [Groff](https://twitter.com/GroffTheBSDGoat) got in the care of [Gavin Atkinson](https://twitter.com/gavinatkinson) (who will bring him to the next devsummit in Cambridge: [BSDCam]()) after being brought to Canada from Japan by OpenBSD dev [Henning Brauer](https://twitter.com/HenningBrauer).

{% img https://assets.keltia.net/blog/blog-13676.jpg "From Henning to Gavin" "From Henning to Gavin" %}

And do not forget the next conference in line, [EuroBSDCon 2016](https://www.eurobsdcon.org/) in Belgrade, Serbia!

{% img https://assets.keltia.net/blog/blog-13674.jpg "EuroBSDCon 2016" "EuroBSDCon 2016" %}

Thanks to Dan and everyone working to make BSDCan such a success!

Pictures
--------
Did I ever entioned I take pictures at every BSD conference I go? :)
Go to [the usual place](https://assets.keltia.net/photos/BSDCan-2016/) to see them :)

So long BSDCan and thanks for all the fish!

Notes
-----
{%footnotes_inline%}
