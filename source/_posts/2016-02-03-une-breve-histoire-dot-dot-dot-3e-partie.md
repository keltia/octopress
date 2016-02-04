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

J'espère cher/chère lecteur/lectrice que tu voudras bien m'excuser pour ce délai par trop long à mon goût dans la rédaction de cette 3ème partie ; 2015 fut à plein d'égard une difficile année pour moi… Comme d'habitude, toute erreur est mienne et ma mémoire pouvant défaillir, toute correction ou commentaire sera le bienvenu.

{% img https://assets.keltia.net/images/bsd-daemon.png "BSD Daemon" "BSD Daemon" %}

NOTE: la plupart des liens Wikipédia de cet article sont vers les versions françaises desdits articles ; je conseille néanmoins si vous le pouvez d'aller consulter les versions anglaises, beaucoup plus complètes à cet égard que les françaises, malheureusement {% fnin %}La page {% wp 386BSD "386BSD" fr %} en est d'ailleurs un terrible exemple :({% endfnin %}.
<!--more-->
BSD vs Linux
------------

Ah, le titre qui en jette, une petite *flamewar* pour se mettre en jambe ?

En fait non, surtout pas. Ce n'est pas comme ça que tout à commencé, en tout cas pour moi. Rappelons nous l'article précédent, je suis à la faculté de Jussieu Paris VII depuis 1988 après mes deux ans d'IUT d'informatique de gestion à Orsay, ayant donc déjà un peu tâté d'Internet et d'un système BSD (4.2BSD sur Gould).

System V R4
-----------
 
À ce moment, sur ma machine perso — un Compaq 386DX-25, je tourne un MS-DOS 3.31 (de manière à pouvoir gérer plus de 32 Mo {% fnin %}Oui oui, pas d'erreur, on parle bien de méga-octets, remettez ça dans le contexte de l'époque, il y a presque 20 ans…{% endfnin %} sur le disque dur).

Le virus UNIX a pourtant déjà pris et je me mets donc à jouer avec à la maison, principalement en regardant Xenix (oui, celui écrit et utilisé au départ par Microsoft puis distribué par SCO {% fnin %}Le SCO de cette époque n'a rien à voir avec l'actuel, attention. Il s'appelle maintenant {% wp Tarantella_(entreprise) "Tarantella" fr %} alors que c'est la société {% wp "Caldera" fr %} qui s'est renommée SCO puis SCO Group et qui « trolle » le monde du libre avec ses soi-disants brevets ou éléments de propriété intellectuelle liés à Linux).{% endfnin %} qui est un {% wp "System V" fr %} R2 (pas très évolué, pas de *sockets* par exemple donc pas de connexion Internet possible facilement, etc.) et, plus prometteur, le System V R4 de la société Microport.

Ça va me permettre d'ailleurs de m'aperçevoir que ma machine a un souci avec une puce mémoire, dès que je commence à pousser un peu la machine, c'est *panic* sur *panic* dès qu'on rempli la mémoire :( La machine sera assez rapidement remplacée par un {% wp Intel_80486DX "486DX/33" fr %} puis {% wp Intel_80486DX "486DX4/100" fr %} {% fnin %}Contrairement à ce qu'indique le nom, le DX4 a une fréquence *trois* plus élevée entre processus/bus — DX4/100 est un processus à bus de 33 MHz et un CPU à ~100 MHz, les mystères de chez Intel.{% endfnin %} plus tard).

Pour tout dire, l'expérience est aussi décevante qu'à la fac, System V est vraiment pas fait pour moi. En plus pas énormément d'outils de base dans ce système et installer les logiciels libres qui existent (quelques outils GNU par exemple) relève de la gageure, tant les différences entre les différents UNIX sont grandes (c'est ce qui lui a interdit le monde du *desktop* — sans parler de la pauvreté des interfaces graphiques, {% wp X_Window_System "X Window" fr %}, {% wp X_Athena_Widgets "Widgets Athena Xaw (EN)" %} et même {% wp Motif_(bibliothèque_graphique) "Motif" fr %} — n'étant pas d'une richesse graphique très élevée…).

{% img https://assets.keltia.net/images/283px-5.25-Diskette.jpg "5 ¼" "5 ¼" %}

En 1990, un UNIX ça veut dire entre 30 et 50 disquettes 5" 1/4 (*floppy disk* en anglais ou disque souple) voire 77 pour un SCO UNIX System V R3.2 complet avec les *packages* optionels comme TCP/IP (4 disquettes !). Inutile de dire qu'une installation prend du temps, beaucoup de temps d'autant que ces systèmes n'étant pas fournis avec les sources, changer un paramètre du noyau ou ajouter un module dans icelui nécessite de recompiler toute la glue (genre un fichier `.c` par *driver*) et de refaire un noyau et ça prenait de longues minutes sur les machines d'antant…

J'ai aussi l'occasion avec un copain de fac d'assister à ma première conférence en anglais sur le monde UNIX à Paris, organisée par l'AFUU (Association française des utilisateurs d'UNIX), première d'une longue série :)

DESS & IHES
-----------

1991, c'est le moment où je fais mon DESS {% fnin %}On évitera de mentionner que j'ai redoublé la maîtrise hein ? Ça reste entre nous, merci.{% endfnin %} (« Logicles fondamentaux » à Jussieu Paris VII donc) et où je partage mon temps de stage entre l'Université — naissante — de Marne-la-Vallée (merci à jmm — Jean-Michel Moreno pour ce stage !) et le prestigieux {% wp Institut_des_hautes_%C3%A9tudes_scientifiques "IHES" fr %} où — grâce à mon meilleur ami qui m'y avait précédé — j'officie aussi comme ingénieur système pour les différents serveurs Sun3 et Sun4 (donc une Sparcstation 2 toute neuve) pour le mail (EARN/BITNET, pas encore le « vrai » Internet — FRIHES51 ou FRIHES61 était l'adresse du nœud)

{% img https://assets.keltia.net/images/320px-IHES_main_building.jpg "IHES" "IHES" %}

Le réseau de l'IHES comprenait le serveur principal, une Sparcstation 2 (SS2) avec 32 Mo de mémoire pour faire du partage de fichier avec {% wp NFS fr %} et serveur des terminaux X utilisés par les mathématiciens, physiciens et autres astro-physiciens du monde entier qui venaient travailler sur leurs recherches dans l'institut.

X Window était en version 4 (X11R4) à ce moment là, prenant 125 Mo pour les sources et prenant 4h à compiler sur cette machine — machine qui se ferait tailler des croupières par ne serait que le moindre *smartphone* actuel ;-) Sur les machines actuelles, ça doit prendre quelques minutes, ce sont maintenant les mastodontes façon Firefox ou pire, OpenOffice qui prennent des temps équivalents et ce, sur des processeurs 100x plus puissants que le pauvre Sparc de la SS2… 

C'est aussi ma première expérience avec l'hybride SVR4 — 4.2BSD que représente SunOS4 (bientôt appelé dans une tentative de réécriture de l'histoire par Sun Solaris 1). Sun a démarré sa transition du monde BSD vers le monde System V, probablement vu comme plus industriel et moins universitaire. Erreur que j'ai longtemps déploré même si ça avait sans doute un sens en terme de *business*… J'ai l'habitude de dire que ce faisant, Sun a échangé les anciens — mais connus — *bugs* 4.2BSD pour les anciens *bugs* SVR4 {% fnin %}SVRn comme System V Release n, une manière courante à l'époque pour nommer rapidement cette branche d'UNIX.{% endfnin %} et bien entendu les nouveaux *bugs* qu'ils ont introduits eux-même.

Il faut quand même savoir que la première version « réellement » utilisable de Solaris fut la 2.5 (vite mise à jour en 2.5.1 d'ailleurs) vu l'étendue des *bugs* et instabilités des précédentes. Sun a même réussi l'exploit de casser complètement l'API DNS (`gethostbyname(3)` et consorts) en 2.3 ou 2.4 étant passé de mémoire de la pile Lachman d'origine — la même que dans SVR3.2 — à une implémentation maison — un comble pour une API issue de BSD, la famille d'origine de Sun…
   
Ça nous donnait un joyeux mélange de comportements SVR4/BSD selon les {% wp API fr %} avec `/usr/lib` et `/usr/5lib`, un jeu de commande dupliqué entre `/usr/bin` et `/usr/5bin`, etc.

Rappel pour ceux qui voudraient comprendre les ramifications des différentes familles UNIX, le site de référence reste le [site d'Eric Levenez](http://www.levenez.com/unix/) :)

En attendant, ça permettait aux chercheurs de travailler, lire et répondre aux mails, faire du TeX/LaTeX pour leurs papiers, etc. Anecdote marrante par ailleurs sur le dernier point, les secrétaires scientifiques étaient celles qui rédigeaient et corrigeaient les papiers des chercheurs, en TeX, sur Mac et haro sur celui ou celle qui osait suggérer un Word ou un Wordperfect comme alternative !  Nul ne pouvait leur arracher leur TeXtures/Mac :)

{% img https://assets.keltia.net/images/texCode.gif "TeXtures" "TeXtures" %}

Expérience très enrichissante pour moi par ailleurs, baigner dans ce monde multi-culturel m'a beaucoup aidé pour l'anglais et m'a aussi — entre autres choses — de rentrer dans mon boulot actuel en 1996.

Le DESS a été une année intéressante : avec un éventail assez large en terme de connaissances (de Postscript {% fnin %}Oui, le langage de description de page d'Adobe, langage intéressant avec une syntaxe postfixée — arguments puis appel de fonction — qui me donna l'occasion lors d'un exercice d'utiliser la 4ème de couverture d'« Elric le nécromancien « de M. Moorcock comme texte :){% endfnin %} à la théorie de la programmation en passant par le réseau et l'anglais — de retour dans le cursus, j'en avais pas fait depuis l'IUT {%fnin %}Aahhh, tout un poême que ce cours d'anglais qui me vit ridiculiser un de mes co-étudiants au {% wp Test_of_English_as_a_Foreign_Language "TOEFL" fr %} : il avait débarqué en début d'année en roulant des mécaniques, déclarant avoir passé 6 mois ou je ne sais plus au Texas (il en avait certes l'accent incompréhensible). Plus dure fut la chute :){% endfnin %})

BSD UNIX
--------

Même si je n'ai pas l'intention de nous expliquer en détail l'histoire complète d'UNIX depuis sa conception dans les Bell Labs fin des années 60, un petit résumé historique s'impose selon moi.

UNIX est formellement né en 1969 dans les {% wp Laboratoires_Bell "Bell Labs" fr %} (appartenant au géant des télécoms {% wp American_Telephone_%26_Telegraph "AT&T" fr %}) créé notamment par {% wp Ken_Thompson "Ken Thompson" fr %} et {% wp Dennis_Ritchie "Dennis Ritchie" fr %}. Fin des années 70, l'Université de Berkeley en Californie achète une licence à Bell Labs et réalise (merci {% wp Bill_Joy "Bill Joy" fr %} {% fnin %}Également auteur de la pile {% wp Suite_des_protocoles_Internet "TCP/IP" fr %} originelle de Berkeley ainsi que de `vi(1)` et `csh(1)` — le {% wp C_shell "C-Shell" fr %}.{% endfnin %} !) les premières releases appelées BSD, pour *Berkeley Software Distributions*.

BSD est selon moi pendant longtemps la principale source d'innovation dans le monde UNIX, AT&T au départ n'ayant pas vraiment prévu de le vendre de manière industriel mais plus sur un point de vue recherche sur les systèmes d'exploitation. Le principal apport à ce niveau étant en 1983 d'être la plateforme de référence pour les protocoles TCP/IP que l'on connait maintenant et l'API `socket(3)` associées.

J'ai dit que c'était un résumé, voir notamment Wikipedia pour plein d'articles bien plus poussés sur le sujet au combien passionnant mais quelque peu hors sujet ici :)

Dans les années 80 nous avons donc cette famille BSD, maintenant avec les versions 4.x dont 4.2BSD (qui comprend la pile TCP/IP et le {% wp Berkeley_Fast_File_System "Fast File System" fr %} écrit par {% wp Marshall_Kirk_McKusick "Kirk McKusick" fr %}), 4.3BSD (comprenant un nouveau système de mémoire virtuelle et une pile TCP/IP améliorée) et 4.4BSD.

Je passe sur les dernières versions intermédiaires de 4.3BSD (Reno, Tahoe), elles sont importantes en elles-même, moins pour nous à part précéder Net/2. Net/2 est la base de ce qui va nous intéresser maintenant, {% wp 386BSD "386BSD" fr %}. Il faut voir Net/2 comme une tentative de Berkeley de se débarrasser du code AT&T qui traine dans les sources parce que le prix d'une licence est assez prohibitif.

NOTE: Net/2 est aussi à l'origine de la société BSDI (qui devint BSDi en 2000), créée par les members de CSRG à Berkeley (Kirk McKusick, Mike Karels, Bill Jolitz notamment) pour développer et vendre BSD/386, la version commerciale de Net/2. 

386BSD
------

Début 1991, Bill et Lynne Jolitz, vétérans du {% wp Computer_Systems_Research_Group "CSRG (EN)" %} décident dans une série de 18 articles dans le mensuel "Dr. Dobb's Journal" de décrire leur portage de la bande Net/2 sur le processeur Intel i386 — le premier à avoir des fonctionnalités modernes nécessaires au support d'OS modernes tels qu'UNIX {% fnin %}J'entends « moderne » par « sans passer par des hacks affreux » notamment en terme de gestion mémoire. Oui, Xenix a eu une version sur Intel i286, non je ne veux pas perdre 5/10e ou plus à mes yeux en regardant le source.{% endfnin %}.

La liste complète des articles est trouvable dans les liens plus bas ; les articles eux-mêmes sont par contre sûrement très difficiles à retrouver, ça date de 25 ans et sur un suport papier uniquement, pas de Web généralisé encore à cette époque…

Il suffira pour notre article présent de préciser que cette série d'articles fut ce qui me décida à attendre fermement la sortie de 386BSD, prévue en 1992, y compris quand, quelques mois plus tard, sorti un machin venu d'un étudiant finnois appelé à un avenir encore incertain à l'époque, un certain {% wp Linus_Torvalds "Linus Torvalds" fr %} et son bout d'OS, « bootable » mais pas tellement plus {% fnin %}Le processus `init(8)` était en gros le *shell* `/bin/bash` ce qui donne une idée du degré de développement à ce stade. Ça suffit par contre à René (cf. article précédent) pour se lancer avec un bonheur ineffable dedans :){% endfnin %}.

Mon insistance à vouloir mon BSD fut l'occasion de beaucoup de discussions entre René et moi d'ailleurs, se moquant gentiment :) {% fnin %}Tu me manques encore, 'spèce d'idiot — tu dois bien désespérer à voir ce qu'ils font de ta France maintenant d'ailleurs, bisous.{% endfnin %}.

Linus aurait d'ailleurs déclaré que si 386BSD avait été disponible quand il avait commencé Linux, celui-ci n'aurait probabelement jamais été créé… ([Source](https://en.wikiquote.org/wiki/Linus_Torvalds#Attributed)).

Usenet
------

Ordoncque, en mars 1992 sort enfin 386BSD 0.0. Comme la version l'indique, ça démarre, c'est bourré de *bugs* mais ça reste plus complet et pour cause que les premières versions de Linux. 386BSD a l'immense avantage de s'appuyer sur près de 20 ans d'expérience UNIX à Berkeley et ce qui manquait — comme le compilateur — a été comblé par l'utilisation de différents produits GNU comme {% wp GNU_Compiler_Collection "GCC" fr %}.

{% img https://assets.keltia.net/images/386BSD_installer_screenshot.png "386BSD" "386BSD" %}

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

FreeBSD
-------

Le procès AT&T - BSDi
---------------------

Comment parler des systèmes BSD dans le contexte des UNIX libres sans parler du fameux procès


Références
----------

- [Porting UNIX to the 386, Bill & Lynne Jolitz](http://porting-unix-to-the-386.jolix.com/)
- [Porting UNIX to the 386: A Practical Approach, 18-part series in Dr. Dobbs Journal, January 1991 - July 1992](https://groups.google.com/forum/#!original/comp.unix.bsd/uXJjzT4g7qI/mLMsO0hJsV4J)
- [386BSD sur WP, articles, liens (EN)](https://en.wikipedia.org/wiki/386BSD#Further_reading)
- [Dr. Dobb's Journal](http://www.drdobbs.com/)
- {% wp Tanenbaum–Torvalds_debate "Linux vs Minix (EN)" %}
- [Greg Lehey sur 386BSD et les Jolitz (EN)](https://mail-index.netbsd.org/netbsd-advocacy/2001/01/18/0017.html)

Notes
-----
{%footnotes_inline%}
