---
layout: "post"
title: "la couverture des tests logiciel"
description: "Les tests couvrent, c'est-à-dire rendent service à, ou sont suivis par rapport à, ou contrôlent tels éléments"
mytitle: "Le test ne renvoie t-il qu'à lui-même ?"
myexcerpt: "Exercer une activité de test, c'est-aussi exercer une activité de reporting. Mais encore faut-il que \"le faire savoir\" soit fait intelligemment !"
mylabel: "viser la réassurance"
comments: "Vous êtes parvenus à mettre en place des sortes de conditions de test ? On ne vous demande qu'une couverture des tests par les tests ? Echangons ensemble sur le sujet."
permalink: "couverture-test"
image: "/assets/img/couverture-de-test.png"
categories: []
tags: ["polemique","avancement"]

---
# Que couvre le test ? #

Au risque de vous surprendre, si on est puriste et qu'on rend à César ce qui est à César, **les tests ne couvrent souvent qu'eux-même**. C'est dire le service rendu si on s'arrête là. Mais tâchons de n'être ni mauvaise langue ni polémique. Il convient de rester factuel et de repositionner le débat vis-à-vis d'un référentiel. 

## De quel référentiel je parle ? ##

Cela tombe bien, c'est à cela que sert un référentiel : servir de "base de référence". Et justement, la question véritable à se poser est peut-être : "à quoi est-ce que je veux faire référence quand je parle de couverture ?" 

## Qu'est-ce que la couverture ? ##

Il convient d'apprécier cette notion de *couverture* et de préciser qu'elle se définit en relation avec la notion de *traçabilité*. 
 
- <a id="tracabilite"></a><quote>La tracabilité est la notion statique de mise en place d'une table de relation</quote> (terme très informatique et ETL : table de correspondance ou table de transcodification).
- <a id="couverture-de-test"></a><quote>La couverture est la notion dynamique d'utilisation de cette table de relation à des fins de communication</quote> : d'avancement...

Il s'agit donc de mesurer **la progression d'une exécution de... en relation à...**

## Quel est le meilleur service à rendre ? ##

Maintenant, la question à se poser est : "à qui veux-je rendre service, et quel est le meilleur service à lui rendre ?". Là encore, ne vous en déplaise, **les tests ne servent souvent qu'eux-même**. Attention, ces propos n'engagent que moi et derrière ces généralités se cachent du vécu que je ne peux citer ici.

Pour résumer la situation de départ que je prendrai en référence :

- Les tests couvrent les tests : tests prévus, versus tests réalisés, à date, en cumulatif ou non...
- Les tests servent les tests : les réalisations recouvrent plus ou moins les estimations, ces mêmes estimations définies comme approximations ont tel degré d'approximation...

Vous pouvez voir un exemple de rapport de ce type dans les fiches indicateurs <sub>à venir</sub>.

## Mesure du système de test ##

La mesure devient alors une méta mesure du *processus de test*.

L'étape récurrente du *planifier* voit s'exercer son pendant *contrôler* en vue de strictement mesurer ce qui lui était demandé.

- Mon effort de test a-t-il été atteint ?
- Mes abaques sont-ils à réajuster ?

## Statisfaction du besoin client ##

Pour caricaturer la réaction d'un client critique : "Merci, mais concernant mes cas les plus critiques, mes processus de base, on en est où ?"

Ce que le client voudra certainement, c'est une relation à ce qui lui tient à coeur, ses processus, ses exigences (voir l'article <sub>à venir</sub> sur l'écueil des exigences).
Encore mieux, si vous êtes parvenus à l'éduquer et à **construire ensemble une compréhension commune des enjeux du test** pour son activité : *les conditions de test* constituent un excellent niveau d'agrégat pour les restitutions (voir l'article <sub>à venir</sub> : si je retenais quelque chose de l'ISTQB).

  