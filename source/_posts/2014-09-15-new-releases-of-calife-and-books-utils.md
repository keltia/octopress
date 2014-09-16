---
layout: post
title: "New releases of calife &amp; books-utils"
date: 2014-09-15 15:47:37 +0200
comments: true
categories: software calife books-utils ruby english C
---

I have a few software utilities, from long ago (esp. [Calife](https://www.keltia.net/programs/calife/) for which I release new versions.  I'll now announce them right here :) 

### Calife

I just issued release 3.0.4 of [Calife](https://www.keltia.net/programs/calife/). Please test.  You can find it on my [Bitbucket](https://bitbucket.org/keltia/calife/downloads) or [Github](https://github.com/keltia/calife/releases) repositories.  There is a `fingerprints` file signed with my GPG key.  Please, check the signature before using the files. 

I just issued release 3.0.4 of [Calife](https://www.keltia.net/programs/calife/). Please test.  You can find it on my [Bitbucket](https://bitbucket.org/keltia/calife/downloads) or [Gibhub](https://github.com/keltia/calife/releases) repositories.  There is a `fingerprints` file signed with my GPG key.  Please, check the signature before using the files. BTW, the GPG key is [here](https://www.keltia.net/keys/8BE879B028731E1C.asc)

I added the `%group` syntax in addition to the current `@group` one. It also uses a more secure `memzero(3)` routine.  It is also in the FreeBSD ports tree.

### Books-Utils

Release 0.4.0 of [books-utils](https://github.com/keltia/books-utils) is available.

`books-utils` is intended to be a [Ruby](https://www.keltia.net/programs/ruby/) gem with utilities dealing with e-book management, generally associated with the wonderful [Calibre](https://www.keltia.net/programs/calibre/) utility. 

It mainly consists of (for now) the `newer-than` script that look into a Calibre database for new books and display this list in various formats ([json](https://en.wikipedia.org/wiki/JSON), [xml](https://en.wikipedia.org/wiki/XML) and [yaml](https://en.wikipedia.org/wiki/YAML)) and/or send it to [Pastebin](http://pastebin.com/) a popular copy-paste site and/or generate a [Zip file](https://en.wikipedia.org/wiki/Zip_%28file_format%29) with all files.  The code is on [Github](https://github.com/keltia).
