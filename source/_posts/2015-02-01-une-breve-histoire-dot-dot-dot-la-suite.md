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
Nous voici de retour dans cette brève (haha) histoire de *mon* informatique qui, ainsi que je le disait dans l'[article précédent](/2015/01/06/une-breve-histoire-de-linformatique/), n'a pas vocation à autre chose que vous faire partager mon parcours dans ces temps de naissance de l'informatique {% fnin %}Vous pouvez aussi dire que mes paragraphes sont trop longs, je plaide coupable.{% endfnin %}. Au sommaire, de la communication avec les {% wp Bulletin_board_system "BBS" %} et [enfin ?] de l'UNIX et du libre :)

L'accouchement n'est pas facile, je dois dire que les événements du 7 janvier m'ont vraiment marqué et revenir à cet exercice d'écriture est compliqué, je sollicite donc ton indulgence chère-cher lectrice-lecteur…
<!--more-->
Le temps des BBS (1991)
-----------------------
Nous nous étions quittés sur la fin de ma période MS-DOS en mentionnant un aspect assez peu abordé dans cette première partie, le début de ma période « _C'est quoi un modem_ {% fnin %}Je ne parle bien évidemment pas du parti politique du même nom, même si je trouve le choix du nom assez marrant.{% endfnin %} ? », pour communiquer de préférence avec le monde entier…

Dans le cadre de mon activité liée au QL et à l'association QLCF (cf. là encore l'article précédent), j'ai connu des gens qui travaillaient en partie dans les télécoms et j'avais déjà récupéré un modem 1200 bauds {% fnin %}Oui, je parle bien de 1200 bauds et non, je n'ai pas eu de 300 bauds. Le moindre des modems grand public, s'il en reste, est à 56k maintenant. kbps, pas kbauds d'ailleurs, même les 56k ne sont que des 2400 bauds avec une modulation permettant plusieurs bits par baud donc.{% endfnin %} (mais qui au final ne me servira à rien car il demandait une liaison téléphonique avec 4 fils — une liaison classique n'en nécessite que 2 — et donc une ligne spécialisée).

Le QL à ce moment n'était pas très connecté en soi, même s'il possèdait un réseau local façon {% wp Nanoréseau "Nano réseau Thomson" fr %} avec des fils permettant de connecter des QL entre eux (que je n'ai jamais eu l'occasion d'utiliser d'ailleurs). Du coup, c'est vraiment dans la période MS-DOS que tout a commencé.

Les modems restaient quelque chose d'assez cher et le prix des connexions téléphoniques n'aidait pas (paiement au temps de connexion, numéros payants même si le fait que les communications locales soient restées longtemps gratuites puis limitées à 20 mn a permis de limiter les factures) du coup il a fallu quelque temps avant que je puisse en avoir un.

