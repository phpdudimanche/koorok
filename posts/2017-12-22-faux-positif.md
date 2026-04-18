---
layout: "post"
title: "rapport au faux en test logiciel : données, procédures"
description: "Fictif, le jeu de donnée. Approximative, la spécification. Irréaliste, la procédure métier modélisée. Question de point de vue."
mytitle: "Et si tout était faux ?"
myexcerpt: "Jeux de données fictifs, procédures métiers enjolivées, vision métier faussée."
mylabel: "faire avec"
comments: "Votre test est jugé trop éloigné de la réalité ? Le métier n'est pas sur la même longueur d'onde que vous ?"
permalink: "faux-positif"
image: "/assets/img/faux-positif.jpg"
categories: []
tags: ["polemique"]

---
# Nos tests sont faux, pas faussés ? #

D'une certaine manière, tout est faux. "La carte n'est pas le territoire", disait Saussure. Nous travaillons sur des représentations/modélisations du réel. Le meilleur ami de l'Homme, notre chien daltonien (j'avais écrit : dalmatien), ne perçoit pas le Monde de la même façon que nous. Et le test, dans tout cela ?

## Mais ton jeu de données est fictif ! ##

Eh bien parfois, le métier ne comprend pas que nous travaillions sur **des données "fausses"** ou bidons, des fakes (voir un article <sub>à venir</sub> sur les outils de génération de données). Le métier veut que nous travaillions sur des données réelles, et même que nous fassions des tests en prod (voir article <sub>à venir</sub> sur tester la prod). Besoin d'évangélisation et d'explication de la part du représentant de l'équipe de test. Qu'est-ce que le vrai, qu'est-ce que la faux, qu'est-ce que nous testons, qu'est-ce qui n'est pas faussé dans les résultats ?

## Mais les données réelles sont bizarres ! ##

Après, il sera possible, voire souhaitable à un moment de jouer (appelation jeu de test oblige) avec les données réelles. Mais ce sera sûrement pour plusieurs raisons.

- Faire plaisir au métier, ou solution de simplicité pour le mettre de notre côté et du coup nous soulager, ou lui générer un niveau de confiance (abusif si on le laisse penser certaines **choses fausses** vis-à-vis du test).
- Tester des données réelles, imposées par le métier ou choisies de manière aléatoires : et cela permettra de faire un sondage sur la qualité des données (non conformes à la documentation, au modèle de table, bref : on nous a raconté des **choses fausses** !).
- Tester une volumétrie réelle, ou pour des tests de performance rejouer de manière automatique des scénarios de la prod d'hier pour éprouver la préprod, chasser des **idées fausses** véhiculées par des exigences non atteignables ou des ragots dangereux et vérifier la réalité des faits.

## Du faux plus vrai que nature ##

Il n'en demeure pas moins que nous travaillons sur du faux. Pourtant, en sortie nous pouvons parvenir à produire plus vrai que nature, c'est-à-dire plus vrai qu'avant. "HomoTesting lave plus blanc que blanc".
<br />  
Exemple d'une procédure métier théorique jamais appliquée, d'une modélisation BPM fausse s'appuyant sur des spécifications utopiques, et que viendrait contrecarrer la réalité de nos procédures de test qui seront même dérivées plus tard en manuel d'utilisation.
<br />  
La vision que nous apportons sur l'application est concrète et éprouvée par la pratique, certes orientée test et pas toujours métier, mais avec une vue critique plus aiguisée parfois que le métier. Comment le métier, englué dans ses habitudes de travail, déçu par chaque nouvelle application qui rabaisse ses ambitions, obligé au pragmatisme par la force des circonstances, pourrait-il trouver le temps de lever la tête, de regarder et de s'écrier... "Mais ce n'est pas vrai !" 

## Le regard aiguisé du testeur ##

Nous, testeurs, nous verrons certains choses qu'ils (<a id="E-T"></a><quote>**les E.T. Extra Testeurs**, les parties prenantes qui nous prennent parfois pour des extra-terrestres</quote>) ne verront pas. Parce que tester est un métier, dit l'ISTQB. Mais aussi et surtout, parce que comme toute chose, tester est aussi question de perspective (sans parler de la maîtrise des méthodes, techniques et outils). 

## Faux positifs ou faux échecs ##

Pour illustrer ces propos, je finirai sur un dernier exemple de faux et de variation de perspective : l'usage d'un double référentiel pour <a id="faux-positif"></a>**exposer les faux posififs comme faux échecs, et les faux négatifs comme faux succès**. 

<table>
<thead><tr><td>Constat</td><td>vue résultat redressé</td><td>vue résultat original</td><td>action </td></tr></thead>
<tfoot><tr><td>Constat</td><td>vue résultat redressé</td><td>vue résultat original</td><td>action </td></tr></tfoot>
<tbody>
<tr><td>c'est un faux</td><td>faux positif</td><td>faux échec</td><td>rejeter l'incident, consigné à tort</td></tr>
<tr><td>c'est un faux</td><td>faux négatif</td><td>faux succès</td><td>consigner l'incident, oublié à tort</td></tr>
</tbody></table>

## Qu'en penser ? ##

Et les stagiaires en formation de s'interroger : pourquoi un tel acharnement à tirer les cheveux en quatre et à représenter ces deux modèles autour du faux pour dire la même chose, mais autrement ?

Mais parce que ce n'est pas le règne de la pensée unique, que plusieurs visions du monde (et du monde du test logiciel aussi) cohabitent, et que l'ISTQB collecte l'existant plutôt qu'il ne le réinvente. Gardez l'esprit ouvert.
<br >  
Pour vous y aider : [petit bonus surprise](https://www.francetvinfo.fr/animaux/en-images-voici-ce-que-voit-votre-chien_1008429.html "regardez par les yeux de votre chien").