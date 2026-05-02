# SQL-Analyse-de-Base-de-Donn-es-Assurance-Habitation
Ce projet porte sur la conception, l'intégration et l'analyse d'une base de données relationnelle pour un système d'assurance habitation. L'objectif est de transformer des données brutes (fichiers CSV) en une base de données fonctionnelle pour répondre à des problématiques métier (tarification, géographie, statistiques immobilières).

Présentation du projet:
Ce projet consiste en la conception et l'exploitation d'une base de données relationnelle pour une compagnie d'assurance habitation. 
L'objectif est de centraliser les informations des contrats et les données géographiques afin d'en extraire des indicateurs clés de performance (KPI) et des analyses territoriales.  

Compétences techniques démontrées:
Modélisation de données : Création d'un dictionnaire de données et d'un schéma relationnel normalisé.  
SGBD Relatinnel : Implémentation sous SQLite 3.  
Data Loading : Importation et vérification de jeux de données volumineux (> 69 000 lignes cumulées).  
SQL Avancé : Rédaction de requêtes complexes avec jointures, agrégations (GROUP BY), filtrages (HAVING) et fonctions de fenêtrage.  

Structure des Données:Dictionnaire des Données:
Le projet s'appuie sur deux tables principales reliées par une clé commune :
Table Contrat : Contient 14 colonnes (ID, adresse, surface, type de local, formule, prix mensuel, etc.).  
Table Region : Contient 8 colonnes (Code région, nom, académie, département, etc.).  

Schéma Relationnel:
La relation est établie via la clé étrangère :
Contrat.Code_dep_code_commune ↔️ Region.Code_dep_code_commune.  

Analyses & Résultats Clés:
Le projet a permis de répondre à 12 problématiques métier. Voici quelques extraits : 

1. Analyse de la tarification:
Cotisation moyenne : Le prix moyen d'une cotisation mensuelle est de 19,33 €.
Top départements : Paris (75) et les Hauts-de-Seine (92) sont les départements affichant les cotisations les plus élevées (respectivement 36,4 € et 26,24 € en moyenne).

2. Statistiques Immobilières
Surfaces maximales : Identification des contrats avec les plus grandes surfaces (jusqu'à 815 m²).
Répartition par valeur : La majorité des contrats (22 720) concernent des biens d'une valeur comprise entre 0 et 25 000 €.

3. Distribution Géographique:
Volume par région : L'Île-de-France arrive en tête avec 14 177 contrats, suivie par la région Provence-Alpes-Côte d'Azur (3 279).

Livrables inclus:
Le dépôt contient la documentation complète du projet :
[Kamoune_Assia_1_document technique_092025.pdf] : Spécifications techniques et dictionnaire de données.  
[Kamoune_Assia_3_méthodologie_092025.pdf] : Étapes de réalisation et captures d'écran de la base de données fonctionnelle.  

Critères de validation:
Le projet a été validé selon les critères suivants : 
Base de données intègre (30 335 lignes dans Contrat, 38 916 dans Region).
Absence d'erreurs SQL sur l'ensemble des requêtes.
Schéma relationnel respectant les formes normales.
