---
layout: post
title: "Une brève histoire… la suite (LONG)"
date: 2015-02-01 11:08:59 +0100
comments: true
sharing: true
categories: french préhistoire informatique dino pc unix
---

De retour
---------
Nous voici de retour dans cette brève (haha) histoire de *mon* informatique qui, ainsi que je le disait dans l'article précédent, n'a pas vocation à autre chose que vous faire partager mon parcours dans ces temps de naissance de l'informatique {% fnin %}Vous pouvez aussi dire que mes paragraphes sont trop longs, je plaide coupable.{% endfnin %}. Au sommaire, de la communication avec les {% wp Bulletin_board_system "BBS" %} et [enfin ?] de l'UNIX et du libre :)

L'accouchement n'est pas facile, je dois dire que les événements du 7 janvier m'ont vraiment marqué et revenir à cet exercice d'écriture est compliqué, je sollicite donc ton indulgence chère-cher lectrice-lecteur…
<!--more-->
Le temps des BBS (1991)
-----------------------
Nous nous étions quittés sur la fin de ma période MS-DOS en mentionnant un aspect assez peu abordé dans cette première partie, le début de ma période « C'est quoi un modem {% fnin %}Je ne parle bien évidemment pas du parti politique du même nom, même si je trouve le choix du nom assez marrant.{% endfnin %} ? », de préférence avec le monde entier…

Dans le cadre de mon activité liée au QL et à l'association QLCF (cf. là encore l'article précédent), j'ai connu des gens qui travaillaient en partie dans les télécoms et j'avais déjà récupéré un modem 1200 bauds {% fnin %}Oui, je parle bien de 1200 bauds et non, je n'ai pas eu de 300 bauds. Le moindre des modems grand public, s'il en reste, est à 56k maintenant. kbps, pas kbauds d'ailleurs, même les 56k ne sont que des 2400 bauds avec une modulation permettant plusieurs bits par baud donc.{% endfnin %} (mais qui au final ne me servira à rien car il demandait une liaison téléphonique avec 4 fils — une liaison classique n'en nécessite que 2 — et donc une ligne spécialisée).

Le QL à ce moment n'était pas très connecté en soi, même s'il possèdait un réseau local façon {% wp Nanoréseau "Nano réseau Thomson" fr %} avec des fils permettant de connecter des QL entre eux (que je n'ai jamais eu l'occasion d'utiliser d'ailleurs). Du coup, c'est vraiment dans la période MS-DOS que tout a commencé.

Les modems restaient quelque chose d'assez cher et le prix des connexions téléphoniques n'aidait pas (paiement au temps de connexion, numéros payants même si le fait que les communications locales soient restées longtemps gratuites puis limitées à 20 mn a permis de limiter les factures) du coup il a fallu quelques temps avant que je puisse en avoir un.

