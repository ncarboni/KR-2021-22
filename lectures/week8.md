---
layout: lecture
title: Week 8 - SPARQL
permalink: /seances/week8-sparql
parent: Séances
nav_order: 8
---


## Objectifs:

Modélisation avec CIDOC-CRM :
- Comment commencer  
- Relier les entités entre elles
- Définition et propriétés, où les chercher

Interroger les données :
- Introduction à SPARQL
- Éléments d'une requête
- Requêtes de base utilisant les wikidata
- Filtrage par le temps
- Filtrage par langue
- Filtrage à l'aide d'une chaîne de caractères contenue dans un littéral
- Exploration des données : OPTIONAL
- Naviguer sur le web des données
	- Fédération avec wikidata
	- Fédération avec wikidata et BNF SPARQL endpoint


## Revoir la séance

- Vous pouvez trouver la présentation [ici](../slides/KR8.pdf) 
- Vous pouvez trouver l'enregistrement de la séance [ici](https://mediaserver.unige.ch/play/164037)


## Lectures complémentaires

- [DuCharme, Bob. Learning SPARQL: querying and updating with SPARQL 1.1. " O'Reilly Media, Inc.", 2013.](https://drive.switch.ch/index.php/s/JmKdHHuM9Z5A4WZ)


## Exercice

Choisissez entre deux parmi les exercices suivants:

### SPARQL sur les données de Wikidata

Lien SPARQL wikidata: [https://query.wikidata.org](https://query.wikidata.org)


Créez une requête SPARQL qui
SELECT toutes les personnes qui:
- sont nées en Suisse après 1600
Pour chacune d'entre elles, récupérez
- leur nom en anglais
- leur image
- leur genre
- leur lieu de naissance
- leur identifiant de la Bibliothèque nationale de France

astuce : voir les propriétés d'une personne suisse bien décrite, exemple : [https://www.wikidata.org/wiki/Q59945](https://www.wikidata.org/wiki/Q59945)

Envoyez la requête SPARQL produite à l'enseignant avant mardi après-midi.

### SPARQL sur les données de la Bibliothèque nationale de France

Lien SPARQL BNF: [https://data.bnf.fr/sparql/](https://data.bnf.fr/sparql/)
Lien documentation modèle de données [https://data.bnf.fr/fr/semanticweb](https://data.bnf.fr/fr/semanticweb)

Créez une requête SPARQL qui
SELECT tous les livres qui 
- ont été publiés en Suisse
Pour chacun récupérez
- leur titre
- leur sujet
Limitez le résultat à 100.

Envoyez la requête SPARQL produite à l'enseignant avant mardi après-midi.

### SPARQL sur les données du Getty

Lien SPARQL Getty: [http://vocab.getty.edu/sparql](http://vocab.getty.edu/sparql)  
Lien ontologie Getty: [http://vocab.getty.edu/ontology](http://vocab.getty.edu/ontology)

En utilisant le sujet `<http://vocab.getty.edu/ulan/500027184>`
SELECT
- son nom
- toutes les relations sociales documentées 
- sa date de naissance et de décès 

### SPARQL sur les données Visual Contagions

Lien SPARQL Visual Contagions : [http://128.199.62.98:3030](http://128.199.62.98:3030/dataset.html?tab=query&ds=/Venus)
Modèle de données : [VisualContagion.png](../static/visualContagions.png)

SELECT 
Tous les objets qui ont former or current owner `<http://lod.unige.ch/visualcontagions/actor/owner113>`
et pour chacun d'eux trouvez:

- le temps où ils ont été produits

## Où trouver des ressources

- [CIDOC-CRM Class and properties declaration](https://cidoc-crm.org/html/cidoc_crm_v7.1.1.html)
- [CIDOC-CRM Ontologie en RDF](http://cidoc-crm.org/rdfs/7.1.1/CIDOC_CRM_v7.1.1.rdfs)
- [Wikidata Query Service Tutorial](https://wdqs-tutorial.toolforge.org).
- [Wikidata SPARQL Tutorial](https://www.wikidata.org/wiki/Wikidata:SPARQL_tutorial). 

## Vocabularies

L'utilisation de linked data vocabulaires dans le cadre du web sémantique permet de fixer le sens de notre modèle et d'en améliorer la réutilisabilité. Voici quelques vocabulaires intéressants pour notre domaine:

- [Art and Architecture Thesaurus](http://www.getty.edu/research/tools/vocabularies/aat/)
- [Homosaurus](https://homosaurus.org)
- [QUDT](http://qudt.org)


