---
layout: "post"
title: "tester ou comparer un attendu à un obtenu"
description: "Le test logiciel se résume à confirmer ou infirmer la présence d'un attendu, qu'il a fallu éliciter, clarifier, justifier, formaliser..."
mytitle: "Qu'est-ce que tester ?"
myexcerpt: "Une simple question comme qu'est-ce que le test n'entraîne pas des réponses aussi simples qu'elles pourraient l'être."
mylabel: "coeur du métier"
comments: "Pouvez-vous répondre aussi simplement à un interlocuteur sur ce qui est le coeur de votre activité ?"
permalink: "test-logiciel"
image: "/assets/img/test-logiciel.jpg"
tags: ["definitions"]

---

# Qu'est-ce que le test logiciel ? #

C'est la question d'ouverture du syllabus Fondation. Mais la question est, sinon biaisée, du moins contextualisée. 

## Dans quel contexte a lieu le test logiciel ? ##

Cette question repose sur d'autres questions :

1. Qu'est-ce que la gestion de projet ?
2. Qu'est-ce que la gestion des risques ?
3. Qu'est-ce que la gestion des exigences ?
4. Qu'est-ce que la qualité ?
5. Qu'est-ce que l'amélioration continue ?
6. Qu'est-ce que l'industrialisation du test ?

Car l'ISTQB considère que **l'activité de test** s'opère dans ce contexte aux multiples dimensions. Ce qui permet très vite de situer son organisation vis-à-vis de la maîtrise des différents sujets, et de lui attribuer une note de mâturité comme en *TMMI*. Pour l'ISTQB, **le processus de test** s'inscrit donc parmi d'autres processus.

Maintenant, reposons nous la question : qu'est-ce que tester ? On a déjà dit que cela pouvait être une activité, un processus, mais plus précisément...

## A quoi cela semble servir au premier abord ? ##

Et c'est là qu'on est tenté de répondre par la manière dont s'effectue le test et  l'objectif qu'il poursuit, d'après ce qu'on a vécu. On ressort alors la définition CMMI des processus VAL et VER.

- <a id="validation-logicielle"></a><quote>La validation contrôle que les "**exigences spécifiées**" (censées ou non, avec des fautes qu'on ne peut reconnaître ou pas) sont bien implémentées. Le côté **"do the things right", bien faire les choses,** telles que précisément demandées, dans les règles de l'Art.</quote>
- <a id="verification-logicielle"></a><quote>La vérification contrôle que les "**exigences basées sur l'usage**" (explicitées ou non, spécifiées ou non, mais rendues nécessaires par l'activité métier qu'elles servent) sont bien implémentées. Le côté **"do the right things", faire les bonnes choses,** telles que s'imposant logiquement pour un bon déroulement du processus métier auquel l'application sous test est dévouée.</quote>

La question n'était :


- ni comment tester, avec ou sans documentation (car on verra que le terme de spécification n'est pas cité), 
- ni pourquoi tester, pour s'assurer que ce qui est écrit est réalisé ou que ce qui est nécessaire est produit. 

La question était et reste la suivante :

## Qu'est-ce que tester ? ##

<a id="tester"></a><quote>Tester, c'est COMPARER un ATTENDU à un OBTENU. Point final. Ce qui se résume, en test unitaire, à : AssertEquals(expected,actual);</quote>. Voir l'article <sub>à venir</sub> sur les tests unitaires.<br /> 
Mais je continue quand même en citant mes sources : la définition de tester est contenue dans la définition de *l'oracle de test* que voici retranscrite à ma sauce (un référentiel, cela s'approprie).

<quote><a id="oracle-de-test"></a>L'oracle de test se définit surtout par ce à quoi il sert, c'est-à-dire à déterminer l'ATTENDU : qui plus tard sera à COMPARER à l'OBTENU (élargissement de la définition au test). Et pour déterminer l'attendu, "tous les moyens sont bons", ou presque.</quote> Sont cités : 

1. manuel utilisateur (il faut comprendre tout type de documentation), 
1. système existant, 
1. individu lui-même.



## Rien qui vous choque ? ##

Et c'est là que cela fait réagir. Les éléments qui constituent le "source utilisée pour" de la définition font réfléchir.

1. N'est utilisé ni le terme assez large et neutre de documentaion logicielle, ni le terme habituel précis de spécification. Il ne faut pas s'en formaliser, ce n'est qu'un exemple, et le terme de spécification sera repris dans la définition de l'anomalie auquel un article <sub>à venir</sub> est consacré. Notons juste, pour lot de consolation, que le terme employé est orienté métier : "utilisateur".
2. Prendre l'existant lorsqu'il existe, en tant que "point de référence" d'après la définition, peut sembler surprenant. Mais la citation l'indique, ce n'est qu'une base, et c'est vrai qu'il faudrait mieux éviter de faire pire qu'avant si ce n'est pas voulu.
3. Peut-être le plus choquant de tous, surtout pour tous ceux qui n'osent penser par eux-même : vous pouvez/devez embarquer votre propre conscience professionnelle, votre propre étalon maître de la qualité logicielle. Il s'agit là de votre propre retour d'expérience qui doit bénificier à l'amélioration continue de la qualité produit. <br /> Cela doit bien-sûr ce faire dans un cadre défini où les limites sont posées, avec les droits et devoirs de chacun. Si vous êtes extrémistes ou en désaccord sur le niveau de qualité attendu ou à consigner, [vous risquez de voir vos incidents rejetés](./statut-rejete "s'accorder sur les conditions du rejet d'un incident"). <br /> Comme en Agile où une définition stricte du *"done"* ou terminé s'impose, sûrement faut-il définir explicitement le *critère d'acceptation* d'un *incident*, et par là même la vocation d'un *gestionnaire d'incident*, voir l'article <sub>à venir</sub> sur le gestionnaire d'incident.

## Pas d'autres notions ? ##

Maintenant, vous savez que j'ai curieusement cité une autre notion que le test pour expliciter le test. Car le test, du moins en français, c'est aussi autre chose :

1. "test" en Anglais : 1 ou N *cas de test*.
2. "testing" en Anglais : *processus de test*.

Mais cela ne change rien à ce que fait tout test : comparer un attendu à un obtenu. D'où l'on peut logiquement envisager deux activités qui s'articulent autour de ce noyau central, même si ce n'est pas le processus de test officiel :

- constituer en amont cet attendu et les moyens de le contrôler,
- consigner en aval cet obtenu et en tirer les conséquences en cas de divergence.




