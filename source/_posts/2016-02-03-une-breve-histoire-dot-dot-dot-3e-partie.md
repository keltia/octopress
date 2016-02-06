---
layout: post
title: "Une brève histoire... 3e partie ! (encore plus LONG)"
date: 2016-02-03 15:06:33 +0100
comments: true
sharing: true
categories: french préhistoire informatique dino pc unix
---

La suite
--------

Après cette [trop] longue interruption de nos émissions, voici enfin la 3ème partie de cette [toujours] brève histoire de *mon* informatique (en toute modestie hein), consacrée cette fois-ci à mon arrivée dans le monde joyeux de l'informatique libre et des {% wp UNIX "UNIX" fr %} libres en particulier. 

À lire après la [première partie](/2015/01/06/une-breve-histoire-de-linformatique/) et la [seconde](/2015/02/01/une-breve-histoire-dot-dot-dot-la-suite/) bien entendu :)

J'espère cher/chère lecteur/lectrice que tu voudras bien m'excuser pour ce délai par trop long à mon goût dans la rédaction de cette 3ème partie ; 2015 fut à plein d'égard une année difficile pour moi… Comme d'habitude, toute erreur est mienne et ma mémoire pouvant défaillir, toute correction ou commentaire sera le bienvenu.

{% img https://assets.keltia.net/images/bsd-daemon.png "BSD Daemon" "BSD Daemon" %}

NOTE: la plupart des liens Wikipédia de cet article sont vers les versions françaises desdits articles ; je conseille néanmoins si vous le pouvez d'aller consulter les versions anglaises, beaucoup plus complètes à cet égard que les françaises, malheureusement {% fnin %}La page {% wp 386BSD "386BSD" fr %} en est d'ailleurs un terrible exemple :({% endfnin %}.
<!--more-->
BSD vs Linux
------------

Ah, le titre qui en jette, une petite *flamewar* pour se mettre en jambe ?

En fait non, surtout pas. Ce n'est pas comme ça que tout à commencé, en tout cas pour moi. Rappelons-nous l'article précédent, je suis à la faculté de Jussieu Paris VII depuis 1988 après mes deux ans d'IUT d'informatique de gestion à Orsay, ayant donc déjà un peu tâté d'Internet et d'un système BSD (4.2BSD sur Gould).

System V R4 (1988-1990)
-----------------------
 
À ce moment-là, sur ma machine perso — un Compaq 386DX-25 tourne un MS-DOS 3.31 (de manière à pouvoir gérer plus de 32 Mo {% fnin %}Oui oui, pas d'erreur, on parle bien de méga-octets, remettez ça dans le contexte de l'époque, il y a presque 20 ans…{% endfnin %} sur le disque dur) qui me sert, entre autres, de support pour le BBS, Finonet, etc.

Le virus UNIX a pourtant déjà pris et je me mets donc à jouer avec à la maison, principalement en regardant Xenix (oui, celui écrit et utilisé au départ par Microsoft puis distribué par Santa Cruz Operations (SCO {% fnin %}Le SCO de cette époque n'a rien à voir avec l'actuel, attention. Il s'appelle maintenant {% wp Tarantella_(entreprise) "Tarantella" fr %} alors que c'est la société {% wp Caldera_(company) "Caldera (EN)" %} qui s'est renommée SCO puis {% wp SCO_Group "SCO Group (EN)" %} et qui « trolle » le monde du libre avec ses soi-disants brevets ou éléments de propriété intellectuelle liés à Linux).{% endfnin %}) qui est un {% wp UNIX_System_V "System V" fr %} R2 (pas très évolué, pas de *sockets* par exemple donc pas de connexion Internet possible facilement, etc.) et, plus prometteur, le System V R4 de la société {% wp Microport "Microport (EN)" %}.

Ça va me permettre d'ailleurs de m'aperçevoir que ma machine a un souci avec une puce mémoire, dès que je commence à pousser un peu la machine, c'est *panic* {% fnin %}Une *panic* est le moment où le système considère qu'il y a trop d'incohérences à un ou plusieurs endroits des données du noyau et décide d'arrêter brutalement la machine, de préférence avec un message d'erreur « utile ».{% endfnin %} sur *panic* dès qu'on rempli la mémoire :( La machine sera assez rapidement remplacée par un {% wp Intel_80486DX "486DX/33" fr %} puis {% wp Intel_80486DX "486DX4/100" fr %} {% fnin %}Contrairement à ce qu'indique le nom, le DX4 a une fréquence *trois* plus élevée entre processus/bus — DX4/100 est un processus à bus de 33 MHz et un CPU à ~100 MHz, les mystères de chez Intel.{% endfnin %} plus tard).

Pour tout dire, l'expérience est aussi décevante qu'à la fac, System V est vraiment pas fait pour moi. En plus pas énormément d'outils de base dans ce système et installer les logiciels libres qui existent (quelques outils GNU par exemple) relève de la gageure, tant les différences entre les différents UNIX sont grandes (c'est ce qui lui a interdit le monde du *desktop* — sans parler de la pauvreté des interfaces graphiques, {% wp X_Window_System "X Window" fr %}, {% wp X_Athena_Widgets "Widgets Athena Xaw (EN)" %} et même {% wp Motif_(bibliothèque_graphique) "Motif" fr %} — n'étant pas d'une richesse graphique très élevée…).

{% img https://assets.keltia.net/images/283px-5.25-Diskette.jpg "Disquette 5 ¼" "Disquette 5 ¼" %}

En 1990, un UNIX ça veut dire entre 30 et 50 disquettes 5" 1/4 (*floppy disk* en anglais ou disque souple) voire 77 pour un SCO UNIX System V R3.2 complet avec les *packages* optionnels comme le réseau TCP/IP (4 disquettes !). Inutile de dire qu'une installation prend du temps, beaucoup de temps d'autant que ces systèmes n'étant pas fournis avec les sources, changer un paramètre du noyau ou ajouter un module dans icelui nécessite de recompiler toute la glue (genre un fichier `.c` par *driver*) et de refaire un noyau et ça prenait de longues minutes sur les machines d'antant… Je n'ai jamais compris comment la compilation de quelques fichiers et l'édition de liens du noyau pouvait prendre tant de temps que ça.

J'ai aussi l'occasion avec un copain de fac d'assister à ma première conférence en anglais sur le monde UNIX à Paris, organisée par l'Association française des utilisateurs d'UNIX (ex-AFUU, maintenant {% wp Association_francophone_des_utilisateurs_du_Net "AFNeT" fr %}), première d'une longue série :)

DESS & IHES (1991)
------------------

1991, c'est le moment où je fais mon DESS {% fnin %}On évitera de mentionner que j'ai redoublé la maîtrise hein ? Ça reste entre nous, merci.{% endfnin %} (« Logiciels fondamentaux » à Jussieu Paris VII donc) et où je partage mon temps de stage entre l'Université — naissante — de Marne-la-Vallée (merci à jmm — Jean-Michel Moreno pour ce stage !) et le prestigieux {% wp Institut_des_hautes_%C3%A9tudes_scientifiques "IHES" fr %} où — grâce à mon meilleur ami qui m'y avait précédé — j'officie aussi comme ingénieur système pour les différents serveurs Sun3 (à base de processeurs Motorola 68010-20-30) et Sun4 (Sparc) pour le mail (EARN/BITNET, pas encore le « vrai » Internet — FRIHES51 ou FRIHES61 était l'adresse du nœud).

{% img https://assets.keltia.net/images/320px-IHES_main_building.jpg "IHES" "IHES" %}

Le réseau de l'IHES comprenait le serveur principal, une {% wp SPARCstation "Sparcstation 2" fr %} (SS2) avec 32 Mo de mémoire pour faire du partage de fichier avec {% wp Network_File_System "NFS" fr %} et serveur des {% wp Terminal_X "terminaux X" fr %} utilisés par les mathématiciens, physiciens et autres astro-physiciens du monde entier qui venaient travailler sur leurs recherches dans l'institut.

X Window était en version 4 (X11R4) à ce moment là, avec 125 Mo pour les sources ce qui prend environ 4h à compiler sur cette machine — machine qui se ferait tailler des croupières par ne serait que le moindre *smartphone* actuel ;-) Sur les machines actuelles, ça doit prendre quelques minutes, ce sont maintenant les mastodontes façon Firefox ou pire, OpenOffice qui prennent des temps équivalents et ce, sur des processeurs 100x plus puissants que le pauvre Sparc de la SS2… 

{% img https://assets.keltia.net/images/sun.sparcstation2.4.jpg "Sparcstation 2" "Sparcstation 2" %}

C'est aussi ma première expérience avec l'hybride SVR4 — 4.2BSD que représente SunOS4 (bientôt appelé dans une tentative de réécriture de l'histoire par Sun, Solaris 1). Sun a démarré sa transition du monde BSD vers le monde System V, probablement vu comme plus industriel et moins universitaire. Erreur que j'ai longtemps déplorée même si ça avait sans doute un sens en terme de *business*… J'ai l'habitude de dire que ce faisant, Sun a échangé les anciens — mais connus — *bugs* 4.2BSD pour les anciens *bugs* SVR4 {% fnin %}SVRn comme System V Release n, une manière courante à l'époque pour nommer rapidement cette branche d'UNIX.{% endfnin %} et bien entendu les nouveaux *bugs* qu'ils ont introduits eux-même.

Il faut quand même savoir que la première version « réellement » utilisable de Solaris fut la 2.5 (vite mise à jour en 2.5.1 d'ailleurs) vue l'étendue des *bugs* et instabilités des précédentes. Sun a même réussi l'exploit de casser complètement l'{% wp Interface_de_programmation "API" fr %} DNS (`gethostbyname(3)` et consorts) en 2.3 ou 2.4 étant passé de mémoire de la pile Lachman d'origine — la même que dans SVR3.2 — à une implémentation maison — un comble pour une API issue de BSD, la famille d'origine de Sun…
   
Ça nous donnait un joyeux mélange de comportements SVR4/BSD selon les API et les chemins utilisés, avec `/usr/lib` et `/usr/5lib`, un jeu de commande dupliqué entre `/usr/bin` et `/usr/5bin`, etc.

Rappel, pour ceux qui voudraient comprendre les ramifications des différentes familles UNIX, le site de référence reste le [site d'Eric Levenez](http://www.levenez.com/unix/) :)

En attendant, ça permettait aux chercheurs de travailler, lire et répondre aux mails, faire du TeX/LaTeX pour leurs papiers, etc. Anecdote marrante par ailleurs sur le dernier point, les secrétaires scientifiques étaient celles qui rédigeaient et corrigeaient les papiers des chercheurs, en TeX, sur Mac et haro sur celui ou celle qui osait suggérer un Word ou un Wordperfect comme alternative !  Nul ne pouvait leur arracher leur TeXtures/Mac :)

{% img https://assets.keltia.net/images/texCode.gif "TeXtures" "TeXtures" %}

Expérience très enrichissante pour moi par ailleurs, baigner dans ce monde multi-culturel m'a beaucoup aidé pour l'anglais et m'a aussi — entre autres choses — permis de rentrer dans mon boulot actuel en 1996 (en plus d'être chez Hervé Schauer Consultants évidemment).

Le DESS a été une année intéressante : avec un éventail assez large en terme de connaissances (de Postscript {% fnin %}Oui, le langage de description de page d'Adobe, langage intéressant avec une syntaxe postfixée — arguments puis appel de fonction — qui me donna l'occasion lors d'un exercice d'utiliser la 4ème de couverture d'« Elric le nécromancien « de M. Moorcock comme texte :){% endfnin %} à la théorie de la programmation en passant par le réseau et l'anglais — de retour dans le cursus, j'en avais pas fait depuis l'IUT {%fnin %}Aahhh, tout un poême que ce cours d'anglais qui me vit ridiculiser un de mes co-étudiants au {% wp Test_of_English_as_a_Foreign_Language "TOEFL" fr %} : il avait débarqué en début d'année en roulant des mécaniques, déclarant avoir passé 6 mois ou je ne sais plus au Texas (il en avait certes l'accent incompréhensible). Plus dure fut la chute :){% endfnin %})

BSD UNIX
--------

Même si je n'ai pas l'intention de nous expliquer en détail l'histoire complète d'UNIX depuis sa conception dans les Bell Labs fin des années 60, un petit résumé historique s'impose néanmois.

UNIX est formellement né en 1969 dans les {% wp Laboratoires_Bell "Bell Labs" fr %} (appartenant au géant des télécoms {% wp American_Telephone_%26_Telegraph "AT&T" fr %}) créé notamment par {% wp Ken_Thompson "Ken Thompson" fr %} et {% wp Dennis_Ritchie "Dennis Ritchie" fr %}. Fin des années 70, l'Université de Berkeley en Californie achète une licence à Bell Labs et réalise (merci {% wp Bill_Joy "Bill Joy" fr %} {% fnin %}Également auteur de la pile {% wp Suite_des_protocoles_Internet "TCP/IP" fr %} originelle de Berkeley ainsi que de `vi(1)` et `csh(1)` — le {% wp C_shell "C-Shell" fr %}.{% endfnin %} !) les premières releases appelées BSD, pour *Berkeley Software Distributions*.

{% img https://assets.keltia.net/images/240px-Seal_of_University_of_California_Berkeley.svg.png "Logo University of California Berkeley" "Logo University of California Berkeley" %}

BSD est selon moi pendant longtemps la principale source d'innovation dans le monde UNIX, AT&T au départ n'ayant pas vraiment prévu de le vendre de manière industriel mais plus sur un point de vue recherche sur les systèmes d'exploitation. Le principal apport à ce niveau étant en 1983 d'être la plateforme de référence pour les protocoles TCP/IP que l'on connait maintenant et l'API `socket(3)` associées.

J'ai dit que c'était un résumé, voir notamment Wikipedia pour plein d'articles bien plus poussés sur le sujet au combien passionnants mais quelque peu hors sujet ici :)

Dans les années 80 nous avons donc cette famille BSD, maintenant avec les versions 4.x dont 4.2BSD (qui comprend la pile TCP/IP et le {% wp Berkeley_Fast_File_System "Fast File System" fr %} écrit par {% wp Marshall_Kirk_McKusick "Kirk McKusick" fr %}), 4.3BSD (comprenant un nouveau système de mémoire virtuelle et une pile TCP/IP améliorée) et 4.4BSD.

Je passe sur les dernières versions intermédiaires de 4.3BSD (Reno, Tahoe), elles sont importantes en elles-même, moins pour nous à part précéder Net/2. Net/2 est la base de ce qui va nous intéresser maintenant, {% wp 386BSD "386BSD" fr %}. Il faut voir Net/2 comme une tentative de Berkeley de se débarrasser du code AT&T qui traine dans les sources parce que le prix d'une licence est assez prohibitif.

NOTE: Net/2 est aussi à l'origine de la société {% wp Berkeley_Software_Design "BSDI (EN)" %} (qui devint BSDi en 2000), créée par les members de CSRG à Berkeley (Kirk McKusick, Mike Karels, Bill Jolitz notamment) pour développer et vendre {% wp BSD/OS "BSD/386 (EN)" %}, la version commerciale de Net/2. 

386BSD (1992-1993)
------------------

Début 1991, Bill et Lynne Jolitz, vétérans du {% wp Computer_Systems_Research_Group "CSRG (EN)" %} décident dans une série de 18 articles dans le mensuel "Dr. Dobb's Journal" de décrire leur portage de la bande Net/2 sur le processeur Intel i386 — le premier à avoir des fonctionnalités modernes nécessaires au support de {% wp Système_d%27exploitation "systèmes d'exploitation" fr %} (OS) modernes tels qu'UNIX {% fnin %}J'entends « moderne » par « sans passer par des hacks affreux » notamment en terme de gestion mémoire. Oui, Xenix a eu une version sur {% wp Intel_80286 "80286" fr %}, non je ne veux pas perdre 5/10e ou plus à mes yeux en regardant le source.{% endfnin %}.

La liste complète des articles est trouvable dans les liens plus bas ; les articles eux-mêmes sont par contre sûrement très difficiles à retrouver, ça date de 25 ans et sur un suport papier uniquement, pas de Web généralisé encore à cette époque…

Il suffira pour notre article présent de préciser que cette série d'articles fut ce qui me décida à attendre fermement la sortie de 386BSD, prévue en 1992, y compris quand, quelques mois plus tard, sorti un machin venu d'un étudiant finnois appelé à un avenir encore incertain à l'époque, un certain {% wp Linus_Torvalds "Linus Torvalds" fr %} et son bout d'OS, « bootable » mais pas tellement plus {% fnin %}Le processus `init(8)` était en gros le *shell* `/bin/bash` ce qui donne une idée du degré de développement à ce stade. Ça suffit par contre à René (cf. article précédent) pour se lancer avec un bonheur ineffable dedans :){% endfnin %}.

Mon insistance à vouloir mon BSD fut l'occasion de beaucoup de discussions entre René et moi d'ailleurs, lui se moquant gentiment {% fnin %}Tu me manques encore, 'spèce d'idiot — tu dois bien désespérer à voir ce qu'ils font de ta France maintenant d'ailleurs, bisous.{% endfnin %} et moi cherchant à le convertir :).

Linus aurait d'ailleurs déclaré que si 386BSD avait été disponible quand il avait commencé Linux, celui-ci n'aurait probabelement jamais été créé… ([Source](https://en.wikiquote.org/wiki/Linus_Torvalds#Attributed)).

Usenet
------

Ordoncque, en mars 1992 sort enfin 386BSD 0.0. Comme la version l'indique, ça démarre, c'est bourré de *bugs* mais ça reste plus complet et pour cause que les premières versions de Linux. 386BSD a l'immense avantage de s'appuyer sur près de 20 ans d'expérience UNIX à Berkeley et ce qui manquait — comme le compilateur — a été comblé par l'utilisation de différents produits GNU comme {% wp GNU_Compiler_Collection "GCC" fr %}.

{% img https://assets.keltia.net/images/386BSD_installer_screenshot.png "Installer de 386BSD" "Installer de 386BSD" %}

On a déjà les bases de ce qui différencie les BSD en général des Linux : un système de base auto-suffisant (*shells*, compilateurs, utilitaires, etc.) dès la sortie de la « boîte » et tout le reste (ce qu'on appelle maintenant les *packages*) à ajouter — entendre « récupérer, compiler, installer et configurer » — après coup. 

Je vois évoluer Linux, c'est très intéressant d'ailleurs et l'épisode de la discussion entre Linus et Andy Tanenbaum (cf. plus bas) le montre bien, la génèse a été semée d'embûches pour les deux systèmes.

Les deux systèmes sont bien présents sur {% wp Usenet "Usenet" fr %}, l'un dans `comp.os.linux` et l'autre dans `comp.unix.bsd.386bsd.*` {% fnin %}La différence de placement dans la hiérarchie `comp` des deux systèmes fut sujette à moultes discussions, les BSDistes trouvant dommage d'être relégués dans un morceau de `comp.unix.bsd` et les Linuxiens regrettant d'être considéré comme un « moindre » UNIX...{% endfnin %}.

Pourquoi mentionner Usenet dans ce contexte ?

Parce que bien plus que les *mailing-lists* (liste de discussion/diffusion) qui sont le reflet de l'avancée des systèmes au jour le jour entre développeurs, Usenet est pendant longtemps l'endroit où vont s'affronter — parfois littéralement — les partisans des deux systèmes. Voire entre partisans de chaque camp comme on va le voir maintenant…

Usenet fut donc le théâtre d'une des plus grosses *flamewars* qui vit au final la scission entre BSDistes et la création en 1993 de {% wp NetBSD "NetBSD" fr %} puis {% wp FreeBSD "FreeBSD" fr %}. Il faut voir qu'à la sortie de 386BSD 0.0 puis 0.1, le système était relativement instable et les *bugs* foisonnaient. 386BSD attira beaucoup d'adeptes venant du monde BSD (ou pas) et ceux-ci commencèrent à écrire des *patches* qu'il envoyèrent à Bill & Lynne Jolitz pour améliorer et stabiliser le système.

Il faut dire que les Jolitz n'accueillirent pas cette initiative avec un enthousiasme débordant et Jordan Hubbart, Terry Lambert, Rod Grimes et Nate Williams principalement (la liste est longue) créèrent donc le fameux « patchkit », mis à jour régulièrement et devant être appliqué afin d'avoir un système utilisable.

Discussion après discussion, il devient clair que les mainteneurs du *patchkit* ne pourront jamais s'entendre avec les Jolitz et ça s'envenime sur Usenet et à un moment, Lynne ira jusqu'à déclarer que 1/3 du *patchkit* est nul, 1/3 est mal écrit et j'ai oublié ce qu'elle pensait du 1/3 restant… Bref, là où Bill corrigeait régulièrement BSD/386 au sein de BSDI, il refusa systématiquement d'intégrer le *patchkit*.

Nul ne sait pourquoi les Jolitz eurent cette attitude (je ne me souviens pas que l'existence de BSDI et que Bill y travaillait ait été mentionné à l'époque) mais le premier résultat fut qu'un groupe d'utilisateurs, fatigués d'attendre la 1.0 de 386BSD promise par les Jolitz s'en allèrent créer {% wp NetBSD "NetBSD" fr %}, menés par C. Demetriou, A. Glass, T. Deraadt et C. Hannum. Leur but affiché était de porter NetBSD sur à peu près tout ce qui avait un processeur et de la mémoire {% fnin %}D'où le slogan de NetBSD "Of course it runs NetBSD" et l'image du *toaster* (grille-pain) associée ;-){% endfnin %}.

À ce moment, les gens du *patchkit* et ceux de NetBSD partagent une machine hébergée à l'Université de Berkeley appelée `sun-lamp.cs.berkeley.edu`, utilisant déjà {% wp Concurrent_versions_system "CVS" fr %} comme outil de gestion de versions. Les relations entre les deux groupes finissent par se dégrader très rapidement après la création de NetBSD et la *flamewar* devient très grave en avril-mai 1993 avec publication par Demetriou ou Deraadt du contenu du fichier `.history` {% fnin %}Ce fichier regroupe l'ensemble des commandes tapée par un utilisateur de manière automatique. Qu'un utilisateur se permette d'utiliser des privilèges de super utilisateur pour aller le consulter est considéré comme une violation de la vie privée par tout ingénieur système responsable.{% endfnin %} de Jordan Hubbard pour essayer de l'accuser de « vol » de code.

En bref, une descente du niveau des discussions largement en dessous de la ceinture qui n'est à l'honneur de personne. C'est à ce stade de l'histoire qu'il faut que je mentionne que c'est précisément les actions du trio Demetriou, Deraadt & Hannum qui me poussèrent à rejoindre FreeBSD quelques mois après, ulcéré que j'étais de leurs actions.

Après quelques tentatives de créer une sorte de 386BSD 0.2, Jordan Hubbard, Terry Lambert, Rod Grimes et David Greenman finiront par créer FreeBSD en juillet 1993 et réussissent à sortir la première version 1.0 en décembre 1993.

FreeBSD (1993-)
---------------

Voici comment j'ai pris le train FreeBSD et que je ne l'ai plus quitté depuis :)

Peu de temps après cette 1.0 est sortie 1.0.2 puis c'est parti sur la branche 1.1, déjà dénommée CURRENT, expression classique pour désigner la branche de code en cours de développement. Celui-ci se passe principalement au travers des listes de discussions, les plus connues (à part les listes privées des développeurs) étant `freebsd-current`, `freebsd-hackers`, `freebsd-arch` et plein plein d'autres, classées par sujet ou architecture.

À la base, le but de FreeBSD est d'améliorer et faire progresser BSD sur la plateforme Intel sans trop se préoccuper d'autres plateformes plus « exotiques » comme la famille Motorola (68000 et consorts — comme le Mac ou l'Amiga) et autres Sparc ; toutes ces architectures largement moins utilisées ou moins documentées ayant tendance à monopoliser des développeurs. C'est là la principale différence au départ entre NetBSD et FreeBSD. Ça reste encore vrai aujourd'hui même si les deux (et maintenant plus) systèmes partagent si ce n'est du code, tout du moins des plateformes. Ça évoluera bien entendu au fil des années (l'intégration du support {% wp DEC_Alpha "Alpha" fr %} 64 bits venant de NetBSD par exemple nous redonnera cet aspect multi-plateformes). 

De son côté pendant 1993-1994, NetBSD sortira 0.8 et 0.9 et enfin 1.0 en octobre 1994. 

Linux continue de se développer dans son coin, acquérant de plus en plus d'utilisateurs et de développeurs, il arrive à sa version 1.0 assez complète en mars 1994.

Mais se profile déjà l'événement qui va bouleverser les deux écosystèmes de manière durable, donnant une avance à Linux que les BSD dans leur ensemble  ne rattraperont jamais sauf à considérer que l'adoption du code BSD dans MacOS X a projeté BSD dans plus de machines que Linux, dans le grand public du moins.

Le procès AT&T - BSDI (1993 - 1994)
-----------------------------------

Comment parler des systèmes BSD dans le contexte des UNIX libres sans parler du fameux procès entre {% wp Unix_System_Laboratories "Unix Systems Laboratories (EN)" %} (ex-Bell Labs) et la société BSDI ?  Cette dernière, créée donc par des membres de CSRG (voir au dessus) dont Bill Jolitz, récupère le code Net/2, y ajoute les éléments manquants — notons le parallèle avec le *patchkit*, il y a duplication du boulot — et vend le résultat sous le nom BSD/386. 

Ils vont surtout dans leur enthousiasme (inconscience ? :)) en faire de la publicité au travers d'un mécanisme classique aux USA, l'utilisation des lettres pouvant exprimer un numéro de téléphone (qui s'en souviens ici hmmmm ? :)) et vont donc prendre un numéro s'exprimant par 0800-ITS-UNIX. Notons le UNIX à la fin, il va être *très* important très vite.

L'histoire retiendra qu'USL — filiale d'AT&T — a utilisé cette violation présumée (et assumée par BSDI puisque tout le but de la campagne de dire que c'est un UNIX) de sa propriété intellectuelle (PI) sur la marque UNIX pour déclencher un procès arguant qu'outre cette question — assez secondaire il faut le dire — de PI, BSDI a violé les termes de la licence UNIX que possédait l'Université de Berkeley (non citée de prime abord) et qu'elle n'aurait pas du rendre disponible Net/2. Du coup le juge leur demande soit d'impliquer l'Université de Berkeley (UCB) ou de laisser tomber.

USL choisit de redéposer sa plainte en impliquant UCB en plus de BSDI. Après d'intenses échanges avec le juge au travers de moultes papiers écrit par les membres de CSRG, tous les points soulevés par USL sauf deux sont rejetés et suite à ça, l'Université décide de contre-attaquer par une plainte de son côté, arguant que USL de son côté avait failli à l'obligation de reconnaitre la contribution {% fnin%}C'est une des clauses les plus connues de la licence BSD originale — cf. [cette page WP](https://en.wikipedia.org/wiki/BSD_licenses#4-clause_license_.28original_.22BSD_License.22.29){% endfnin %} d'UCB dans le code System V.

Il se trouve que peu après le début du double procès, USL va être rachetée par Novell et grâce entre autres à l'intervention de Ray Noorda (PDG de Novell) qui déclare préférer la compétition sur le marché plutôt que dans les cours de justice, le procès va se régler à l'amiable, ça va juste prendre beaucoup de temps et ce n'est qu'en janvier 1994 que les deux parties arrivent à un accord.

Il *faut* à ce propos voir la conférence de Kirk sur les 20 ans d'UNIX à Berkeley (cf. plus bas). Il l'a donnée durant l'une des dernières
 conférences BSDCon en Californie pendant près de 2h, un verre de bière à la main {% fnin %}Et après s'être assuré que tout le monde en voulant également avait le temps d'aller en chercher ! :){% endfnin %} ! Kirk est un excellent conteur et racontée ainsi, ces événements assez lourds à l'époque deviennent presque amusants…

{% img https://assets.keltia.net/blog/kirk-26338.jpg "Kirk McKusick" "Kirk McKusick" %}

Sans rentrer dans les détails, 3 fichiers sont enlevés de 4.4BSD (qui restera comme 4.4BSD-Encumbered), d'autres sont modifiés, un copyright AT&T est ajouté dans plein d'autres et s'en suit la création de 4.4BSD-Lite, la base de NetBSD et FreeBSD puisqu'au terme de cette accord, la redistribution de systèmes dérivés se serait pas impacté *si* ils se basaient sur 4.4BSD-Lite.

À ce moment, FreeBSD et NetBSD vont prendre une approche radicalement opposée et si ça n'aura pas d'impact pour les utilisateurs, celui sur les développeurs sera plus profond du côté NetBSD :

- FreeBSD décide de repartir des sources « vierges » de 4.4BSD-Lite et d'y ré-appliquer les modifications dévéloppées depuis. Un nouveau dépôt CVS est donc créé avec les sources de 4.4BSD-Lite ;
- NetBSD eux décident de garder leur dépôt CVS et d'y incorporer les sources de 4.4BSD-Lite.

La conséquence est que le dépôt CVS de NetBSD ne sera pas disponible pour le reste du monde pendant pas mal de temps vu qu'à un certain moment dans le temps (le but d'un système de gestion de sources est justement de garder précieusement cet historique !) il est toujours emcombré des sources problématiques Net/2…

Ça n'a peut-être pas l'air très important en soi, surtout 20 ans après mais c'est la chose qui a découragé plein de développeurs et sans doute de boîtes commerciales de l'aventure BSD et ceux-ci se sont tournés vers Linux, lui donnant un élan qui n'a pas été rattrapé comme je le disais avant.

C'est la vie©®

L'année d'après, arrive l'expulsion de Theo Deraadt de la *core team* de NetBSD, lequel ira fonder OpenBSD pour se consacrer aux aspects sécurité avec audit de code, intégration de code tiers pour le maîtriser {% fnin %}La formule « diplomatique » pour *fork*, sachant que ça a pour conséquence de compliquer la maintenance a fortiori si le code en question est abandonné après par les auteurs originaux cf. bind4…{% endfnin %}. Il a en cela partiellement réussi son coup selon moi : oui, surtout au départ, OpenBSD a été plus sécurisé que les deux autres mais je pense que les autres l'ont rattrapé. Et Theo n'a pas manqué de montrer à quel point NetBSD avait eu raison de se séparer de lui ; son attitude a toujours été très agressive allant jusqu'à menacer de pirater FreeBSD (et s'est fait bannir des listes de diffusion).

Cathédrale et bazar
-------------------

Petit aparté sur les modèles de développement des UNIX libres :

Dans son fameux papier de 1999 intitulé « The Cathedral and the Bazaar » {% fnin %}Voir la page WP en français {% wp La_Cath%C3%A9drale_et_le_Bazar "La cathédrale et le bazar" fr %} ou celle plus complète là encore en {% wp The_Cathedral_and_the_Bazaar "anglais" %}{% endfnin %}, Eric S. Raymond, bien connu dans le monde Linux (et également comme activiste pro-armes/NRA) a théorisé les modèles de développement utilisés par le monde Linux et le monde BSD.

Je l'ai toujours trouvé trop partial d'un côté et pas totalement adapté à la réalité de l'autre côté surtout sur la supposée rigidité apportée par la cathédrale (à voir le nombre élevé de développeurs dans FreeBSD par exemple). La réalité n'est jamais aussi tranchée, notez par exemple que Linus est un « dictateur éclairé » pour certains aspects de Linux alors que FreeBSD élit sa *core team* tous les deux ans. Enfin, il me parait difficile de comparer des OS complets du côté BSD et un « simple » noyau du côté de Linux, sans les distributions on ne ferait pas grand chose avec… 

Et moi ?
--------

Le but n'est pas en soi de parler de moi dans cette série, plus de relater les événements tels que je les ai vécus. 

Néanmoins, puisqu'on parle d'histoire : je deviens committer {% fnin %}Ce terme désigne une personne ayant le droit d'incorporer des changements (*commit* en anglais) dans le code du projet par opposition à juste contributeur.{% endfnin %} FreeBSD le 20 février 1995, 2e français après Jean-Marc Zucconi (décédé depuis malheureusement, la release 7.0 lui est dédiée ainsi qu'à Jonathan Lemon) pour m'occuper de la Foire aux questions (FAQ {% fnin %}*Frequently Asked Questions* en anglais, merci à nos amis québécois pour cette superbe traduction qui préserve l'acronyme !{% endfnin %}) et de ce qui deviendra le *Handbook*, pièce maîtresse de la documentation de FreeBSD. J'avais décidé de réécrire cette FAQ originellement en mode texte tout bête dans un format plus pratique, hypertexte en utilisant le *package* {% wp LinuxDoc "linuxdoc-sgml (EN)" %} créé par Matt Welsh pour Linux. 

C'est ainsi que le projet FreeBSD a adopté `linuxdoc-sgml`pour toute sa documentation. Maintenant, nous utilisons plutôt {% wp DocBook "DocBook" fr %} dans sa version {% wp XML "XML" fr %} (et plus {% wp SGML "SGML" fr %}), plus complet (et plus verbeux).

Après deux ans dans la documentation, je suis passé au développement dans le noyau en 2007-2008 et j'ai travaillé un temps dans la partie *Virtual File System* (VFS) et les systèmes de fichiers empilables (*stackable filesystems*) avec `unionfs` et `nullfs`. Maintenant, ayant malheureusement moins de temps à consacrer à FreeBSD, je m'occupe de quelques ports et un peu de {% wp Ntpd "ntpd(8)" fr %} dans le système de base ({% wp Network_Time_Protocol "NTP" fr %} pour le protocole).

Je reste un fervent supporter de FreeBSD qui est, pour mes besoins et mes centres d'intérêt, le meilleur UNIX libre pour tout ce qui concerne la partie serveur, le côté *desktop* ayant basculé en 2003 sur MacOS X qui est la plus ergonomique et la plus utilisable des interfaces graphiques. Tous mes serveurs tournent FreeBSD avec {% wp ZFS "ZFS" fr %} pour assurer l'intégrité de mes données (chiffrées bien sûr).

Conclusion
----------

Je vais, pour cette troisième partie m'arrêter là, il en reste plein à dire sur la suite de cette histoire, merci chère lectrice — cher lecteur d'être arrivé si loin :)

PS : merci à deuzeffe pour la relecture :)

Références
----------

- [Porting UNIX to the 386, Bill & Lynne Jolitz](http://porting-unix-to-the-386.jolix.com/)
- [Porting UNIX to the 386: A Practical Approach, 18-part series in Dr. Dobbs Journal, January 1991 - July 1992](https://groups.google.com/forum/#!original/comp.unix.bsd/uXJjzT4g7qI/mLMsO0hJsV4J)
- [386BSD sur WP, articles, liens (EN)](https://en.wikipedia.org/wiki/386BSD#Further_reading)
- [Dr. Dobb's Journal](http://www.drdobbs.com/)
- {% wp Tanenbaum–Torvalds_debate "Linux vs Minix (EN)" %}
- [Greg Lehey sur 386BSD et les Jolitz (EN)](https://mail-index.netbsd.org/netbsd-advocacy/2001/01/18/0017.html)
- [Le procès décrit par Kirk McKusick (EN)](http://www.oreilly.com/openbook/opensources/book/kirkmck.html)
- [20 years of Berkeley UNIX, Kirk McKusick](http://www.mckusick.com/history/index.html)
- [Essai d'Eric S. Raymond, The Cathedral and the Bazaar (EN)](http://www.catb.org/~esr/writings/cathedral-bazaar/)
- [Site de Kirk McKusick](http://mckusick.com/)

- [Projet FreeBSD](https://www.FreeBSD.org/)
- [Projet NetBSD](https://netbsd.org/)
- [Projet OpenBSD](http://www.openbsd.org/)
- [Linux Documentation Project](http://www.tldp.org/)

Images de Wikipédia sauf pour la SS2 (http://sunstuff.org/pictures/).

Notes
-----
{%footnotes_inline%}
