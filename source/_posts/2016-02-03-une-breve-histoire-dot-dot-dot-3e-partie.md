---
layout: post
title: "Une brève histoire... 3e partie !"
date: 2016-02-03 15:06:33 +0100
comments: true
sharing: true
categories: french préhistoire informatique dino pc unix
---

La suite
--------

Après cette [trop] longue interruption de nos émissions, voici enfin la 3ème partie de cette [toujours] brève histoire de *mon* informatique (en toute modestie hein), consacrée cette fois-ci à mon arrivée dans le monde joyeux de l'informatique libre et les UNIX libres en particulier. 

À lire après la [première partie](/2015/01/06/une-breve-histoire-de-linformatique/) et la [seconde](/2015/02/01/une-breve-histoire-dot-dot-dot-la-suite/) bien entendu :)

{% img https://assets.keltia.net/images/bsd-daemon.png "BSD Daemon" "BSD Daemon" %}

NOTE: la plupart des liens Wikipédia de cet article sont vers les versions françaises desdits articles ; je conseille néanmoins si vous le pouvez d'aller consulter les versions anglaises, beaucoup plus complètes à cet égard que les françaises, malheureusement {% fnin %}La page {% wp 386BSD "386BSD" fr %} en est d'ailleurs un terrible exemple :({% endfnin %}.
<!--more-->
BSD vs Linux
------------

Ah, le titre qui en jette, une petite *flamewar* pour se mettre en jambe ?

En fait non, surtout pas. Ce n'est pas comme ça que tout à commencé, en tout cas pour moi. Rappelons nous l'article précédent, j'arrive à la faculté de Jussieu Paris VII en 1988 après mes deux ans d'IUT d'informatique de gestion à Orsay, ayant déjà un peu tâté d'Internet et d'un système BSD (4.2BSD sur Gould).

System V R4
-----------
 
À ce moment, sur ma machine perso — un Compaq 386DX-25, je tourne un MS-DOS 3.31 (de manière à pouvoir gérer plus de 32 Mo {% fnin %}Oui oui, pas d'erreur, on parle bien de méga-octets, remettez ça dans le contexte de l'époque, il y a presque 20 ans…{% endfnin %} sur le disque dur).

Le virus UNIX a pourtant déjà pris et je me mets donc à jouer avec à la maison, principalement en regardant Xenix (oui, celui écrit et utilisé au départ par Microsoft puis distribué par SCO {% fnin %}Le SCO de cette époque n'a rien à voir avec l'actuel, attention. Il s'appelle maintenant {% wp Tarantella_(entreprise) "Tarantella" fr %} alors que c'est la société {% wp "Caldera" fr %} qui s'est renommée SCO puis SCO Group et qui « trolle » le monde du libre avec ses soi-disants brevets ou éléments de propriété intellectuelle liés à Linux).{% endfnin %} qui est un {% wp "System V" fr %} R2 (pas très évolué, pas de *sockets* par exemple donc pas de connexion Internet possible facilement, etc.) et, plus prometteur, le System V R4 de la société Microport.

Ça va me permettre d'ailleurs de m'aperçevoir que ma machine a un souci avec une puce mémoire, dès que je commence à pousser un peu la machine, c'est *panic* sur *panic* dès qu'on rempli la mémoire :( La machine sera assez rapidement remplacée par un {% wp "486DX25" fr %} puis 486DX4-100 plus tard).

Pour tout dire, l'expérience est aussi décevante qu'à la fac, System V est vraiment pas fait pour moi. En plus pas énormément d'outils de base dans ce système et installer les logiciels libres qui existent (quelques outils GNU par exemple) relève de la gageure, tant les différences entre les différents UNIX sont grandes (c'est ce qui lui a interdit le monde du *desktop* — sans parler de la pauvreté des interfaces graphiques, {% wp "X Window" fr %}, {% wp "Xaw" fr %} et {% wp "Motif" fr %} — comment dire…).

{% img https://assets.keltia.net/images/283px-5.25-Diskette.jpg "5 ¼" "5 ¼" %}

En 1990, un UNIX ça veut dire entre 30 et 50 disquettes 5" 1/4 (*floppy disk* en anglais ou disque souple) voire 77 pour un SCO UNIX System V R3.2 complet avec les *packages* optionels comme TCP/IP (4 disquettes !). Inutile de dire qu'une installation prend du temps, beaucoup de temps d'autant que ces systèmes n'étant pas fournis avec les sources, changer un paramètre du noyau ou ajouter un module dans icelui nécessite de recompiler toute la glue (genre un fichier `.c` par *driver*) et de refaire un noyau et ça prenait de longues minutes sur les machines d'antant…

DESS & IHES
-----------

1991, c'est aussi le moment où je fais mon DESS (« Logicles fondamentaux » à Jussieu Paris VII donc) et où je partage mon temps de stage entre l'Université — naissante — de Marne-la-Vallée (merci à jmm — Jean-Michel Moreno pour ce stage !) et le prestigieux {% wp Institut_des_hautes_%C3%A9tudes_scientifiques "IHES" fr %} où — grâce à mon meilleur ami qui m'y avait précédé — j'officie aussi comme ingénieur système pour les différents serveurs Sun3 et Sun4 (donc une Sparcstation 2 toute neuve) pour le mail (EARN/BITNET, pas encore le « vrai » Internet — FRIHES51 ou FRIHES61 était l'adresse du nœud)

{% img https://assets.keltia.net/images/320px-IHES_main_building.jpg "IHES" "IHES" %}

Le réseau de l'IHES comprenait le serveur principal, une Sparcstation 2 (SS2) avec 32 Mo de mémoire pour faire du partage de fichier avec {% wp NFS fr %} et serveur des terminaux X utilisés par les mathématiciens, physiciens et autres astro-physiciens du monde entier qui venaient travailler sur leurs recherches dans l'institut.

X Window était en release 4 (X11R4) à ce moment là, prenant 125 Mo pour les sources et prenant 4h à compiler sur cette machine — machine qui se ferait tailler des croupières par ne serait que le moindre *smartphone* actuel ;-) Sur les machines actuelles, ça doit prendre quelques minutes, ce sont maintenant les mastodontes façon Firefox ou pire, OpenOffice qui prennent des temps équivalents et ce, sur des processeurs 100x plus puissants que le pauvre Sparc de la SS2… 

C'est aussi ma première expérience avec l'hybride SVR4 — 4.2BSD que représente SunOS4 (bientôt appelé dans une tentative de réécriture de l'histoire par Sun Solaris 1). Sun a démarré sa transition du monde BSD vers le monde System V, probablement vu comme plus industriel et moins universitaire. Erreur que j'ai longtemps déploré même si ça avait sans doute un sens en terme de *business*… J'ai l'habitude de dire que ce faisant, Sun a échangé les anciens — mais connus — *bugs* 4.2BSD pour les anciens *bugs* SVR4 {% fnin %}SVRn comme System V Release n, une manière courante à l'époque pour nommer rapidement cette branche d'UNIX.{% endfnin %} et bien entendu les nouveaux *bugs* qu'ils ont introduits eux-même.

Il faut quand même savoir que la première version « réellement » utilisable de Solaris fut la 2.5 (vite mise à jour en 2.5.1 d'ailleurs) vu l'étendue des *bugs* et instabilités des précédentes. Sun a même réussi l'exploit de casser complètement l'API DNS (`gethostbyname(3)` et consorts) en 2.3 ou 2.4 étant passé de mémoire de la pile Lachman d'origine — la même que dans SVR3.2 — à une implémentation maison — un comble pour une API issue de BSD, la famille d'origine de Sun…
   
Ça nous donnait un joyeux mélange de comportements SVR4/BSD selon les {% wp API fr %} avec `/usr/lib` et `/usr/5lib`, un jeu de commande dupliqué entre `/usr/bin` et `/usr/5bin`, etc.

Rappel pour ceux qui voudraient comprendre les ramifications des différentes familles UNIX, le site de référence reste le [site d'Eric Levenez](http://www.levenez.com/unix/) :)

En attendant, ça permettait aux chercheurs de travailler, lire et répondre aux mails, faire du TeX/LaTeX pour leurs papiers, etc. Anecdote marrante par ailleurs sur le dernier point, les secrétaires scientifiques étaient celles qui rédigeaient et corrigeaient les papiers des chercheurs, en TeX, sur Mac et haro sur celui ou celle qui osait suggérer un Word ou un Wordperfect comme alternative !  Nul ne pouvait leur arracher leur TeXtures/Mac :)

{% img https://assets.keltia.net/images/texCode.gif "TeXtures" "TeXtures" %}

Expérience très enrichissante pour moi par ailleurs, baigner dans ce monde multi-culturel m'a beaucoup aidé pour l'anglais et m'a aussi — entre autres choses — de rentrer dans mon boulot actuel en 1996.

BSD UNIX
--------

Même si je n'ai pas l'intention de nous expliquer en détail l'histoire complète d'UNIX depuis sa conception dans les Bell Labs fin des années 60, un petit résumé historique s'impose selon moi.

UNIX est formellement né en 1969 dans les {% wp Laboratoires_Bell "Bell Labs" fr %} (appartenant au géant des télécoms {% wp American_Telephone_%26_Telegraph "AT&T" fr %}) créé notamment par {% wp Ken_Thompson "Ken Thompson" fr %} et {% wp Dennis_Ritchie "Dennis Ritchie" fr %}. Fin des années 70, l'Université de Berkeley en Californie achète une licence à Bell Labs et réalise (merci {% wp Bill_Joy "Bill Joy" fr %} {% fnin %}Également auteur de la pile {% wp Suite_des_protocoles_Internet "TCP/IP" fr %} originelle de Berkeley ainsi que de `vi(1)` et `csh(1)` — le {% wp "C-Shell" fr %}.{% endfnin %} !) les premières releases appelées BSD, pour Berkeley Software Distributions.

BSD est selon moi pendant longtemps la principale source d'innovation dans le monde UNIX, AT&T au départ n'ayant pas vraiment prévu de le vendre de manière industriel mais plus sur un point de vue recherche sur les systèmes d'exploitation. Le principal apport à ce niveau étant en 1983 d'être la plateforme de référence pour les protocoles TCP/IP que l'on connait maintenant et l'API `socket(3)` associées.

J'ai dit que c'était un résumé, voir notamment Wikipedia pour plein d'articles bien plus poussés sur le sujet au combien passionnant mais quelque peu hors sujet ici :)

Dans les années 80 nous avons donc cette famille BSD, maintenant avec les versions 4.x dont 4.2BSD (qui comprend la pile TCP/IP et le {% wp Berkeley_Fast_File_System "Fast File System" fr %} écrit par {% wp Marshall_Kirk_McKusick "Kirk McKusick" fr %}), 4.3BSD (comprenant un nouveau système de mémoire virtuelle et uen pile TCP/IP améliorée) et… 4.4BSD, la version qui va nous intéresser maintenant.

386BSD
------

Début 1991, Bill et Lynne Jolitz, vétérans du {% wp Computer_Systems_Research_Group "CSRG - EN" %} 

Linux
-----


FreeBSD
-------


Références
----------

- [Porting UNIX to the 386, Bill & Lynne Jolitz](http://porting-unix-to-the-386.jolix.com/)
- [Porting UNIX to the 386: A Practical Approach, 18-part series in Dr. Dobbs Journal, January 1991 - July 1992](https://groups.google.com/forum/#!original/comp.unix.bsd/uXJjzT4g7qI/mLMsO0hJsV4J)
- [386BSD sur WP, articles, liens](https://en.wikipedia.org/wiki/386BSD#Further_reading)

Notes
-----
{%footnotes_inline%}
