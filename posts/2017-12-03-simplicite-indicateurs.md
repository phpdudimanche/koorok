---
layout: "post"
title: "simplicité du suivi de l'avancement du test"
description: "Suivre l'activité de test devrait être simple : pour être facile à faire, évident à comprendre, et j'en passe."
mytitle: "Si on essayait de suivre \"simplement\" le test ?"
myexcerpt: "Et si les indicateurs devenaient aussi évidents et ancrés dans les esprits que l'idée pourtant fausse : tester c'est exécuter un test IHM ?"
mylabel: "viser la simplicite"
comments: "Jugez-vous vos indicateurs incompréhensibles, trop complexes et trop difficiles à générer ?"
permalink: "simplicite-indicateurs"
image: "/assets/img/simplicite-du-test.png"
categories: []
tags: ["statut de test","avancement"]

---
# Jusqu'à quel point peut-on rester simple ? #

Avec la "légitimité" (article <sub>à venir</sub>) qui nous apporte reconnaissance et confiance de la part des commanditaires, la simplicité *KISS* peut être un véritable atout. Que gagne-t-on à complexifier (même si le complexe peut être redécomposé en éléments simples) ? Pour rester ou tâcher d'être simple, voici les minima syndicaux du test.

## Statut d'avancement du test ##

1. Non commencé.
2. [Commencé](./test-en-cours "test en cours de progression").
3. Terminé.

## Statut de découverte de la qualité ##

1. [Incident](./test-KO "test avec incident").
2. Pas d'incident.

## Statut des incidents ##

1. Ouvert.
2. Fermé.

## Le juste niveau de détails ##

Bien-sûr, tout dépend du **CQFD(Ce Qu'il Faut Démontrer)** : voir l'article <sub>à venir</sub> sur les indicateurs. Ce qui amène à définir une notion *LEAN* inexistante (et pour cause si le Lean vise à la qualité totale du zéro défaut) : "la juste qualité" (cf le juste à temps) qui se définirait alors en opposition avec la *sur-qualité* et la *sur-production*. A quoi bon "vouloir faire bien", et en plus à la main, consommateur de temps et générateur d'erreur, en produisant un rapport trop riche, difficilement lisible, exploitable, utile... !

## Question - réaction ##

Ces 3 rapports répondent à des questions "légitimes" et font entrevoir des plans d'action évidents.

Question // Réponse // Réaction

1. Les tests avancent ? // OUI, 2 et 3 / NON, 1 // Et si cela n'avance pas comme prévu...
2. Il y a des incidents ? // OUI, 1 / NON, 2 // Et si il y en a trop ou pas assez...
3. Il reste encore des incidents ? // OUI, 1 / NON, 2 // Et si il y en a trop d'ouverts...

## Complexité cachée ##

Derrière cette apparente simplicité se cache une complexité, peut-être ignorée si l'implicite est partagé par tous.

1. Liée au test, la notion d'avancement est ambigüe. Voir article <sub>à venir</sub> sur l' interprétation du terme avancement.
2. La question de l'existence d'incidents peut faire l'objet de plusieurs rapports. Quels incidents et où ? Par exemple : que des incidents à minimum majeurs et consolidés sur des conditions de test par nature surveillées car à risque ou à valeur ajoutée.
3. La question du "méta statut" d'incident sous-entend s'intéresser aux incidents ouverts. Mais ces incidents sont toute criticité confondue ou pas, et toute cause égale à sa voisine ou pas (débat d'un incident de nature système qu'il ne faut pas imputer au compte d'incident produit imputable pour "faute" à l'éditeur).

## La définition des limites ##

On pourrait considérer qu'au delà de cette vue, on commence déjà à entrer dans la complexité. Il faut alors prévoir un solide argumentaire pour justifier et interpréter les éléments ajoutés aux **statuts discutables et alors souvent discutés**. Ces discutateurs devant l'éternel (merci Elie Simoun) existent, et j'en fais parti. Ce sont aussi bien des personnes de mauvaise foi, des gens obtus, des personnalités lentes à comprendre ou avec leur propre raisonnement, que des testeurs à l'esprit critique exacerbé les poussant à **critiquer/questionner le process de test lui même**.



