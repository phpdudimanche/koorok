---
layout: "post"
title: "utiliser un outil de test, pour quel besoin, comment"
description: "Les outils de test doivent supporter et non contrarier les activités de test. Le respect des besoins et bonnes pratiques devrait être primordial.."
mytitle: "De quel outil a-t-on besoin ?"
myexcerpt: "Pour être utile, l'outillage doit correspondre au besoin, à la réalité terrain...."
mylabel: "utile ou superflu ?"
comments: "Vous vous êtes aussi heurtés à des fonctionnalités inutiles, voire dangereuses... Ajoutez vos remarques à la liste."
permalink: "besoin-en-outillage"
image: "/assets/img/besoin-outil-test.jpg"
categories: []
tags: ["outils"]

---
# Que voulez-vous, au juste ?

Il peut être assez facile de perdre de vue son besoin initial et de répondre à l'appel des sirènes. Dans notre société de consommation, les fournisseurs ont développé un don certain pour faire émerger de nouveaux besoins (voir l'article sur [ce qu'on peut trouver  à redire à une solution tout en un](/outil-test-tout-en-un "suite logicielle")). 

## Comment rester au plus juste de ses besoins et avoir le "juste ce qu'il faut" ?

 J'ai déjà observé des applications s'enrichir et se complexifier au fil du temps, amenant à ne plus correspondre au besoin et à l'ergonomie basique. 

Je fais par exemple référence aux outils de mesure d'audience avec des modules purement et simplement non enlevables/masquables et devenus par trop désagréables pour des patrons de TPE, non-addictes aux usines à gaz. Et quand on voit l'évolution de GoogleAnalytics...

## Comment tenir bon contre les tentations ?

Gardez la têtre froide et cernez vos besoins avant de vous faire pervertir.  C'est la démarche que nous vous proposons. Brique par brique nous regarderons ce qu'il vous faut pour bâtir votre maison (voir ici [ce lotissement par brique](/modules-test-logiciel "isoler chaque module de test")).

Nous citerons ici les écueils les plus évidents.

- Dans la partie exécution d'un **référentiel de test**, avez-vous réellement besoin de piloter les tests unitaires ou IHM (voir l'article  <sub>à venir</sub> dédié aux interfaces). Ne sont-ils pas pour vous ou votre organisation des tests automatiques lancés de manière automatique par lot, au lieu d'un test unique lancé manuellement ? Cette question peut revenir pour l'usage d'un outil ATTD de type Fitnesse (voir article <sub>à venir</sub>) qui lance unitairement et manuellement une spécificaion exécutable et voit son résultat dans la page de wiki.
- Souhaitez vous pouvoir exécuter rapidement et de manière unitaire un test parce qu'il répond à un questionnement urgent, ou souhaitez vous être systématiquement enfermé dans une mécanique de création d'éléments : release/campagne/suite de test ?
- Pensez-vous que la statistique de nombre de cas de test par testeur et par jour soit une bonne chose lorsque vous avez des typologies de cas de test différents et que vos testeurs se rebellent à l'idée de se voir imposer des quotas ? (voir l'article <sub>à venir</sub> sur les indicateurs)
- Est-ce une bonne pratique que ce référentiel de test englobant un bug-tracker mais ne le faisant intervenir qu'à la partie exécution des tests (je pense à testLink) ?
- Voulez-vous réellement vous voir imposer en champ obligatoire à la consignation d'un ticket dans un **gestionnaire d'incident** : le caractère reproductible d'un événement sur une procédure de test qui met 5 jours à aboutir ?

## Comment cerner ses besoins ?
Bien-sûr, la question la plus difficile est de connaître ses besoins. Connais toi toi même, disait le philosophe. Faute de cette connaissance et de ce respect strict des besoins, l'outil devient vite inapproprié.
Or, ne vaut-il mieux pas aucun outil qu'un outil inapproprié ou mal utilisé ?

Vigilance, donc. C'est d'autant plus facile de sauter à pieds joints dans les pièges qu'il suffit de se laisser faire (voir [tendance au tout en un](/outil-test-tout-en-un "solution complète"))