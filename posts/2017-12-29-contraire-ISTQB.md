---
layout: "post"
title: "bien interpréter les concepts ISTQB"
description: "Ne pas prendre l'ISTQB à la lettre, ou alors, gare aux dégâts. Lire entre les mots et trouver sa méthode."
mytitle: "Faire le contraire de l'ISTQB ?"
myexcerpt: "Peut-on appliquer l'ISTQB sans réfléchir aux conséquences ? Restons critiques."
mylabel: "adapter au contexte"
comments: "Vous avez vu des jeunes extrémistes se faire virer des projets ? Vous ne parvenez pas à éduquer le métier ?"
permalink: "contraire-ISTQB"
image: "/assets/img/contraire-a-ISTQB.jpg"
tags: ["polemique"]

---
# ET si je devais faire tout le contraire de l'ISTQB ?  #

Dans l'article comportant [l'index des termes cités ou définis ](./notions-test-logiciel "référentiel des notions de test informatique")je rappelais la fonction dédiée à un référentiel. Il est possible donc de faire référence en s'inscrivant en porte-à-faux et en prenant le contre pied de certains concepts.

## Que demande le métier ? ##

C'est que pris au pied de la lettre, certains concepts sont le meilleur moyen pour se faire exclure d'un projet. Prenons ces trois questions, légitimes d'un point de vue métier.

1. Alors, ça fonctionne,
2. tu as tout testé,
3. on peut mettre en prod ?

Il est possible d'apporter plusieurs types de réponses. 

## Comment se faire exclure du projet ? ##

Premier ensemble de réponse, des réponses défaitistes pour le client, en étant jusqu'au-boutiste vis-à-vis de l'interprétation de l'ISTQB. 

1. Arrête de me demander ce qui fonctionne, tu sais bien que le test ne montre que ce qui ne fonctionne pas. Notre élément de preuve est la *présence de défauts*. L'absence de défauts peut prêter à confusion : bonne qualité produit ou mauvaise qualité du test avec *illusion d'absence d'erreur* ? 
1. Et puis non, on ne peut tout tester : *test exhaustif impossible*, et quand bien-même tu ne me donnerais peut-être pas les ressources pour tout tester : *le test dépend du contexte*, du niveau de risque qui dicte l'*effort de test*, etc.
1. Quant à ce que tu attends de moi, je ne rentrerais pas dans ton petit jeu, je suis partisan de l' *indépendance du test* et ne peux être juge et parti, à toi d'utiliser l'*information pour prise de décision*.

Cette réponse est la plus proche d'une compréhension extrémiste de l'ISTQB, tournée ici sous une forme puriste et méprisante. C'est oublier un autre concept comme la génération d'un niveau de confiance.

## Comment se faire comprendre du métier ? ##

Second ensemble de réponse, des réponses constructives et pragmatiques, en étant pédagogue et en cherchant à générer un *niveau de confiance* vis-à-vis de l'application et des tests qui la couvrent.

1. **Ca fonctionne.** En tout cas le process de test a bien fonctionné. Nous avons trouvé tant d'incidents. Certains sont non résolus. Ils portent plutôt sur les aspects suivants et avec telle criticité.
2. **On a tout testé**, c'est-à-dire : les objectifs de test ont été atteints, les efforts de test consommés. Nous avons appliqué les technique de test adaptées aux risques.
3. **Pour la mise en prod**, comme définis ensemble, si les critères d'acceptation sont atteints, tu sais quoi faire. Sinon, tu as le détail des défauts recensés et peux aviser en conséquence.

## Comment éduquer progressivement le métier ? ##

Il faut donc pouvoir : 

- répondre positivement au métier (2è lot de réponses) sans le braquer mais au contraire en allant dans son sens, 
- tout en renvoyant le métier au document de *politique de test* qui commencera à lui ouvrir les yeux sur ce que peuvent être les tests (1er lot de réponses).