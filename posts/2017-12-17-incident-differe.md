---
layout: "post"
title: "différer un incident : pourquoi, comment"
description: "Les incidents jugés insuffisamment prioritaires peuvent être remis à des versions ultérieures (ou aux calendes greques ?). On les note alors comme différés."
mytitle: "Différer un incident : pour quoi faire ?"
myexcerpt: "Les incidents n'ont pas vocation ou obligation à être tous corrigés. On peut égalemnt remettre au lendemain ce qui ne peut être fait sur la prochaine version logicielle."
mylabel: "reporter ou rejeter ?"
comments: "Les incidents différés vous ont aussi posé problème ? Vous n'utilisez jamais \"différé\" ? Echangons ensemble autour de nos pratiques."
permalink: "incident-differe"
image: "/assets/img/incident-differe.jpg"
categories: []
tags: ["statut de test"]

---
# Le statut fermé d'un incident est-il si simple ? #
Loin de moi toujours l'idée de complexifier. Au contraire, je serais partisan de [la simplicité, dans la mesure du possible](./simplicite-indicateurs "indicateurs evocateurs") : c'est-à-dire de l'éducation des parties prenantes à cette *politique de test*. Je vois toujours les sources potentielles de problème derrière d'apparentes simplicités qui ne présenteront pas de problème, jusqu'au jour où... Voir l'article <sub>à venir</sub> : que faire quand.

## Que faire des incidents différés ? ##
Si les incidents différés restent ouverts et qu'ils ne sont pas exclus des compteurs (voir articles <sub>à venir</sub> sur l'outillage), ils viennent greffer vos comptes, alors que le test n'a pas d'action sur la décision de correction.  
 
Rappel sur la séparation des pouvoirs, évoquée dans un des *4 objectifs de test ISTQB*. <a id="objectif-information"></a><quote>Le test donne de l'information potentiellement utile à prise de décision</quote> : voir [la page 13 du syllabus ISTQB FONDATION](https://www.istqb.org/downloads/send/2-foundation-level-documents/3-foundation-level-syllabus-2011.html "quatre objectifs de test").

## Où placer le statut "différé" ? ##
- L'incident différé est un incident "ouvert" au sens où il n'a pas été résolu. 
- L'incident différé est un incident "fermé" au sens où il a été traité. Toute la subtilité est peut-être dans ce mot "traité. 

## Rappel sur le processus de gestion des incidents ##
Pour éclairer cet état d'incident "traité", voici un rappel ISTQB de <a id="debugger-vs-tester"></a>la différence entre les processus de *débuggage* et de *gestion des incidents*.

<table class="explain">
<thead><tr><td>Etapes</td><td>Incident</td><td>Bug</td></tr></thead>
<tfoot><tr><td>Etapes</td><td>Incident</td><td>Bug</td></tr></tfoot>
<tbody>
<tr><td>1</td><td colspan="2" style="text-align:center">Identifier</td></tr>
<tr><td>2</td><td colspan="2" style="text-align:center">Analyser</td></tr>
<tr><td>3</td><td>Traiter</td><td>Corriger</td></tr>
</tbody></table>

## Mais ce n'est jamais fini ##

Si la mission des tests concernant les incidents est de veiller à ce que le processus soit achevé, la mission est terminée. Un incident différé est en méta statut fermé, et bien-sûr retiré du rapport courant pour éviter de le polluer.

Bien-sûr, fermé peut prêter à confusion. C'est la bouche à commentaire des acteurs qui est fermée. On a dit le principal au sujet de cet indident. L'incident a été arbitré, avec **décision de le différer, donc de le fermer pour l'instant**. L'idée normalement est de le rouvrir par la suite si... on a assez de temps ou un creux d'activité.   

Dans certaines circonstances, vu que le temps a plutôt tendance à se réduire comme peau de chagrin, et que la qualité totale du *zéro défaut* n'est pas visée, cette *dette technique* est plutôt acquise pour toujours et il serait plus clair de mettre directement "rejeté" plutôt que "différé". Mais se poserait alors un autre problème. [Voir l'article sur le statut rejeté](./statut-rejete "rejeter un incident").