Interlude Minitel
-----------------
En France, nous avons eu l'immense chance (haha) d'avoir ce superbe joyau qu'était le {% wp Minitel "Minitel" fr %} qui, s'il lui faut reconnaître d'avoir poussé plein de gens dans le monde merveilleux de la communication informatique, n'en restait quand même un outil doté de caractéristiques techniques assez pourries (à la vitesse royale de 1200 bauds en descente et de 75 (!) en montée — le standard utilisé n'ayant été choisi que pour créer un lien de consommateur vers fournisseur, le modèle français de la communication {% fnin %}en opposition avec la notion infiniment plus équitable d'Internet où tout le monde est la fois producteur et consommateur d'information.{% endfnin %}).

{% img https://assets.keltia.net/blog/320px_Minitel_terminal.jpg "Minitel" "Minitel" %}

J'utilisais d'ailleurs un Minitel 1b (celui qui permettait d'échanger les vitesses en descente/montée — 1200/75 donc — en cours de communication) pour me connecter à la faculté de Jussieu sur le compte de ma professeur d'architecture système (Edwige P. sois en encore remerciée, tu ne sais sans doute pas ce que tu as déclenché) {% fnin %}Oui, je l'admets tout à fait, c'est Mal©® — on ne doit jamais partager un mot de passe ou un compte sur une machine. Je n'ai rien cassé par contre.{% endfnin %}

Fin de l'interlude
------------------

En 1991, une société américaine lance un des premiers modems V32bis abordables, le {% wp SupraFAXModem_14400 "SupraFAXModem (EN)" %}. L'appellation V32bis désigne la norme ITU pour les modems à 14400 bps ce qui représente une vitesse brute (hors protocole donc) d'environ 1.8 Ko/s.

Je m'en suis acheté un (ne me demandez pas le prix; probablement aux alentours de de 400 FF — 60 € vu les prix US) et j'ai pu me lancer enfin dans l'aventure des {% wp Bulletin_board_system "BBS" fr %}, ces serveurs, généralement sous Windows (avec le logiciel PC-Board notamment — sur ModulaBBS, Suptel ou encore Li'LL BBS) ou QNX, OS temps-réel avec micro-noyau ([QBBS](http://www.qbbs.fr/)).

{% img https://assets.keltia.net/blog/320px-SupraFAXmodem_144_LC.jpg "SupraFaxModem 14400" "SupraFaxModem 14400" %}

On y trouvait des forums de discussion (le principal intérêt de ces serveurs), parfois des espaces de téléchargement de logiciels _freeware_ (gratuits donc) et _shareware_ (pour lesquels il était demandé de payer après une période de test) et parfois plus{% fnin %}On y trouvait aussi à quelques endroits des logiciels commerciaux, avec des noms comme Warez ou SLC, de manière plutôt discrète et réservés aux habitués, ces espaces étant clairement dans l'illégalité…{% endfnin %}.

C'est suite à des discussions avec certains sur ModulaBBS que j'ai pu participer à un « petit midi », appellation donnée à un repas (précédé par un apéro bien évidemment) avec le même cercle d'habitués comprenant cette fois-ci René Cougnenc, Serge Delbono, Sam Cabannes et Christian « Bubulle » Perrier. C'est grâce à ce déjeuner que j'ai pu accéder à Li'LL BBS d'ailleurs, tenu par Attila Altan. Li'LL BBS, tournant sous {% wp PCBoard "PCBoard" fr %}, était connecté à plusieurs réseaux différents (avec ModulaBBS notamment) y compris {% wp FidoNet "FidoNet" fr %} {% fnin %}Li'LLBBS était numéroté `2:320/7` et j'ai été un des rares « points » avec `2:320/7.2`.{% endfnin %}. Ces petits midi furent l'occasion de refaire le monde maintes fois et aussi, fin 1991, de parler d'un petit logiciel écrit par un finlandais inconnu, un certain {% wp Linus_Torvalds "Linus Torvalds" fr %}. Li'LL BBS est resté longtemps mon BBS de prédilection et même s'il n'existe plus en tant que tel, il en subsiste une liste de discussion et les amis que j'y ai toujours comme Attila, Gordon et les autres :)

Une anecdote assez connue concerne ce même Gordon {% fnin %}De son nom complet, Gordon E. Peterson II d'ailleurs ;-){% endfnin %} et quelqu'un d'assez connu déjà… un certain Richard Stallman : lors d'une conférence à l'école d'informatique EPITA {% fnin %}Pas encore célèbre pour avoir piraté la moitié de RENATER en 1994, ce qui leur avait valu d'être mis en liste noire chez les clients d'[HSC](/2014/12/12/la-fin-dune-epoque-dot-dot-dot/) cf. [ce tweet](https://twitter.com/Keltounet/status/287314804329291778).{% endfnin %} sur le logiciel libre et je suppose le projet GNU — je n'étais pas à ladite conférence — l'auditoire a eu l'occasion d'assister à ce qui a été, appelons un chat un chat, une engueulade en français entre nos deux Américains sur le sujet _free software_ vs _shareware_, les deux points de vue ne pouvant manifestement pas s'accorder {% fnin %}Si quelqu'un a assisté à la conférence elle-même, ça m'intéresse, Gordon à qui j'ai posé la question, ne se souvient plus exactement de la date…{% endfnin %} :)

J'ai fait tourner le mien d'ailleurs, un petit nœud assez discret, me servant plus de réceptacle pour les copains et me permettant de récupérer mes messages Fido que je lisais _via_ [Golded](http://golded.org/), un des meilleurs programmes du genre. J'avais même pris une ligne téléphonique dédiée à la maison pour ça :)

René
----
Que dire sur {% wp René_Cougnenc "René Cougnenc" fr %} qui n'ait pas été dit à maintes reprises ? Que ce type, franchouillard dans le meilleur sens possible, buveur, fumeur, blagueur et altruiste au possible, ancien ingénieur du son — qui finit par être désespéré de l'évolution de son métier et de son côté précaire, converti à l'informatique et équipé par un ordinateur offert par ses copains de Li'LL BBS, auteur de BBTH {% fnin %}Logiciel pour accéder aux services QBBS et Minitel.{% endfnin %} et d'un logiciel d'accès à distance {% fnin %}Lequel lui permettra de récupérer les premières versions de Linux — 0.17 et 0.18 en 1991 grâce à C. Perrier et de les diffuser sur son serveur `renux`{% endfnin %}, était adorable, toujours près à discuter de ses passions avec tout le monde.

Il deviendra un pilier de la partie francophone de Usenet, notamment dans le groupe `fr.comp.os.linux` et avant dans les groupes qui existaient sur les BBS. Nous discutions souvent des différences entre Linux et à l'époque {% wp 386BSD "386BSD" fr %}, lui étant heureux de voir le développement du premier et s'amusant de ma volonté d'attendre le second (voir plus loin). La manière dont évoluait le monde en 1995-96 le désespérait déjà (que ne dirait-il maintenant à voir nos libertés rognées ainsi !) et il a choisi de le quitter en [juillet 1996](https://groups.google.com/d/topic/fr.comp.os.linux/eAQzrhEXejI/discussion).

René était mon pote, un grand copain qui me manque toujours…

{% img https://assets.keltia.net/blog/rene_cougnenc.jpg "René Cougnenc" "René Cougnenc" %}

Les BBS, suite
--------------
Ce fut aussi l'occasion de rencontrer certains autres personnages qui devinrent célèbres sur {% wp Usenet "USENET" fr %} quelques années après comme le surnommé {% wp Jean-Bernard_Condat "Concombre" fr %}, qui, nonobstant sa page WP, n'a vraiment eu de « hacker » que le nom, s'étant ridiculisé à essayer de pirater le fax de François Vigneron, alors modérateur d'un groupe de discussion sur ModulaBBS. Inutile de dire que lors de son arrivée quelques années plus tard sur Usenet {% fnin %}Je ne pourrai pas vous donner des références sur ce point, Google ayant tellement détruit l'interface de Google Groups après le rachat de Dejanews qu'il est maintenant impossible de faire des recherches correctement dans les archives de Usenet :({% endfnin %}, sa réputation était déjà faite… Je ne donnerai a priori pas plus de détail, n'ayant pas envie de me prendre un procès du personnage :)

{% wp FidoNet "FidoNet" fr %} était, d'une certaine manière, calqué sur le réseau {% wp Unix_to_Unix_Copy_Protocol "UUCP" fr %} mais avec une architecture fortement hiérarchisée pour répartir au mieux et surtout au plus proche les coûts téléphoniques, organisé en pays et en régions. Des passerelles existent toujours d'ailleurs entre Usenet et FidoNet.

Le monde des BBS s'est progressivement réduit à la fin des années 1990 suite à l'essor en parallèle de Usenet et des forums web après, lesquels ont globalement bouffé Usenet aussi d'ailleurs pour notre malheur.

L'aventure UNIX (1988 et au-delà)
---------------------------------------------
Retour en arrière sur UNIX…

Avant de passer à un UNIX libre en 1991, suite à mon entrée en licence à Jussieu Paris VII en 1988, après mon DUT à Orsay (voir l'article précédent), je tombe complètement dans l'univers UNIX au travers des machines mises à disposition des étudiants. C'est là que je suis confronté pour la première fois à un système {% wp Berkeley_Software_Distribution "BSD" fr %}, la machine principale étant un Gould Encore fonctionnant avec 4.2BSD, royalement dotée de 8 Mo de mémoire pour la quarantaine de terminaux, une partie de DEC VT100 et l'autre de Falco VT220, les deuxièmes étant reliés au Gould à 19 200 bps, les premiers ne l'étant qu'à 9 600.

{% img https://assets.keltia.net/blog/falco-vt220.png "Falco VT220" "Falco VT220" %}

La différence n'est pas si importante que ça, jusqu'au moment où, ayant fini les divers TP et autres exercices, on décide de jouer un peu. Sur des jeux multi-joueurs comme `Banzai` (une modification du jeu classique `Hack` de l'époque — un espace en forme de labyrinthe dans lequel les joueurs évoluent et se tirent dessus, renaissant de manière aléatoire  dans lesquels la rapidité de réaction sur un terminal donné peut faire la différence entre gagner et perdre :)).

 C'est aussi à cet endroit que j'ai pu jouer à ces grands classiques que sont {% wp Rogue_(jeu_vidéo) "Rogue" fr %}, {% wp Larn "larn" fr %} et autres {% wp NetHack "Nethack" fr %} {% fnin %}Ces jeux existent toujours et sont encore disponibles sur les UNIX actuels comme FreeBSD et il m'arrive encore d'y jouer — un jeu ne nécessite pas forcément la dernière carte vidéo-de-la-mort-qui-tue et la fibre :){% endfnin %}.

{% img https://assets.keltia.net/blog/larn.png "larn" "larn" %}

Les autres machines disponibles disposaient quant à elles d'une version de System V, l'autre grande famille UNIX (et l'origine en fait, BSD n'étant que les évolutions de l'Université de Berkeley, CA sur la Version 7 {% fnin %}Voir à ce propos, le [site d'Eric Levenez](http://www.levenez.com/unix/) qui raconte d'une manière graphique l'évolution complète des familles UNIX au travers des âges…{% endfnin %}. Dès le départ, j'ai pu voir que l'UNIX qu'elles utilisaient était moins pratique et moins puissant que le BSD d'à côté, c'est à ce moment que j'ai décidé de suivre cette voie plutôt que l'autre :)

J'ai aussi commencé à utiliser le {% wp Interface_système "shell" fr %} qui restera le mien pendant quelques années, {% wp Tcsh "tcsh" fr %}, d'abord livré comme [patch](https://fr.wiktionary.org/wiki/patch) sur les sources de {% wp C_shell "csh" fr %} puis comme produit à part entière. Ce n'est qu'il y a environ 15 ans que j'ai basculé sur {% wp Z_Shell "Zsh" fr %}.

Rappelons nous, nous sommes en 1988 et la faculté est reliée à un petit bout d'Internet par l'intermédiaire d'une liaison modem à 9 600 bps (_via_ l'{% wp Institut_national_de_recherche_en_informatique_et_en_automatique "INRIA" fr %}, ell-même reliée à Amsterdam). Là encore, le chiffre est correct, l'ensemble de l'université Paris VII (et peut-être Paris VI aussi) avec des dizaines de milliers d'étudiants partageait une liaison 6 fois moins rapide que le plus simple des modems actuels à 56 kbps de même que tous les étudiants de licence et maitrise informatique partageaient une machine avec 8 Mo de mémoire vive :)

Ça donne une perspective légèrement différente sur les machines actuelles et leurs possibilités (tout comme les 1 Ko du ZX81 de l'article précédent), non ?

J'ai eu aussi l'honneur d'avoir comme professeur de système et réseau (et théorie de la programmation en DESS) {% wp Jean-Marie_Rifflet "Jean-Marie Rifflet" fr %}, également auteur de livres connus sur UNIX et le réseau {% fnin %}Notamment « La programmation sous UNIX » notre livre de chevet en licence et « La communication sous UNIX », reflet du cours qu'il nous donna en maîtrise.{% endfnin %}.

La faculté était reliée donc à Internet _via_ cette liaison mais disposait aussi d'un accès {% wp European_Academic_Research_Network "EARN/BITNET" fr %} par l'intermédiaire du CICRP, un labo de mathématiques juste à côté. Il y avait un système {% wp Multics "Multics" fr %}, ancètre d'UNIX et sur celui-ci, nous, étudiants et professeurs, utilisions ce système pour envoyer des courriers électroniques. Ce qui incidemment permettait de récupérer des fichiers venant de machines distantes avec un système appelé BitFTP : vous donniez la liste des commandes du protocole {% wp File_Transfer_Protocol "FTP" fr %} et receviez en retour de mail, les différents morceaux du logiciel, à recoller soi-même. D'ailleurs une fois, j'ai vu l'administrateur système de Paris VII, Jean-Michel Moreno {% fnin %}Lui-même auteur d'un livre sur l'administration système UNIX. Pour l'anecdote, la première citation du livre était de Lénine :){% endfnin %} entrer dans une colère monstre car il avait perdu l'un des 140 et quelques morceaux de la version de gcc qu'il venait de télécharger…

L'accès à Internet restait assez compliqué à utiliser, le {% wp Domain_Name_System "DNS" fr %} n'étant même pas configuré sur le Gould, nous obligeant à récupérer périodiquement le fameux fichier `HOSTS.TXT` lequel contenait la liste exhaustive des sites Internet afin d'y piocher les adresses IP de quelques serveurs sous intéressant, généralement pour y récupérer les _freewares_ et _sharewares_ précédemment cité dans le chapitre BBS :)

À ce moment là, nous finissions par connaitre par cœur les IP de `prep.ai.mit.edu` (berceau de GNU déjà), `wuarchive.wustl.edu` et autres `simtel20.wsmr.army.mil` (White Sands Missile Range qui comme le nom l'indique, est une base de lancement de missiles américaine — si si je vous assure, ils hébergeaient des dizaines de mégaoctets de logiciels MS-DOS, Amiga et autres :)) {% fnin %}Dans le genre, mais que fait ma mémoire pour retenir ces choses-là, je me souviens encore du nom de l'administrateur du site BITNET en Turquie qui hébergeait un nœud BitFTP, Turgut Kalfaoğlu.{% endfnin %}. Simtel20 tournait sous {% wp TOPS-20 "TOPS-20" %} sur une DEC.

L'autre aspect de ce système Multics était d'avoir des forums de discussions sur divers sujets (pas encore de Usenet à cette époque pour la fac). Il se trouve que j'essayais toujours de développer mes programmes de cryptographie et cherchant un algorithme pour générer une liste de nombres aléatoires, en fait un mélange d'une suite croissante de nombres genre de 000 à 999. J'ai donc publié ma question sur un de ces forums sans trop y croire en fait à ce moment là et j'ai reçu, à ma grande de surprise, plusieurs réponses de parfaits inconnus…

Ça peut paraitre banal maintenant, où Twitter ou [Stack Overflow](http://stackoverflow.com/) sont couramment utilisés pour des questions de ce genre mais en 1988, ça m'a fait un choc. Et ça a changé ma vision des choses d'une telle manière que je me suis jeté dans Usenet quand j'y ai eu accès et n'ai eu de cesse de partager mes quelques connaissances (informatique ou autres).

Usenet (1990-20??)
-------------
{% wp Usenet "Usenet" fr %} est finalement arrivé à Jussieu aux alentours de 1990. Usenet n'était pas alors un serveur de logiciels piratés ou d'images « pieuses » comme beaucoup le croient maintenant, c'était principalement un ensemble de serveurs connectés entre eux (les nœuds) et servant des utilisateurs soit directement soit _via_ des serveurs « feuilles {% fnin %}La différence entre les deux est qu'une feuille n'a qu'un seul fournisseur alors qu'un nœud au moins deux.{% endfnin %} ».

Je ne vais pas détailler l'histoire et le fonctionnement de Usenet ici, je vous renvoie à la conférence que j'ai donnée à [Pas Sage en Seine](http://www.passageenseine.org/Passage/pses-2013) en 2013, la présentation PDF est [ici](https://assets.keltia.net/pses2013.pdf) et la vidéo [ici](http://lacantine.ubicast.eu/channels/#pas-sage-en-seine-2013).

En résumé, j'ai participé à Usenet assez tard (Usenet est né en 1979, créé par des administrateurs dans des universités américains par, entre autres, [Steve Bellovin](https://www.cs.columbia.edu/~smb/blog/control/) et n'ai pas vu les premiers événements marquants (comme la grande réorganisation de `mod` et `net` vers le système actuel de Big8) mais j'ai pu participer à plein de groupes, vu l'essor des UNIX libres (et les _flame wars_ correspondantes en 1993 par exemple) et la montée en puissance de la hiérarchie francophone `fr.*`.

Je crois qu'à part l'épisode des anonymes sur `fr.*`, l'événement le plus marquant fut le vote pour le groupe `rec.music.white-power`.

Le premier raconte une période, fin 1998, durant laquelle, suite à la protestation de divers intervenants à propos d'articles anonymes ne faisant que de la pub pour un service de logiciels piratés — la publicité sous toute ses formes est interdite dans les groupes généraux — les courageux auteurs avaient publié des articles nous accusant d'être des pédophiles (le tout en faisant une usurpation d'identité…),

Le deuxième épisode ne concerne pas `fr.*`mais Usenet en entier : le groupe `rec.music.white-power` a suscité énormément de discussion (intitulé et futur contenu clairement racistes) et le vote fut épique, celui-ci se terminant avec plus de 40 000 votes avec près de 8 000 annulés pour cause de bourrage d'urne, le groupe n'a pas été créé vu le nombre de votes NON {% fnin %}Ce genre de choses rend plutôt foi en l'Humanité, le résultat final fut 592 YES/33033 NO.{% endfnin %}… Aucune autre proposition n'a rivalisé avec celle-ci depuis.

Je suis d'ailleurs devenu le responsable technique de ces groupes `fr.*`en 1998 suite à un conflit avec le « Control » de l'époque. Jusqu'à présent, même si le boulot que ça représente est minime (quelques groupes créés en 2014 seulement), personne n'a vraiment essayé de reprendre le flambeau :)

On y avait retrouvé en 1994 le cher concombre dans un des épisodes les plus célèbres, celui du vrai-faux article anonyme. Impossible de retrouver l'enfilade mais grâce à François-Yves, voici une discussion en parlant :) -- [Enfilade](https://groups.google.com/forum/?hl=fr#!search/concombre$20anon.penet/fr.network.internet/s3ig5jvgkHw/KKy6WXFb7XgJ).

À mes débuts, les seuls lecteurs de News étaient en mode texte sous UNIX (les terminaux VT220, vous vous souvenez ?) et portaient des noms comme `rn` (évolution de `readnews`par Larry Wall — également auteur de {% wp Perl_(langage) "Perl" fr %}) qui fut suivi de `trn` {% fnin %}Je l'utilise encore d'ailleurs, pour le peu de Usenet qu'il m'arrive encore de faire :){% endfnin %} (pour _threaded_ rn, affichant d'une manière assez géniale les fils de discussion, manière encore inégalée pour moi), `slrn`ou encore `tin`. Il existait aussi quelques lecteurs en mode « graphique » comme `Knews` et `pan2`.

{% img https://assets.keltia.net/blog/trn4-arbre.png "trn4" "trn4 et la tree-view" %}

UUCP a été à l'origine le mode de transport privilégié de Usenet, en permettant l'échange de courriers électroniques puis de _batches_ (paquets de messages) puis, l'Internet étant arrivé et le protocole {% wp NNTP "NNTP" fr %} créé en 1986, NNTP est devenu la manière de connecter les différents serveurs dans le monde.

Tout modestement, mon petit serveur, `keltia.frmug.fr.net`, connecté uniquement en UUCP _via_ un modem a été dans le Top 1000 des serveurs en octobre 1994 :)

La publicité a toujours été interdite dans à peu près tous les groupes, au point où assez tôt des gens se sont mis à détruire sur des critères techniques des articles clairement en violation des chartes (en émettant un article spécial, appelé _cancel_). Ensuite des robots comme {% wp Cleanfeed_(Usenet_spam_filter) "Cleanfeed (EN)" %} et d'autres ont pris le relais.

Je me souviens que dans ma période la plus prolixe en la matière, vers 1996 j'ai, en un seul mois, détruit plus de 10 000 articles, la majorité venant d'une régurgitation de serveurs Exchange de `microsoft.com`, manifestement Microsoft essayait de faire fonctionner le support NNTP dans Exchange, avec beaucoup de ratés… QuickMail, un outil de messagerie/forums sur MacOS, en a généré beaucoup aussi {% fnin %}La dénomination officielle était _spew_ qui était à distinguer de _spam_.{% endfnin %}.

L'autre anecdote amusante que je n'ai pas eu le temps de raconter à PSES concerne une erreur de traduction : un jour, un non-francophone avait publié un article (dans `fr.misc.divers` peut-être) demandant pourquoi les Français étaient si fan de la plongée sous-marine. Après quelques interrogations, ne comprenant pas de prime abord le rapport avec le sujet et la hiérarchie, je compris… En anglais, « plongeurs » se dit _divers_, venant de _to dive_, et il est clair qu'il n'y a rien de plus proche de _divers_ que « divers » (`fr.misc.divers` `fr.usenet.divers`, etc.). :)

On y aura vu la loi de Godwin, les premiers {% wp Spam "SPAMS" fr %} avec les avocats Canter & Siegel et la "Green Card", les lettres-chaînes du type "MAKE MONEY FAST", les annonces de la naissance de Linux et du Web, de multiples discussions enflammées comme celle entre Andrew Tanenbaum et Linus Torvalds à propos de Linux…

Avec tout ceci, la partie sur les UNIX libres est passé un peu à la trappe, va falloir un 3e article… :)

Merci encore à vous lectrices-lecteurs.  Merci à deuzeffe pour la relecture.

Références
----------
- [La programmation sous UNIX, by Jean-Marie Rifflet, Delmas et Cie, 1986](http://amzn.to/1zLq06W)
- [La communication sous UNIX, 2nd ed., by Jean-Marie Rifflet, Delmas et Cie, 2000](http://amzn.to/1DuR3kt)
- [UNIX Administration, by Jean-Michel Moreno, Ed. Delmas et Cie](http://amzn.to/1DuRwmF)

Les images viennent de Wikipedia Commons sauf celle de René qui vient de [mans.gyptis.org](http://mans.gyptis.org/mw/index.php?title=Fichier:rené_cougnenc.gif) — et stockées en local.

Notes
-----
{%footnotes_inline%}
