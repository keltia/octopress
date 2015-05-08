---
layout: post
title: "Métadonnées ! Mais où ça ?"
date: 2015-05-08 20:22:23 +0200
comments: true
sharing: true
categories: politique renseignement french libertés Internet métadonnées
---

Ce titre à lui tout seul sous forme de jeu de mot reflète la situation actuelle née du vote de la loi dite du Renseignement le mardi 5 mai 2015. Pendant toute la discussion sur le projet de loi à l'Assemblée nationale, une ambigüité a été entretenue de haut vol — par les auteurs de la loi, pas le ministre ; lui ne fait sans doute pas la différence — sur le sujet des métadonnées.

>En gros, la notion que nous autres informaticiens avons de ces métadonnées ne sont pas les mêmes que celle des services de renseignement.

Cette ambigüité est très importante et permet au ministre de ne probablement pas [trop] mentir quand il déclare ne pas vouloir faire de {% wp Deep_packet_inspection "DPI" fr %} dans les fameuses boîtes noires {%fnin%}Cette appellation vient de Matignon, pas des opposants contrairement à ce que certains soutiens à la loi essayent de faire croire.{%endfnin%}.
<!--more-->
Sous le terme quelque peu barbare (et anglais) de DPI, se cache un ensemble de techniques d'inspection plus ou moins approfondies des paquets {% wp Internet_Protocol "IP" fr %} sur le réseau. Pour nous autres informaticiens, ces métadonnées sont très réduites à ce niveau, se limitant en gros à « quelle machine dialogue avec quelle autre et comment ». C'est la seule chose que pourraient voir les fameuses boîtes noires si elles ne font pas de DPI. 

>Si si rien de plus. Toutes les autres métadonnées sont à *l'intérieur* des paquets.

Ca permet déjà beaucoup puisque ça permet de savoir que la machine A s'est connectée à Facebook ou que la machine B a récupéré du courrier chez Free. Ou que la machine C est allé se connecter au serveur `www.islamic-news.fr`. Pas de notion d'utilisateur là dedans. Les composantes de l'Internet n'ont pas besoin de plus pour s'échanger des paquets dans le monde entier.

Je pense que nous pouvons nous accorder sur le fait que ce soit tout à fait insuffisant pour les services de renseignement. Eux veulent savoir qui échange du mail avec qui, qui va voir telle ou telle page sur un site ou encore va regarder des pages pro-jihad sur Facebook. On voit que sans DPI, ils ne vont pas pouvoir voir grand chose.

Même la supposition « une adresse IP = un utilisateur » est assez rapidement fausse : supposons que j'invite des amis chez moi ; je suis un gars sympa, je vais leur donner le mot de passe de la borne Wifi pour leur permettre de se connecter. Vu la manière dont la plupart des foyers se connectent à Internet, tout le trafic que nous allons ainsi générer ne sera visible que sous la forme de « mon adresse IP s'est connectée à A, B, C et plein d'autres machines ». Aucun moyen de savoir si c'est moi ou d'autres qui l'avons généré.

De même, en examinant les paquets constituant une connexion à un serveur de courrier électronique utilisant le protocole {% wp Simple_Mail_Transfer_Protocol "SMTP" fr %}, on ne saura jamais qui écrit à qui. Le savoir suppose d'aller voir le contenu des paquets TCP et extraire les champs `From:` et `To:` pour connaitre expéditeur et destinataire(s). 

Pour Facebook, pareil il faudrait aller regarder dans les paquets eux-même pour extraire la partie droite de l'adresse, (ce qui est après le `facebook.com`) et ainsi de suite.

Or, la plupart des protocoles IP sont ainsi fait que seule une analyse approfondie (le *Deep* de DPI) permet d'extraire ces métadonnées… Ne serait-ce que pouvoir filtrer les sites pro-jihad suppose de détourner les paquets {% wp Domain_Name_System "DNS" fr %} et donc inspecter la requête du client. Tout vient de ce que la couche inférieure transporte le contenu qui lui est fourni par la couche au dessus et ainsi de suite.