Interlude Minitel
-----------------
En France, nous avons eu l'immense chance (haha) d'avoir ce superbe joyau qu'était le {% wp Minitel "Minitel" fr %} qui, s'il lui faut reconnaitre d'avoir poussé plein de gens dans le monde merveilleux de la communication informatique, n'en restait quand même un outil doté de caractéristiques techniques assez pourries (ah la vitesse royale de 1200 bauds en descente et de 75 (!) en montée — le standard utilisé n'ayant été choisi que pour créer un lien de consommateur vers fournisseur, le modèle français de la communication {% fnin %}en opposition avec la notion infinimment plus équitable d'Internet où tout le monde est la fois producteur et consommateur d'information.{% endfnin %}).

{% img http://assets.keltia.net/blog/320px_Minitel_terminal.jpg "Minitel" "Minitel" %}

J'utilisais d'ailleurs un Minitel 1b (celui qui permettait d'échanger les vitesses en descente/montée — 1200/75 donc — en cours de communication) pour me connecter à la faculté de Jussieu sur le compte de ma prof d'archi (Edwige P. sois en encore remercié, tu ne sais sans doute pas ce que tu as déclenché) {% fnin %}Oui, je l'admets tout à fait, c'est Mal©® — on ne doit jamais partager un mot de passe ou un compte sur une machine. Je n'ai rien cassé par contre.{% endfnin %}

Fin de l'interlude
------------------

En 1991, une société américaine lance un des premiers modems V32bis abordables, le {% wp SupraFAXModem_14400 "SupraFAXModem (EN)" %}. L'appellation V32bis désigne la norme ITU pour les modems à 14400 bps ce qui représente une vitesse brute (hors protocole donc) d'environ 1.8 Ko/s.

Je m'en suis acheté un (ne me demandez pas le prix; probablement aux alentours de de 400 FF — 60 € vu les prix US) et j'ai pu me lancer enfin dans l'aventure des {% wp Bulletin_board_system "BBS" fr %}, ces serveurs, généralement sous Windows (avec le logiciel PC-Board notamment — sur ModulaBBS, Suptel ou encore Li'LL BBS) ou QNX, OS temps-réel avec micro-noyau ([QBBS](http://www.qbbs.fr/)).

{% img http://assets.keltia.net/blog/320px-SupraFAXmodem_144_LC.jpg "SupraFaxModem 14400" "SupraFaxModem 14400" %}

On y trouvait des forums de discussion (le principal intérêt de ces serveurs), parfois des espaces de téléchargement de logiciels _freeware_ (gratuits donc) et _shareware_ (pour lesquels il était demandé de payer après une période de test) et parfois plus{% fnin %}On y trouvait aussi à quelques endroits des logiciels commerciaux, avec des noms comme Warez ou SLC, étant dans l'illégalité…{% endfnin %}. Ce mo

Suite à des discussions avec certains sur ModulaBBS que j'ai pu participer à un « petit midi », appellation donnée à un repas (précédé par un apéro bien évidemment) avec le même cercle d'habitués comprenant cette fois-ci René Cougnenc, Serge Delbono, Sam Cabannes et Christian « Bubulle » Perrier. C'est grâce à ce déjeuner que j'ai pu accéder à Li'LL BBS d'ailleurs, tenu par Attila Altan. Li'LL BBS, tournant sous {% wp PCBoard "PCBoard" fr %}, était connecté à plusieurs réseaux différents (avec ModulaBBS notamment) y compris {% wp FidoNet "FidoNet" fr %}{% fnin %}Li'LLBBS était numéroté `2:320/7` et j'ai fini par être un des rares « points » avec `2:320/7.2`.{% endfnin %}. Ces petits midi furent l'occasion de refaire le monde maintes fois et aussi, fin 1991, de parler d'un petit logiciel écrit par un finlandais inconnu, un certain {% wp Linus_Torvalds "Linus Torvalds" fr %}. Li'LL BBS est resté longtemps mon BBS de prédilection et même si le BBS n'existe plus, il en subsiste une liste de discussion et les amis que j'y ai toujours comme Attila, Gordon et les autres :)

J'ai fait tourner le mien d'ailleurs, un petit nœud assez discret, me servant plus de réceptacle pour les copains et me permettant de récupérer mes messages Fido que je lisais _via_ [Golded](http://golded.org/), un des meilleurs programmes du genre.

René
----
Que dire sur {% wp René_Cougnenc "René Cougnenc" fr %} qui n'ait pas été dit à maintes reprises ? Que ce type, franchouillard dans le meilleur sens possible, buveur, fumeur, blagueur et altruiste au possible, ancien ingénieur du son — qui finit par être désespéré de l'évolution de son métier et de son côté précaire, converti à l'informatique et équipé par un ordinateur offert par ses copains de Li'LL BBS, auteur de BBTH {% fnin %}Logiciel pour accéder aux services QBBS et Minitel.{% endfnin %} et d'un logiciel d'accès à distance {% fnin %}Lequel lui permettra de récupérer les premières versions de Linux — 0.17 et 0.18 en 1991 grâce à C. Perrier et de les diffuser sur son serveur `renux`{% endfnin %}, était adorable, toujours près à discuter de ses passions avec tout le monde.

Il deviendra un pilier de la partie francophone de Usenet, notamment dans le groupe `fr.comp.os.linux` et avant dans les groupes qui existaient sur les BBS. Nous discutions souvent des différences entre Linux et à l'époque {% wp 386BSD "386BSD" fr %}, lui étant heureux de voir le développement du premier et s'amusant de ma volonté d'attendre le second (voir plus loin). La manière dont évoluait le monde en 1995-96 le désespérait déjà (que ne dirait-il maintenant à voir nos libertés rognées ainsi !) et il a choisi de le quitter en juillet 1996.

René était mon pote, un grand copain qui me manque toujours…

{% img http://assets.keltia.net/blog/rene_cougnenc.jpg "René Cougnenc" "René Cougnenc" %}

Les BBS, suite
--------------
Ce fut aussi l'occasion de rentrer certains autres personnages qui devinrent célèbres sur {% wp Usenet "USENET" fr %} quelques années après comme le surnommé {% wp Jean-Bernard_Condat "Concombre" fr %}, qui, nonobstant sa page WP, n'a vraiment eu de « hacker » que le nom, s'étant ridiculisé à essayer de pirater le fax de François Vigneron, alors modérateur d'un groupe de discussion sur ModulaBBS. Inutile de dire que lors de son arrivée quelques années plus tard sur Usenet {% fnin %}Je ne pourrai pas vous donner des références sur ce point, Google ayant tellement détruit l'interface de Google Groups après le rachat de Dejanews qu'il est maintenant impossible de faire des recherches correctement dans les archives de Usenet :({% endfnin %}, sa réputation était déjà faite… Je ne donnerai a priori pas plus de détail, n'ayant pas envie de me prendre un procès du personnage :)

{% wp FidoNet "FidoNet" fr %} était, d'une certaine manière, calqué sur le réseau {% wp Unix_to_Unix_Copy_Protocol "UUCP" fr %} mais avec une architecture fortement hiérarchisée pour répartir au mieux et surtout au plus proche les coûts téléphoniques, organisé en pays et en régions. Des passerelles existent toujours d'ailleurs entre Usenet et FidoNet.

Le monde des BBS s'est progressivement réduit à la fin des années 1990 suite à l'essor en parallèle de Usenet et des forums web après (lesquels ont globalement bouffé Usenet aussi d'ailleurs, pour notre malheur).

L'aventure UNIX et du libre (1988 et au-delà)
---------------------------------------------
Retour en arrière sur UNIX…

Avant de passer à un UNIX libre en 1991, suite à mon entrée en licence à Jussieu Paris VII en 1988, après mon DUT à Orsay (voir l'article précédent), je tombe complètement dans l'univers UNIX au travers des machines mises à disposition des étudiants. C'est là que je suis confronté pour la première fois à un système {% wp Berkeley_Software_Distribution "BSD" fr %}, la machine principale étant un Gould Encore tournant 4.2BSD, royalement dotée de 8 Mo de mémoire pour la quarantaine de terminaux, une partie de DEC VT100 et l'autre de Falco VT220, les deuxièmes étant reliés au Gould à 19200 bps, les premiers n'étant qu'à 9600.

{% img http://assets.keltia.net/blog/falco-vt220.png "Falco VT220" "Falco VT220" %}

La différence n'est pas si importante que ça, jusqu'au moment où, ayant fini les divers TP et autres exercices, on décide de jouer un peu et sur des jeux multi-joueurs comme `Banzai` (une modification du jeu classique `Hack` de l'époque — un espace en forme de labyrinthe dans lequel les joueurs évoluent et se tirent dessus, renaissant de manière aléatoire  dans lesquels la rapidité de réaction sur un terminal donné peut faire la différence entre gagner et perdre :) C'est aussi à cet endroit que j'ai pu jouer à ces grands classiques que sont {% wp Rogue_(jeu_vidéo) "Rogue" fr %}, {% wp Larn "larn" fr %} et autres {% wp NetHack "Nethack" fr %} {% fnin %}Ces jeux existent toujours et sont encore disponibles sur les UNIX actuels comme FreeBSD et il m'arrive encore d'y jouer — un jeu ne nécessite pas forcément la dernière carte vidéo-de-la-mort-qui-tue et la fibre :){% endfnin %}.

{% img http://assets.keltia.net/blog/larn.png "larn" "larn" %}

Les autres machines disponibles disposaient quant à elles d'une version de System V, l'autre grande famille UNIX (et l'origine en fait, BSD n'étant que les évolutions de l'Université de Berkeley, CA sur la Version 7 {% fnin %}Voir à ce propos, le [site d'Eric Levenez](http://www.levenez.com/unix/) qui raconte d'une machine graphique l'évolution complète des familles UNIX au travers des âges…{% endfnin %}. Dès le départ, j'ai pu voir que l'UNIX qu'elles utilisaient était moins pratique et moins puissant que le BSD d'à côté, c'est à ce moment que j'ai décidé de suivre cette voie plutôt que l'autre :)

J'ai aussi commencé à utiliser le {% wp Interface_système "shell" fr %} qui restera le mien pendant quelques années, {% wp Tcsh "tcsh" fr %}, d'abord livré comme [patch](https://fr.wiktionary.org/wiki/patch) sur les sources de {% wp C_shell "csh" fr %} puis comme produit à part entière. Ce n'est qu'il y a environ 15 ans que j'ai basculé sur {% wp Z_Shell "Zsh" fr %}.

Rappelons nous, nous sommes en 1988 et la fac est reliée à un petit bout d'Internet par l'intermédiaire d'une liaison modem à 9600 bps. Là encore, le chiffre est correct, l'ensemble de l'université Paris VII (et peut-être Paris VI aussi) avec des dizaines de milliers d'étudiants partageait une liaison 6 fois moins rapide que le plus siple des modems actuels à 56 kbps, de même que tous les étudiants de licence et maitrise informatique partageaient une machine avec 8 Mo de mémoire vive :)

Ça donne une perspective légèrement différente sur les machines actuelles et leurs possibilités (tout comme les 1 Ko du ZX81 de l'article précédent), non ?

J'ai eu aussi l'honneur d'avoir comme professeur de système et réseau (et théorie de la programmation en DESS) {% wp Jean-Marie_Rifflet "Jean-Marie Rifflet" fr %}, également auteur de livres connus sur UNIX et le réseau {% fnin %}Notamment « La programmation sous UNIX » notre livre de chevet en licence et « La communication sous UNIX », reflet du cours qu'il nous donna en maîtrise.{% endfnin %}.

La faculté était reliée donc à Internet _via_ cette liaison mais disposait aussi d'un accès {% wp European_Academic_Research_Network "EARN/BITNET" fr %} par l'intermédiaire du CICRP, un labo de mathématiques juste à côté. Il y avait un système {% wp Multics "Multics" fr %}, ancètre d'UNIX et sur celui-ci, nous, étudiants et professeurs, utilisons ce système pour envoyer des courriers électroniques. Ce qui incidemment permettait de récupérer des fichiers venant de machines distantes avec un système appelé BitFTP : vous donniez la liste des commandes du protocole {% wp File_Transfer_Protocol "FTP" fr %} et receviez en retour de mail, les différents morceaux du logiciel, à recoller vous-mêmes. D'ailleurs une fois, l'administrateur système de Paris VII, Jean-Michel Moreno {% fnin %}Lui-même auteur d'un livre sur l'administration système UNIX. Pour l'anecdote, la première citation du livre était de Lénine :){% endfnin %} entrer dans une colère monstre car il avait perdu l'un des 140 et quelques morceaux de la version de gcc qu'il venait de télécharger…

L'accès à Internet restait assez compliqué à utiliser, le {% wp Domain_Name_System "DNS" fr %} n'étant même pas configuré sur le Gould, nous obligeant à récupérer périodiquement le fameux fichier `HOSTS.TXT` lequel contenait la liste exhaustive des sites Internet afin d'y piocher les adresses IP de quelques serveurs sous intéressant, généralement pour y récupérer les _freewares_ et _sharewares_ précédemment cité dans le chapitre BBS :)

À ce moment là, nous finissions par connaitre par cœur les IP de `prep.ai.mit.edu` (berceau de GNU déjà) et autres `simtel20.wsmr.army.mil` (White Sands Missile Range qui comme le nom l'indique, est une base de lancement de missiles américaine — si si je vous assure, ils hébergeaient des dizaines de mégaoctets de logiciels MS-DOS, Amiga et autres :)) {% fnin %}Dans le genre, mais que fait ma mémoire pour retenir ces choses-là, je me souvient encore du nom de l'administrateur du site BITNET en Turquie qui hébergeait un nœud BitFTP, Turgut Kalfaoğlu.{% endfnin %}.

L'autre aspect de ce système Multics était d'avoir des forums de discussions sur divers sujets (pas encore de Usenet à cette époque pour la fac). Il se trouve que j'essayais toujours de développer mes programmes de cryptographie et cherhant un algorithme pour générer une liste de nombres aléatoires, en fait un mélange d'une suite croissante de nombres genre de 000 à 999. J'ai donc posté ma question sur un de ces forums sans trop y croire en fait à ce moment là et j'ai reçu, à ma grande de surprise, plusieurs réponses de parfaits inconnus…

Ça peut paraitre banal maintenant, où Twitter ou [Stack Overflow](http://stackoverflow.com/) sont couramment utilisés pour des questions de ce genre mais en 1988, ça m'a fait un choc. Et ça a changé ma vision des choses d'une telle manière que je me suis jeté dans Usenet quand j'y ai eu accès et n'ai eu de cesse qu'à partager mes quelques connaissances (informatique ou autres).

Usenet (1990)
-------------

Références
----------
- [La programmation sous UNIX, by Jean-Marie Rifflet, Ed. Delmas et Cie](http://amzn.to/1zLq06W)
- [La communication sous UNIX, by Jean-Marie Rifflet, Ed. Delmas et Cie](http://amzn.to/1DuR3kt)
- [UNIX Administration, by Jean-Michel Moreno, Ed. Delmas et Cie](http://amzn.to/1DuRwmF)

Notes
-----
{%footnotes_inline%}
