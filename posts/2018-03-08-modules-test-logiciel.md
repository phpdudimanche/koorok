---
layout: "post"
title: "un module de test dédié par besoin spécifique, et tout s'éclaire"
description: "Pour couvrir une activité de test complète et ses dépendances, le besoin en outillage peut être vaste. Comment isoler chacune des problématiques ?"
mytitle: "De quelle brique logicielle as-tu besoin ?"
myexcerpt: "A chaque besoin sa solution. A chaque problématique métier, son module logiciel. Pensons isolément."
mylabel: "un module par besoin"
permalink: "modules-test-logiciel"
comments: "Vous voyez quelque chose de plus ? Ajoutez votre grain de sel."
image: "/assets/img/modules-test-logiciel.gif"
categories: []
tags: ["outils"]

---

# De quel module ai-je besoin en test ?

Certains diront que je rêve, d'autres que j'observe. Je pense à un inventaire à la Prévert. On voit vite la réalité terrain ou les redondances apparaître. Je les note directement au sein de la liste pour chaque point. 

## Une liste exhaustive d'outils de test ou d'aide au test.

Tous ces outils ne sont pas à proprement parler des outils de test. Mais aucun des outils cités n'est sans effet sur l'activité de test.

1. Lotissement projet : découpage fonctionnel ou/et lignes budgétaires. Certains SI ont des outils de lotissement budgétaire qui s'ajoutent au découpage par fonction ou activité. Cela occasionne parfois de multiples saisies. En termes de traçabilité et d'interface, un incident pourrait se retrouver également lié à une ligne budgétaire précise qui facture son coût de traitement ou récupère le bénéfice apporté par la détection du risque.
2. Gestion des utilisateurs et des droits : rôles différents selon les projets ou même phases projet.  Pour un même outil, un utilisateur peut avoir plusieurs rôles répartis sur plusieurs projets. Dans chaque outil, on retrouve le module de gestion utilisateur. Les interfaces permettent sûrement de mutualiser l'effort, de centraliser le référencement de tous les droits multi applications multi projets par utilisateur, de propager les droits par SSO...
3. Gestion des disponibilités : présence, congés, jours fériés. Avis aux heureux salariés des SSII, euh ESN, qui saisissent leur temps et chez le client et dans leur société. La disponibilité réelle et à jour devrait forcément intervenir de façon intelligente dans l'outil suivant d'allocation des ressources aux activités projet.
4. Planification projet : découpage planning et allocation des hommes. Le coeur de la gestion projet : PBS, WBS et ici OBS. Les référentiels de test proposent l'allocation des tests aux ressources, voir même l'assignation de ces ativités dans une période de temsp déterminée.
5. Gestion des exigences : niveaux d'exigences, relations entre exigences, traçabilité. De plus en plus à la mode, et se confondant avec le module de lotissement par cycle de vie projet : le découpage Agile avec ses normalement "aides à la discussion" et "spécifications avec le juste niveau de détails nécessaires et connus à date".
6. Gestion des incidents : consignation des tickets, workflow, capitalisation sur le retour d'expérience. De plus en plus intégré ou interfacé à l'outil suivant de référentiel de test.
7. Référentiel de test : dépôt commun, maintenance. Nombre de personnes se focalisent sur cet outil pourtant optionnel et qui risque de biaiser le processus de test. S'interfacent avec ou comprennent de plus en plus d' outils de test IHM avec logiciels de capture vidéo.
8. Aide à la sélection des données de test : application des techniques  d'analyse boîtes noires par domaine, par wise... et boîtes blanches par couvertures de branches, de chemins, d'instructions,  décisions, conditions, conditions décisions, conditions décisions modifiées MCDC...  En fonction du risque renseigné, proposition de données discriminantes dans l'algorithme ou les règles de gestion.
9. Générateur de test : focalisation des tests, effort de test. Comme le RAD, utopie d'une modélisation mais plus BMP qu'UML afin de créer et surtout maintenir les tests à la volée : outils MBT.
10. Générateur de données : données factices, données périssables, besoin en volumétrie... Economiser du temps et respecter des règles de constitution de type regex, partager les données...
11. Gestionnaire de données : cohérence des données, dépendances aux environnements. Mise à disposition, traçabilité.
12. Gestion du code source : versionning, historisation, roll-back, travail en commun. Indispensable en Intégration Continue.
13. Outil d'intégration continue : interfaçage outil, interface web, historisation. Couramment utilisé our faciliter l'interfaçage entre outils.
14. Gestionnaire de configuration logicielle : OS, outils, réseau, serveurs, SI. Maintenir l'inventaire et le rendre disponible. 
15. Gestion des environnements virtualisés : VM de dev et test... Disposer des même environnments pour comparer ce qui est comparable. Emuler N environnements pour des tests de compatibilité : téléphone mobile spécifique, os, version OS, navigateur, version navigateur.
16. Gestionnaire de dépendance : maintenance des librairies. Facilitateur pour les installations et le partage des paramétrages.
17. Lanceur de tâche : automatisation, ordonnancement. Très vite pratique en automatisation.
18. Qualité du code : analyse de code source, détection d'antipattern, mesure de complexité cyclomatique, densité du code, pourcentage de commentaires. De la nécessité de savoir ce qu'on recherche et de doser le seuil d'alerte.
18. Outil de test unitaire : test runner, librairie d'assertion. Pléthore de solutions, mais choix dicté par le langage utilisé en code source.
19. Harnais de test : driver, mock, partial mock, spy, stub. Indispensable pour tester de manière isolée, en test unitaire et d'intégration.
20. Outil de test fonctionnel : drivers de navigateurs, copies d'écran. Liberté dans le choix des langages de script, mais limitation par les capacités de la solution à naviguer sur certains environnements : SAP, QT...
21. Outil de test serveur : performance, charge, volumétrie, stress. Possibilité de rejouer l'historique d'une production.
22. Rapports divers : harmonisation, indépendance, pérennisation pour le SI. Nombre d'outils précédemment cités se font fort de proposer leur propre moteur de reporting. D'autres normalisent les rapports, par exemple sous format Xml de type Junit. Certains autres facilitent l'accès à leurs données par des API ou une bonne documentation de leur modèle de données.

## Un sommaire pour des articles dédiés 

Voilà le programme. Peut-être aurais-je le temps de consacrer un article à chaque module, sauf si je n'ai aucune expérience sur le sujet. Ce qui est certain, c'est que pour les besoins de l'analyse, je prends le contrepied de [la solution logicielle complète qui brouille toutes les pistes](/outil-test-tout-en-un "isoler chaque besoin").

Et puisqu'on en est à parler de briques ou modules, petit bonus lego : http://agiteur.com/usine-lego-chiffres/