---
layout: post
title: "New mfsbsd tutorial out for FreeBSD 11.x"
date: 2017-09-03 15:43:52 +0200
comments: true
sharing: true
categories: freebsd mfsbsd english tutorial
---

## Preambule

You may remember these articles I posted a while ago in the "howtos" category on my [website](https://www.keltia.net/).  I had two pf them on my ZFS-on-root setup, [one on FreeBSD 8.2](https://www.keltia.net/howtos/mfsbsd-zfsv28/) for a local machine and one for a [remotely managed server on FreeBSD 9.2](https://www.keltia.net/howtos/mfsbsd-zfs91/).

The most important one was the latter as I moved all my services on dedicated servers hosted in datacentres (all managed by [Online](https://www.online.net/){% fnin %}You may have noticed there is this slightly bigger and and even more well-known French hosting provider called OVH.  They seem to have weird technical design choices (like watercooling), an even more weird network setup (can you say fscked up IPv6?) and some "interesting" notions on spam filtering I happen to disagree with.  In short, I do not trus them for my stuff.{% endfnin %}).

My most heavily used machine at Online is getting old now by today's standards and, to stay within the scope of the aforementioned articles, lacking the cryptographic hardware extenstions in its CPU (an [Intel Xeon L3426](http://ark.intel.com/products/43233/Intel-Xeon-Processor-L3426-8M-Cache-1_86-GHz) — as you can see, old :)).

While I was just running my web & mail site out of it, I do not really need blazing fast disks (or I'd have taken SSD) but still, now that I'm sharing stuff with the [Transmission](http://www.transmissionbt.com/) P2P client and building my own set of FreeBSD packages for the host and its [jails](https://www.keltia.net/howtos/jail-mgmt-with-ansible/) with [Poudriere](https://github.com/freebsd/poudriere/wiki), the bandwidth limitation is taking its toll (35 MB/s without the {% wp AES_instruction_set "AES-NI" %} instructions vs 150 MB/s).

I may also running out of disks space (ahem), the disks are 90% filled…

## Remote Management

There is also this slightly (read: enormously) annoying thing with both HP and Dell machines, their remote management systems (known as {% wp Intelligent_Platform_Management_Interface#Baseboard_management_controller "BMC" %}), respectively iLO and iDRAC, just *sucks*.  These thingy require either a .Net machine (read: Windows) or a Java applet to be run to be able to access the remote console.  The keyboard when running the java applets is completely fscked up (not to mention heavily biaised toward QWERTY ones).  I just hate them.

So, after looking for some time for a replacement machine at Online (and even on other providers such as [Hetzner](https://www.hetzner.com/?country=gb) in Germany) and experimenting with another one here (a 2013 dedibox on an HP DL120G7 machine), I finally took another machine at Online, the new 2017 ST8.

It is a Dell R210 machine (iDRAC is slightly less cumbersome than iLO from HP) and while it is still using an oldish Xeon processor (the [E3-1220V2](http://ark.intel.com/products/65734/Intel-Xeon-Processor-E3-1220-v2-8M-Cache-3_10-GHz)), it is way better than the L3426 and it has the AES-NI instruction set.  The nice thing is also that after two-three years of reducing the hard disks from 2 TB to 1 TB to cut costs, they got to put 2 4 TB disks which means two times as much disk space \o/

Considering the issues I had with the previous machines and the BMC, and following some discussions with a Linux (now FreeBSD) friend, I decided to find a setup where I do not rely on the BMC for the most simple task of all: rebooting!  With my previous setups , I had to log on the BMC, run the virtual machine then I could have access to the early boot stages when the GELI passphrase is supposed to unlock the encrypted pool duing boot.

If you add the keybaord mapping issues I also mentioned you can see why such a setup is not only necessary but also better on my nerves :)   In the last days of "oldnext", the HP machine that was supposed to replace the main one, I was not able to connect to the iLO system at all.  Very frustrating.

## mfsbsd

You may recall that I started using [mfsbsd](http://mfsbsd.vx.sk/) to bootstrap the installation of the remote system as FreeBSD was not a usable option for the "Rescue System" (it is now).  I started to thing that mfsbsd would be a good system to boot the entire system on, enabling me to ssh into the machine to unlock the encrypted pool, thus removing the need to use the BMC.

During these years, two things happened, one is the availability of FreeBSD as an installaton (alas just with {% wp Unix_File_System "UFS" %}) & rescue system at Online and the second is an interesting addition to the `reboot(8)` utility: the `-r` flag.  This flag allows the system to everything regular reboot does except rebooting it the kernel itself.  That way, you can change the root-to-be filesystem, shutdown all processes and restart with the new root.

I can now install a system with mfsbsd, boot from there, unlock the encrypted pool and "reboot" into it \o/

Only constraint is to keep the mfsbsd partition in sync with any kernel change (including modules) as you are still running that mfsbsd kernel but you will load modules from the encrypted pool.

There are some pieces missing (like the script that will do the `reboot -r` thing) but the tutorial is online as a Work-In-Progress [there](https://www.keltia.net/howtos/mfsbsd-zfs11/).

As usual, all comments and corrections are welcome. 

{%footnotes_inline%}
