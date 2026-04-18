---
layout: "post"
title: "non, ce n'est pas une anomalie, c'est normale"
description: "Les termes sont importants. Ce n'est pas une anomalie parce que le comité ne l'estime pas comme tel, mais si un incident a réellement eu lieu..."
mytitle: "Mais est-ce vraiment une anomalie ?"
myexcerpt: "L'incident est lié à son rapporteur. Quelque chose s'est produit en lui qui a tiré le signal d'alarme. Tâchons de le comprendre."
mylabel: "apprenons les uns des autres"
permalink: "anomalie-normale"
comments: "Comment réagir face à ceux qui ont leur propre défintion de l'anomalie ?"
image: "/assets/img/anomalie-normale.jpg"
categories: []
tags: ["polemique"]

---
# Quoi, elle est normale, cette anomalie ? #

L'association des termes "normale anomalie" semble contradictoire : un oxymoron, non ? Pourtant, c'est une contradiction logique liée au moins à deux points :
  
- la gestion des priorités 
- et l'aspect pragmatique de nos activités.

## Les axiomes projet et test ##

Selon que l'on gravite dans certains univers professionnels (l'informatique), que l'on ait eu vent de certaines méthodes (gestion de projet) ou de certaines normes ou référentiels (ISTQB), on ne peut nier les éléments suivants : 
 
- On n'aura pas forcément le temps de tout faire.
- On n'aura pas forcément le droit de traiter toute chose à valeur égale.
- Gérer un projet, c'est gérer les priorités et les risques.
- Tout défaut n'a pas obligation à être corrigé.

Si vous n'en êtes pas convaincus, ouvrez la discussion ou ouvrez les ouvrages de référence.

## Le sens de la réalité ##

**Le sens de la réalité dans l'action**, qui est la gestion des arbitrages, ne doit/devrait pas supplanter le sens de **la réalité des faits**, qui est un peu le maître étalon d'une certaine vérité idéalisée mais indéniable.

Un comportement gênant concernant  "une anomalie normale", serait de nier qu'il s'agisse d'*incident* ou d'anomalie. Son existence est indubitable en tant qu'<a id="incident"></a><quote>événement ayant eu lieu et ayant choqué un testeur, [d'où le besoin d'une analyse plus poussée](http://glossary.istqb.org/search/incident "incident demandant enquête") sur les raisons de cette perception de distorsion entre attendu quelqu'en soit la raison et obtenu</quote>. Que son **statut de gravité ou de priorité** l'amène à être [rejetée](./statut-rejete "incident trivial rejete") n'entre pas en ligne de compte. Cet événement qui continuera d'avoir un caractère surprenant pour certains doit/devrait rester/exister dans l'inventaire.

Certains défauts avérés ne seront pas corrigés, et d'une certaine manière ne seront pas communément considérés comme des défauts par les non initiés au monde du test. Pourtant, pour les initiés cela demeure des défauts selon le caractère idéal de leur référence (voir l'article <sub>à venir</sub> sur la quête d'idal dans le test) :  

- recherche de perfection,
- niveau d'exigence,
- respect des règles de l'art,
- logique du comportement.

## Quelques exemples ##

Ce n'est pas normal mais c'est normal parce qu'on l'a laissé. 
 
- Le filtre ne fonctionne pas et tout s'affiche.
	- Finalement, ça arrange le métier parce qu'il voit tout et en a l'habitude maintenant.
	- On ne fait pas corriger ; je n'ai pas confiance, cela risquerait d'être pire.
- Le dernier icône crée soudain une deuxième ligne
	- On le sait, ce n'est pas responsive sur ce point mais ce n'est pas trop grave.


## L'impact du déni de réalité ##

Prenons le problème à l'envers. Si nous nions les faits, qu'arrive-t-il ?  

- Chaque nouveau venu ayant un vécu spécifique ou un niveau d'exigence particulier verra ce défaut comme une verrue au milieu du nez et le consignera, **à tort selon vous** et aura droit à vos réprimandes, **à tort selon lui**. Pas terrible pour le ressenti des uns et des autres.

Merci d'ajouter d'autres points encore <u>en commentaires</u> si vous en voyez.

## L'énoncé des règles du jeu ##

Dans le même ordre d'idées, certains incidents ne sont pas des <a id="correction"></a><quote>corrections (dûes par le fournisseur et jugées non conformes et leur modification est à la charge du fournisseur)</quote> mais des <a id="evolution"></a><quote>évolutions (oubliées ou non existantes à l'époque de la demande et donc à rejouter aux frais du client)</quote>, d'autres portent sur le système et non sur l'application sous test. Ce sont néanmoins des incidents, non ? Il n'y a pas de procès d'intention : qu'a-t-il voulu faire, devait-il le faire ?

Ou alors, si vous avez des spécificités telles qu'elles heurtent l'entendement, merci de les citer dans les *critères d'acceptation* des incidents ou anomalie. J'en parlais dans [l'article définissant le test](./test-logiciel "ce que tester veut dire"). La moindre des choses n'est-elle pas d'indiquer quelles sont les règles du jeu ?


Et vous, comment traitez-vous ce cas ? Sondage :  

- Vous ne rencontrez pas ce cas ou vous l'ignorez.
- Tout testeur doit prendre connaissance de ces cas particuliers.
- Vous devez chaque fois rejeter et clôturer l'incident.
- A chacun de rechercher avant si l'incident n'existe pas déjà.

