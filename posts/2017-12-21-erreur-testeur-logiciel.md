---
layout: "post"
title: "erreur humaine introduisant un défaut logiciel"
description: "L'humain est faillible et \"fait des erreurs\", en test logiciel comme ailleurs. Le testeur peut avoir tort, mais pas sans raisons."
mytitle: "J'ai tort, et alors ?"
myexcerpt: "Le testeur peut avoir tort, mais pas sans raisons."
mylabel: "apprendre des erreurs"
comments: "On vous a reproché vos erreurs sans vous donner les moyens de vous améliorer ? Vous avez un bras cassé en test que vous ne parvenez pas à bonifier ?"
permalink: "erreur-testeur-logiciel"
image: "/assets/img/erreur-testeur-logiciel.jpg"
categories: []
tags: ["polemique"]

---
# Et si on avait tort ? #

Bien-sûr, cela va fatalement nous arriver. L'erreur est humaine. <a id="erreur-et-defaut"></a><quote>L'erreur est une action humaine inappropriée pour le contexte qui a pour effet d'introduire un défaut ou élément non souhaité/non ATTENDU dans un livrable quel qu'il soit</quote>. Je retranscris volontairement les deux définitions d'*erreur* et de *défaut* dans le contexte humain et test.

## Comment éviter les erreurs ? ##

Donc, on aura ou on a déjà tort. Et alors ? L'essentiel est de le savoir et de prévoir le coup. Et plutôt de justement rechercher les coups en nous mettant dans notre tort (voir l'article <sub>à venir</sub> sur le champ obligatoire de gravité pour consigner un incident), autant essayer de minorer ce risque d'erreur qui sera perçu comme un signe de mauvaise qualité du test lui-même et non du produit.
<br />  
L'un des *4 objectifs du test* n'est-il pas de : <quote><a id="prevenir-defauts"></a>prévenir les défauts, c'est-à-dire empêcher qu'une erreur humaine ne les introduise dans le livrable en contribuant de manière indirecte  à l'amélioration continue du processus de production logiciel.</quote> Mais l'intervention dans le processus de création logicielle est indirecte uniquement. 

## Comment rester à sa place ? ##

Rappelez-vous un autre principe soulevé dès <a id="TMAP"></a> *TMAP* <quote>(Testing Management APproach : méthode de test de Sogeti, plus directive que l'ISTQB puisque qu'elle comporte presque des recettes de cuisine mais à laquelle l'ISTQB a emprûnté)</quote> : *débugger n'est pas tester !*. Vous trouverez [les deux processus de débuggage et gestion d'incident](./incident-differe "débugger n'est pas tester") dans l'article consacré au statut différé d'un incident. Ces processus sont assez proches, d'où la possible confusion.

## Comment éviter les reproches ? ##

Et dans un souci d'*amélioration continue*, inutile ou contre-productif d'essayer de nous culpabiliser en pointant du doigt nos erreurs (voir l'article sur [notre rapport au faux](./faux-positif "tester avec des données bidons")). Pointer le taux de rejeté et accuser nominativement tel ou tel testeur est contraire à la bonne ambiance, à l'esprit de confiance et au degré d'autonomie d'un membre d'une équipe en contexte *Agile*.

Pour rappel, il faut bien considérer la notion d'*engagement* en contexte Agile, à contre-balancer avec la notion d'*estimation*. <quote><a id="estimation-agile"></a>L'estimation est la plus juste au sens de sans marge de sécurité et avec par conséquent une reconnaissance du droit à l'erreur. Le processus de rétrospective cherchera plus tard à apprendre de nos erreurs.  Mais l'erreur sera collective, car l'estimation est collégiable.</quote> Donc, le [taux d'incident rejeté](./statut-rejete "pourquoi rejeter un incident") est à surveiller uniquement lorsqu'il dépasse un seuil de tolérance ou *critère d'acceptation* négocié. Il conviendra alors de se pencher sur les *causes racines* du phénomène mais au niveau processus et non personne par personne.

Soyons donc tolérants envers les humains qui commettent des erreurs, mais intransigeants envers la qualité logicielle. Cherchez l'erreur ou le paradoxe.