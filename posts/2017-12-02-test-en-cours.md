---
layout: "post"
title: "le test logiciel en cours est commencé non terminé"
description: "Un test 'en cours' n'est pas terminé : mais il continue, il est bloqué, en attente ?"
mytitle: "Que signifie réellement \"en cours\" pour un test ?"
myexcerpt: "Un test en cours est semblable à un film fleuve s'étalant sur plusieurs jours ou à une pause publicitaire avant la reprise du feuilleton ?"
mylabel: "différents types de en cours"
comments: "Avez-vous des difficultés à expliquer que des tests puissent rester en cours longtemps, ou que cela ne soit pas de votre fait ?"
permalink: "test-en-cours"
image: "/assets/img/en-cours-de-test.jpg"
categories: []
tags: ["statut de test","avancement"]

---

# Que signifie réellement "en cours" pour un test ? #

Si je pose la question, c'est que la réponse ne semble pas si simple (d'ailleurs, [à quel degré de simplicité vise-t-on ?](./simplicite-indicateurs "simplicité des indicateurs de test")). Sommes nous réellement dans un contexte *Agile* avec un tableau de type *kanban* à 3 colonnes : 

1. TODO : à faire
2. INPROGRESS : en cours (notre questionnement)
3. DONE : fait

## De quel niveau de détails avez-vous besoin ? ##

La question sous jacente est : avez-vous besoin de distinguer des sous cas ? Mon test est "en cours" parce que :

1. le test se poursuit normalement de manière ininterrompue sur plusieurs jours ;
2. le test se poursuit en pointillé, quelques actions un jour sur deux pour faire transiter les données dans un processus testé de bout en bout ;
3. le test prévu pour être ininterrompu (idéalement pour le projet, mais pas pour le produit SIC) se fait stopper net dans son élan par un incident bloquant voir plusieurs avec un effet de *masquage de défauts*.

## Quels noms de statuts utiliser ? ##

Si vous avez besoin de distinguer ces cas (voir l'article <sub>à venir</sub> : le raisonnement par le contre-exemple), il faut les isoler pour les futurs indicateurs et donc disposer des statuts adéquats permettant de pourvoir aux regroupements statistiques. Cela donne 3 statuts dont les seuls noms devraient être explicites :

1. **en cours** : se poursuit
1. **en attente** : se réalise par à coup sans pour autant connaître d'incidents bloquants,
1. **bloqué** : n'est toujours pas terminé mais est stoppé par un incident bloquant (sauf si bloqué sert à indiquer un retard dans le commencement).


Tous ces statuts sont en cours parce que les tests ont commencé. Certains (des américains dont Rex Black et les exégètes du glossaire ISTQB), utilisent le terme bloqué pour spécifier au contraire ce qui ne peut être commencé (voir l'article sur [le statut bloqué](./test-bloque "avancement du test bloque")).


