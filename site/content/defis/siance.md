---
title: SIANCE
description: Améliorer le contrôle des activités nucléaires
who: Autorité de sûreté nucléaire
themes:
  - Santé-Environnement
  - Sécurité
promos:
  - Promotion 4
town: Montrouge (92120)
date: 2021-09-26T12:22:00.655Z
expertises:
  - Développement
  - Data science
image: img/eig4-siance.svg
visible: true
---
{{< dailymotion x82e0pj "Vidéo présentant les réalisations du défi SIANCE">}}

SIANCE est une plateforme de collecte et d’analyse de documents publics relatifs à la sûreté nucléaire et à la radioprotection. Elle est dotée d’une interface web adaptée aux activités de contrôle menées par l’Autorité de Sûreté Nucléaire.

## La problématique : des données provenant des inspections difficiles à analyser et à traduire en actions

La France possède actuellement 17 centrales en fonctionnement, 87 installations relatives à la vie du combustible mais aussi plus de 50 000 installations exposant à des rayonnements ou des sources radioactives, comme certaines installations médicales (hôpitaux, cliniques, dentistes, vétérinaires) ou industrielles. L’Autorité de sûreté nucléaire (ASN), en charge du contrôle de la sûreté nucléaire et de la radioprotection, effectue environ 1 800 inspections par an pour contrôler ces installations nucléaires et leurs équipements afin de garantir la protection des personnes et de l’environnement.

Lors d’un contrôle, les inspecteurs de l’ASN peuvent relever des écarts à la réglementation en vigueur; cette dernière relève entre autre des codes de l’environnement, du travail, de la santé publique, mais aussi de décrets propres à chaque installation majeure. À l’issue d’une inspection, une “lettre de suite” est envoyée à l’établissement contrôlé pour lui faire part des écarts constatés et lui demander de se mettre en conformité à la réglementation.

De plus, en cas d’incident relevant de la sûreté nucléaire ou de la radioprotection, toute installation est tenue d’envoyer à l’ASN un “compte rendu d’événement significatif” indiquant la nature et les causes de l’incident ainsi que les éventuels impacts sur les personnes et les équipements.

**L’ASN cherche à simplifier son processus d’inspection et d’évaluation en regroupant, organisant et consolidant les problématiques rencontrées par l’ASN et décrites dans les lettres de suite et les événements significatifs.**

## Le défi : faciliter le travail d’inspection et orienter la politique de contrôle des activités nucléaires

### Décloisonner et consolider les données

Nous avons organisé dans une base de données consolidée les lettres de suite produites par l’ASN, les installations inspectées, les événements significatifs ainsi que l’historique des différentes problématiques d’inspection de l’ASN depuis 2002.

Une interface web permet aux inspecteurs de valoriser ces données en croisant des informations qui étaient auparavant organisées trop différemment les unes des autres pour être comparées.

De plus, notre interface repose sur une *Application Programming Interface* (API) qui permet à l’écosystème numérique de l’ASN de bénéficier de cette base de connaissance.

### Améliorer la préparation des inspections

L’interface web permet de rassembler des lettres de suite et des comptes-rendus d’événements significatifs à l’échelle d’un établissement ou d’une problématique d’inspection, pour identifier notamment les problèmes récurrents sur un type d’installation. L’indexation de toutes les demandes précédemment faites par l’ASN facilite la recherche documentaire ainsi que la rédaction des lettres de suite.

### Donner une visibilité sur l’état de la sûreté nucléaire et de la radioprotection

Des indicateurs calculés sur la base des informations extraites des lettres de suite *via* de l’apprentissage automatique (traitement du langage naturel, *NLP*) et des traitements algorithmiques classiques permettent de suivre l’évolution de certaines problématiques, généralement ou sur des équipements spécifiques.

## Les étapes clefs

> * **Recherche utilisateur**: nous avons été à la rencontre des inspecteurs dans les directions régionales (qui suivent des établissements) et dans les directions nationales (qui suivent des problématiques).
> * **Apprentissage**: nous avons entraîné un algorithme de *machine learning* (NLP) pour classer de manière dite “supervisée” les sections des lettres de suite en fonction des problématiques qu’elles abordaient. Une *ontologie* (classification des problématiques de l’ASN, *typologie*) avait été déterminée en amont du défi par les inspecteurs.
> * **Production et consolidation de données**: notre processus d’ingestion des données traite les lettres de suite, les événements significatifs et les croise avec des informations externes (API sirene de l’INSEE, etc.).
> * **Harmonisation de 20 ans de données**: nous avons produit trois référentiels métiers qui répertorient les installations nucléaires, et les problématiques d’inspections afin de les harmoniser.
> * **Construction d’interfaces**: nous avons produit 6 écrans principaux qui répondent aux différents besoins des inspecteurs: “Préparer une inspection”, “Rechercher un document”, “Observer un document annoté par l’apprentissage”, “Planifier le programme d’inspection”, “Administrer le portail” (site, processus d’ingestion, apprentissage), “Évaluer une problématique de recherche”.
> * **Opérationnalisation**: dès le premier mois, nous avons déployé l’outil en production et en pré-production afin de bénéficier des retours des inspecteurs, d’adapter notre outil en continu et communiquer sur son existence.
> * **Liens avec d’autres institutions**: nous avons effectué de multiples présentations du projet SIANCE à des homologues étrangers de l’ASN et à des services du ministère de la Transition Écologique.

## Suite du défi

Pierre-Étienne Devineau a été prolongé jusqu’en décembre 2021 pour terminer l’industrialisation du projet. Durant ce temps il compte :

> * développer un outil pour faciliter l’analyse des indicateurs de sûreté nucléaires dûs par EDF
> * terminer l’interface d’annotation
> * publier le code source de l’application
> * améliorer les performances de l’algorithme d’apprentissage automatique
> * créer une API pour échanger avec PIREX, un outil d’analyse complémentaire de SIANCE développé par l’institut de radioprotection et de sûreté nucléaire (institut public expert intervenant avec l’ASN)
> * publier en *open data* le référentiel des installations nucléaires civiles