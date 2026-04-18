---
layout: "post"
title: "l'incident pour ITIL et l'incident pour l'ISTQB"
description: "Lorsque plusieurs référentiels cohabitent au sein d'une équipe, comment établir un consensus ? Le propre d'un référentiel étant de parvenir à se comprendre, parler plusieurs langues ne facilite pas la tâche !"
mytitle: "ISTQB VS ITIL ?"
myexcerpt: "Lorsque deux univers se rencontrent, comment se comprennent-ils ?"
mylabel: "le choix des mots"
comments: "Comment gérez-vous les arbitrages/écarts de langage lorsque deux référentiels ont cours au sein d'une même équipe ?"
permalink: "ISTQB-compatible-ITIL"
image: "/assets/img/ISTQB-VS-ITIL.jpg"
categories: []
tags: ["definitions"]

---
# L'ISTQB est-il soluble dans ITIL ? #

Ainsi posée, bien sûr que la question attend NON comme réponse. C'est que ce sont deux différentiels, potentiellement différents. Chacun d'eux peut offrir un paradigme complet, une vision du monde entière, auto-suffisante. Difficile d'être polythéiste dans des univers monothéistes.

Combiner ces deux référentiels de "bonnes pratiques" n'est pas prévu. C'est pourtant la réalité du monde du travail, lorsque des systèmes de pensée différents se rencontrent.

## ISTQB et ITIL sont-ils sur les mêmes périmètres ? ##

J'ai un confrère ITIL (plus d'1 million de certifiés ?) qui ne tolère pas la vision du monde ISTQB ([535 000 certifié ISTQB](https://www.istqb.org/about-as/facts-figures.html "certification ISTQB")). Faisons un parallèle entre ces deux référentiels de bonne pratique.

Tout d'abord, ils ne sont pas sur le même périmètre. 

- ISTQB <a id="ISTQB"></a><quote>(International Software Testing Qualifications Board) s'intéresse au test, aux problématiques qualité de toute la chaîne de fabrication logicielle</quote> 
- ITIL <a id="ITIL"></a><quote>(Information Technology Infrastructure Library) s'intéresse à l'infrastructure, à l'exploitation des plateformes principalement en production</quote>.

## Qu'est-ce que l'incident ? ##

Le terme qui pose évidemment le plus de problème à l'aficionados ITIL lorsque je l'utilise est incident. J'avais déjà évoqué les litiges qu'il peut y avoir autour de [ce terme d'incident](./anomalie-normale#incident "incident approuve ou non") lorsque cette appellation nous est refusée.

Le workflow ITIL est :

- **Incident** égale dysfonctionnement d'une infrastructure en service. Ce qui se rapproche le plus en ISTQB est **défaillance** : <a id="defaillance"></a><quote>dysfonctionnment visible d'une application en exécution.</quote>
- **Problème** est la catégorisation de cet incident, ou la classe dont l'incident est l'instanciation ou l'objet. Je tourne autour de la définition exprès. Mais disons que l'incident est l'itération d'un problème, et que ce problème est reporté dans l'outil de support de résolution d'incident pour qu'à chaque itération le support technique puisse ressortir la même procédure de résolution d'incident. En ISTQB, le terme qui se rapproche le plus du problème ITIL est **cause racine** du défaut : <a id="cause-racine"></a><quote>catégorisation de haut niveau pour l'introduction d'un défaut qui permet de relier plusieurs incidents entre eux et de trouver un effet de levier pour l'amélioration des processus</quote>.

Le workflow ISTQB schématisé est :

- **Incident** : ticket au statut ouvert.
- **Anomalie** : ticket au statut confirmé.

## Qu'est-ce que le bug ? ##

Le collègue me dit que je n'ai qu'à utiliser le terme de bug, pour être neutre et ne pas faire entorse aux principes ITIL. Je peux en effet l'utiliser, mais alors cela heurte le principe de précaution abordé dans l'ISTQB.

- **Bug** est un **défaut**, <a id="bug"></a><quote>élément qui pose problème dans un livrable, quel qu'il soit, étant considéré comme une imperfection</quote>. 

Il y a alors un conflit ouvert entre les 2 référentiels.

- Qualifier un événement de bug est prématuré pour l'ISTQB alors qu'on ignore encore si ce n'est pas l'observateur qui a un bug et commet une erreur dans son observation.
- Qualifier un événement d'incident est sacrilège pour ITIL lorsq'il n'y a pas dysfonctionnement d'un système et qu'il s'agit juste d'un élément choquant à la lecture d'une doc par exemple.

## Parle-t-on de la même chose ? ##

On en revient une fois de plus au périmètre :

- ITIL porte sur des problématiques d'exécution.
- ISTQB englobe toutes les problématiques de qualité logiciel, y compris en mode **statique**, <a id="test-statique"></a><quote>sans exécution de l'application sur un système</quote>.

Un terme neutre synonyme d'incident pour les deux référentiels serait événement. On soumet alors, (ni un incident, ni un bug, ni une anomalie), mais un rapport d'étonnement, dans ce fameux outil au nom également tendancieux pour un pratiquant ITIL : le gestionnaire d'incident, voir <sub>article à venir</sub>. 
