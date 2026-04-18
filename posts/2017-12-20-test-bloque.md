---
layout: "post"
title: "un test est dit bloqué lorsqu'on ne peut commencer ou continuer à tester"
description: "Les contrôles sont impossibles à effectuer sur ce test ? Le test est bloqué ou non testable."
mytitle: "Qui bloque sur le statut bloqué du test ?"
myexcerpt: "Lorsque l'on souhaite faire passer des messages, encore faut-il s'assurer qu'ils soient bien compris. Un test bloqué peut évoquer différentes choses."
mylabel: "bloqué : au début, au muilieu..."
comments: "Vous faîtes aussi un blocage sur bloqué ? Ou au contraire vous trouvez que la discussion est trop capilotractée ?"
permalink: "test-bloque"
image: "/assets/img/test-bloque.jpg"
categories: []
tags: ["statut de test","avancement"]

---
# Mais qu'est-ce qui bloque dans le statut "bloqué" ? #

Bienheureux les simples d'esprit qui se posent moins de questions et ne se rendent même pas compte que certaines notions prêtent à discussion.

## Bloqué prête à confusion ##

Bloqué gêne sur un point essentiel :

- Bloqué sonne comme un cas de test avec incident, lequel incident a un statut bloquant : il est donc possible de comprendre "KO bloquant", voir l'article consacré aux [différents types de KO](./test-KO "KO ou test avec incident"),
- Or bloqué semble s'interprétrer plutôt comme **empêche l'attendu d'être comparé à l'obtenu, faute de pouvoir obtenir cet obtenu**.

Peut-être la confusion n'est-elle pas permise en anglais, mais en français, elle fait son petit effet. Or, le doute ne correspond pas à la clarté que devrait revêtir un statut, voir l'article <sub>à venir</sub> sur les caractéristiques d'un indicateur.

## Si l'on voulait être clair ##

Et puis si l'on souhaite vraiment être limpide, <quote>tout événement survenant durant les tests et qui pose question et demande investigation</quote>, bref, un *incident*, pourrait catégoriser d'office le test en "KO". Cela cadre avec la vision simpliste des indicateurs proposée dans l'article des [minima sociaux du suivi de test](./simplicite-indicateurs "un simple suivi de test"). Cela entrerait ainsi parfaitement en opposition avec "OK" qui résulterait d'une absence d'incident ou d'une autre règle de décision discutée en un article <sub>à venir</sub> consacré aux critères cités dans l'ISTQB.

## Alors, on l'utilise ou pas, ce statut ? ##

Si l'on souhaite utiliser "bloqué", ou toute autre appellation qui n'est après-tout que convention et nous importe peu, c'est que l'on souhaite apporter une distinction par l'usage de ce statut plutôt qu'un autre. De son index, *l'indicateur* pointe du doigt ce qu'il veut désigner comme sujet de son étude. 

## Que permettrait donc l'usage d'un tel statut ? ##

Un peu de surf et de lecture nous apprend qu'isoler un tel statut permet de réaliser les actions suivantes.

- Arrêter le compteur de la charge (travail interrompu). Mais cela ne peut pas arrêter le compteur du délai, qui tourne tout le temps, le temps passe et ne peut être consommé qu'à vitesse constante.
- Préciser que le test n'a pu être vérifié, validé ou invalidé.

Si vous avez de tels besoins, effectivement avoir recours à un statut de ce type peut être utile, sauf si un statut plus générique avec le même effet couvre déjà ce cas.

## Et les autres, que font-ils ? ##

Le moins que l'on puisse dire, c'est que les pratiques sont assez disparates en la matière. 

- L'ISTQB pourrait laisser supposer que [c'est le critère d'entrée en début d'exécution de test qui n'est pas atteint](http://glossary.istqb.org/search/blocked "bloqué par le critère d'entrée").
- Un outil IBM ajoute [le distinguo entre "Blocked" en début d'exécution et "Partially Blocked" en cours d'exécution](https://jazz.net/help-dev/clm/index.jsp?topic=%2Fcom.ibm.rational.test.qm.doc%2Ftopics%2Fc_execution_verdicts.html "test partiellement bloqué") si on ne peut atteindre le "Completed" ou "Executed"
- Les raisons du caractère "non Excécutable" ou "Non Testable" peuvent porter non seulement sur le système, mais également sur le projet : [bloqué pour cause de testeur en vacances](http://help.runtestrun.com/kb/using-test-run/what-are-the-differences-between-various-test-case-statuses "test bloqué pour raison de projet"), comme un peu le caractère "Suspendu" que l'on peut aussi trouver.

Bref, tous les goûts sont dans la nature. Et vous, quelle est votre position sur la question ? 

## Et pour évacuer la question ? ##

Ou alors, vous appliquez cette autre version :   

- "Non testable" pour bloqué dès le début. 
- "Bloqué" pour bloqué ensuite.

De toute façon, tout cela n'est que question de convention. Du moment que toutes les parties prenantes s'y retrouvent, faîtes strictement ce que vous voulez. Aucun conseil à donner. 

Je m'étonne juste de la subtilité de certains termes qui peuvent prêter à confusion. Et comme je le disais au début, si vous ne vous en rendez même pas compte, peut-être tant mieux pour vous.