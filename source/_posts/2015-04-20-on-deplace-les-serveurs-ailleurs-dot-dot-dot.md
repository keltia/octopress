---
layout: post
title: "On déplace les serveurs ailleurs..."
date: 2015-04-20 11:10:42 +0200
comments: true
sharing: true
categories: politique renseignement opinion french rant libertés Internet censure
---

Comme prévu, le projet de loi sur le renseignement (voir mon billet précédent [ici](/2015/03/17/lettre-ouverte-a-nos-gouvernants/)) a été voté à l'Assemblée nationale le 16 avril 2015 avec notamment le vote — public cette fois-ci contrairement aux amendements — de l'article 2 sur les boîtes noires, équipements espions devant être implémentés chez les principaux opérateurs Internet et hébergeurs {% fnin %}Ne vous y méprenez pas, les boîtes noires sont déjà implantées chez les opérateurs majeurs, cette loi ne sert « qu'à » les légaliser...{% endfnin %}.
<!--more-->
L'hébergeur historique AlterN a déjà annoncé le déplacement de tous ses serveurs à l'étranger, tout comme EU.org, « fournisseur de noms de domaine gratuits depuis le siècle dernier ». Ayant participé un peu aux débuts de EU.org avec Pierre et le soutenant totalement dans sa démarche, j'ai décidé moi aussi de déplacer mes ressources/serveurs ailleurs.

J'ai donc un serveur de nom — `ns3.keltia.net` — configuré et fonctionnant depuis un autre pays (la Hollande pour l'instant, peut-être un autre serveur ailleurs plus tard), pris chez l'hébergeur de VPS {% fnin %}Virtual Private Server — une machine virtuelle hébergé sur un hôte avec un {% wp Hyperviseur "hyperviseur" fr %}.{%endfnin %} appelé Vultr.

C'est un hébergeur assez récent, qui a des points de présence en Europe, aux USA et ailleurs (Japon, Australie notamment). Ce sont des machines assez rapides avec des disques SSD pour le stockage. [FreeBSD](http://www.freebsd.org/) 10.1 est supporté, condition *sine qua none* pour moi :)

Si vous êtes intéressé-e pour avoir un serveur de noms secondaire hors France, contactez-moi :) — [contact](https://www.keltia.net/people/roberto/). IPv4 et IPv6 bien entendu, DNSSEC bienvenue et recommandé :)

Références
----------

- [Vote loi — NEXTINPACT](http://www.nextinpact.com/news/93837-loi-renseignement-compte-rendu-troisieme-journee-debats.htm)
- [Annonce AlterN](http://altern.org/)
- [Annonce EU.org](http://eu.org/loirens.html)

Notes
-----
{%footnotes_inline%}