>les métadonnées du niveau IP ne sont pas dans la même couche que les metadonnées SR

En résumé, « nos » métadonnées sont dans les couches 2 à 4 (IP et TCP/UDP/ICMP) alors que la majorité des leurs sont en couche 7 (applications). 

L'article de notre ami [Numendil](https://twitter.com/Numendil) reflète bien l'interrogation des informaticiens.

Autre point qui est symptomatique des différences entre les deux mondes :

>Les services de renseignement disent qu'il n'y a surveillance que si un humain en espionne un autre

Dans ce contexte, la surveillance de masse par les boîtes noires n'est que de la collecte automatisée pour eux et justifie tout à fait leurs déclarations.

Donc les boîtes noires, pour extraire les métadonnées utilisables par les SR vont *forcément* faire du DPI. Et ne présenter que ces metadonnées dans un format utilisable par les SR. Et l'intégralité de ces métadonnées  — nécessaires pour une analyse hors-ligne dans le temps — sera forcément lue, interprêtée et surtout *stockée*… {% fnin %}Pas l'intégralité du trafic évidemment, on ne peut pas dupliquer tout le trafic ainsi.{% endfnin %}

Pire, pour le trafic chiffré, il sera conservé tant qu'il n'aura pas été décrypté (soit par cassage du système de chiffrement soit par obtention de la clé par d'autres méthodes {% fnin %}Sans rentrer dans les considérations de *Forward Secrecy* ou {% wp Confidentialité_persistante "Confidentialité persistante" fr %} en français.{% endfnin %}). 

Quant à l'affirmation dans la loi même de la non surveillance des professions dites protégées comme les journalistes, les avocats voire les parlementaires eux-mêmes, elle ne tient pas très longtemps non plus : pour les reconnaitre, il faudra bien extraire ces informations avant de pouvoir décider de ne pas les conserver (sans blague, qui y croit encore ?). Il sera donc *trop tard*…

Sans parler bien évidemment de l'accès qu'ils pourront avoir chez les fournisseurs d'accès/hébergeurs au travers de l'équivalent français de {% wp PRISM_(programme_de_surveillance) "PRISM" fr %} et qui permet de compléter les informations et les croiser. Trop parano ? Peut-être. Ou pas.

L'exemple le plus concret nous a été fourni par François de Rugy {% fnin %}M. de Rugy est député du groupe écologiste comme [Sergio Coronado](https://twitter.com/sergiocoronado) mais il a lui voté *POUR* la loi et tente tant bien que mal de la justifier avec les éléments de langage du gouvernement. Un appel du pied assez mal déguisé en fait… {% endfnin %} lui-même sur Twitter il y a deux jours ; un utilisateur a reçu par courrier électronique une réponse du député, au format Word et a été voir le fichier :

{% blockquote @FdeRugy https://twitter.com/FdeRugy/status/595901759308079104 %}
Livrer en pâture le nom d'un salarié parce qu'on combat son patron :  éthique du net, vie privée, toussa toussa... ?{% endblockquote %}

Le nom de son assistant parlementaire est stocké dans les métadonnées du fichier Word, donnée qui ne peut être connue qu'en allant le lire. CQFD.

Merci à Agnès, Pierre et Jean-Baptiste pour la relecture. 

Références
----------
- [Pixellibre - DPI ou pas ?](http://pixellibre.net/2015/04/les-boites-noires-si-ce-nest-pas-du-dpi-quest-ce-que-ca-sera/)
- [La loi expliquée à mes parents](http://blog.jbfavre.org/2015/04/07/loi-renseignement-expliquee-simplement/)
- [La pilule, quelle couleur ?](http://blog.jbfavre.org/2015/04/20/la-pilule-vous-la-preferez-bleue-ou-rouge/)
- [Métadonnées et EU.org](http://signal.eu.org/blog/2015/04/20/eu-org-les-metadonnees-et-la-loi-renseignement/)
- [B. Cazeneuve @libe](http://www.liberation.fr/societe/2015/04/10/parler-de-surveillance-generalisee-est-un-mensonge_1238662) 

Notes
-----
{%footnotes_inline%}
