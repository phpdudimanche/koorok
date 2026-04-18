---
layout: "post"
title: "tests fumigatoires automatiques"
description: "Restreindre les tests automatiques à un périmètre réduit piloté par les risques. Assurer ainsi la continuité de l'activité en garantissant le maintien du processus."
mytitle: "Qu'est-ce que tu fumes ?"
myexcerpt: "Attention à la dépendance ! Qui peut le plus n'a-t-il pas du mal à faire le moins ? Dans la course à l'automatisation : comment résister à tout scripter et à tout exécuter  ?"
mylabel: "isoler les tests fumigatoires"
comments: "L'entité test ou une autre gère-t-elle les risques ? Votre organisation accepte-elle le principe de réduire le périmètre des tests à l'occasion des tests fumigatoires ?"
permalink: "tests-fumigatoires-ou-smoke-tests"
image: "/assets/img/tests-fumigatoires.jpg"
categories: []
tags: ["polemique"]

---

# Comment faire des tests fumigatoires ? #

Le point de départ de la question est un constat qui peut faire mal : comment "s'obliger" à faire de tests fumigatoires ? Parce qu'il est bien plus simple de ne pas faire de tests fumigatoires ou *smoke tests*. Dans pareil cas, on ne se pose alors pas de question tout court. On ne se pose pas les questions suivantes :

- Comment faire des tests pilotés par les risques ?
- Comment réaliser le voeu XP d'un build en 10 minutes ?

## Comment sécuriser le processus sous test ? ##

Dans la famille des *tests de régression* (voir l'article <sub>à venir</sub> sur le débat régression/non régression), les tests fumigatoires ont une place à part, bien identifiée ! Ces tests permettent de : <a id="tests-fumigatoires"></a><quote>tester à la grosse maille les fonctions vitales d'un processus qui n'ont pas de solutions de contournement</quote>. Ces tests sont donc orientés risque.

En l'absence de tels tests, la question serait donc : y-a-t-il officiellement une *gestion des risques* ? Ce qui ouvre le débat <sub>à venir</sub> sur le champ d'action des testeurs.

## Comment déployer rapidement ? ##

Lorsque les tests sont outillés et que le projet est dans un environnment d'*intégration continue*, difficile pour l'esprit humain de "se restreindre à une gestion des risques efficace". Difficile en effet de se tenir les propos suivant **"qui peut le plus pourrait s'astreindre au moins"**. Et pourtant...

Comment déployer rapidement en exécutant la totalité des tests ? 
Comment de tels tests pourraient tenir en moins d'une heure ? Comment ne pas encourir le risque d'avoir des erreurs d'exécution ou des [faux positifs](./faux-positif "faux échecs") pour des tests tellement peu importants qu'ils sont non maintenus, ou/et obsolètes et qu'on ne s'est pas donné la peine d'enlever. 
Le risque est  le suivant : **en confondant quantité et qualité, et en voulant bien faire, on fait mal**.

## Comment techniquement réaliser l'opération ? ##

Techniquement, l'effort n'est pas si grand. Exemple Xunit :

1. ajouter une annotation pour identifier chaque test ciblé @fumigatoire
2. cibler l'exécution sur ce tag

Et ensuite, si vous étiez un peu joueur ou pressé par le temps, vous pourriez mettre en place la règle de décision suivante pour les *tests de régression* avec l'algorithme suivant en pseudo-code pour examiner le rapport d'exécution XML de type Junit :

<pre>
IF exists fumigatoire==KO
THEN alerte a regarder
ELSEIF count KO > $seuil
THEN alerte a regarder
DEFAULT
THEN alerte a ignorer, commiter
ENDIF
</pre>

Cela permet de n'attirer l'attention que sur deux cas :

1. ce qui est vraiment important en terme de risque,
1. ou ce qui est vraiment important en terme d'effort de correction. 

En dehors de ces deux cas, le reste pourra facilement être corrigé par hotfix et le commit peut se faire en automatique.

## Comment humainement réaliser l'opération ? ##

La véritable difficulté est humaine ou organisationnelle. On en revient à la question déjà posée, qui peut être creusée :

- Y-a-t-il une gestion des risques véritable ?
- La gestion des risques est-elle assumée, partagée par tous et communiquée à tous ?
- Qui valide le choix des tests fumigatoires, ou se font-ils sur la base d'une détection des risques préalablement validée ?
- Etc.

Du moment que la règle de décision pour effectuer la sélection des *tests fumigatoires* est claire, son application l'est aussi.