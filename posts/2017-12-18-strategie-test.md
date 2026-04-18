---
layout: "post"
title: "la stratégie de test n'est pas le plan de test"
description: "L'approche de test est l'instanciation de la stratégie de test pour un projet. La stratégie de test concerne la tactique de test à employer pour tester telle problématique et application au sein de l'organisation."
mytitle: "Le test est-il jetable ?"
myexcerpt: "Faute de stratégie de test véritable au niveau organisation, l'approche de test en mode projet est jetable."
mylabel: "stratégie vs approche"
comments: "Vous aussi, vous devez appeler stratégie ce qui n'en est pas une ? Vous en souffrez et recherchez un juste milieu ?"
permalink: "strategie-test"
image: "/assets/img/strategie-de-test.png"
categories: []
tags: [polemique]

---
# Le test est-il jetable ? #

Je pose cette question en réaction à un comportement suffisament fréquent pour qu'il soit éclairant. Même des certifiés ISTQB emploient le terme de *stratégie de test* pour parler d'*approche de test*. Qu'est-ce que cela révèle ? 

## Le test en mode projet ou mode service ? ##

A mon sens, mais cela n'engage que moi, cela révèle le caractère limité de la portée du test. Le test s'inscrit dans le cadre très borné du projet, avec sa fameuse date de fin (sauf en *Agile* à appliquer strictement le proverbe : "tant que je gagne, je joue ; tant que je crée de la valeur, je développe").
<br />  
C'est donc le *mode projet* qui est jetable, à l'opposé du *mode service*. La question suivante est alors : **à qui rendent service vos activités de test** : au projet qui ne fait que passer, ou au SI qui devra maintenir une nouvelle application sur la durée ?
<br />  
On peut bien-sûr toujours prolonger le projet en jouant sur les mots, en créant un autre projet en phase de run avec une date de péremption lointaine mais connue du DSI qui envisage le retrait de l'application à telle date. Mais vous voyez certainement ce que je veux dire...

## L'approche de test sans la stratégie de test ? ##

L'absence parfois de <a id="strategie-test"></a><quote>capitalisation sur les tests au niveau d'un programme ou module métier</quote> est significative (intention de la stratégie de test, même si, on me le faisait remarquer, [la définition de la stratégie de test "l'autorise" à porter sur projet unique](http://glossary.istqb.org/search/test%20strategy "statégie de test mono projet")). Il arrive qu'il n'y ait pas de <a id="approche-test"></a><quote>"stratégie de test" réutilisable et instanciable avec adaptation pour tout nouveau projet</quote> (produisant l'approche de test).
<br />  
Pour prendre une image POO : il y a directement existence de l'objet sans instancation de sa classe : impossible ! On reste enfermé dans le projet sans capitaliser à un niveau plus haut. Seule existe alors *l'approche de test* qui est insérée dans *le plan de test*. Et l'organisation-projet (oxymore ?) la nomme stratégie de test, inconsciemment pour se cacher que la stratégie de test n'existe pas ? Si le mode projet oblige à tout centrer et lotir sur le projet, effectivement, difficile de justifier une véritable stratégie de test.   

## Comment revendiquer l'amélioration continue ? ##

Mais impossible alors d'ancrer l'activité de test dans une politique d'*amélioration continue* bénéficiable au plus grand nombre : aux futurs projets qui traverseront les mêmes problématiques déjà traitées par votre projet concernant ce pan métier.
<br />  
On ne peut cependant pas nous reprocher un tel comportement. Tout dépend de ce dont nous avons en charge : un portefeuille projet ou un portefeuille d'applicatifs ?
<br />  
Pour poursuivre le débat sur le test jetable, un autre article <sub>à venir</sub> continuera à répondre par l'affirmative avec la maintenance des cas de test.

