# 🏠 SQL – Analyse de Base de Données Assurance Habitation

## 📌 Description
Ce projet porte sur la conception, l'intégration et l'analyse d'une base de données relationnelle pour un système d'assurance habitation.

L'objectif est de transformer des données brutes (fichiers CSV) en une base de données fonctionnelle pour répondre à des problématiques métier :
- tarification  
- géographie  
- statistiques immobilières  

---

## 🎯 Présentation du projet
Ce projet consiste en la conception et l'exploitation d'une base de données relationnelle pour une compagnie d'assurance habitation.

L'objectif est de :
- centraliser les informations des contrats  
- exploiter les données géographiques  
- extraire des indicateurs clés de performance (**KPI**)  
- réaliser des analyses territoriales  

---

## 🛠️ Compétences techniques démontrées

- **Modélisation de données**
  - Création d'un dictionnaire de données  
  - Schéma relationnel normalisé  

- **SGBD relationnel**
  - Implémentation sous **SQLite 3**  

- **Data Loading**
  - Importation et vérification de jeux de données volumineux (> 69 000 lignes)  

- **SQL avancé**
  - Jointures (**JOIN**)  
  - Agrégations (**GROUP BY**)  
  - Filtrages (**HAVING**)  
  - Fonctions de fenêtrage  

---

## 🧱 Structure des données

### 📊 Dictionnaire des données

Le projet s'appuie sur deux tables principales reliées par une clé commune :

- **Table Contrat**
  - 14 colonnes (ID, adresse, surface, type de local, formule, prix mensuel, etc.)

- **Table Region**
  - 8 colonnes (code région, nom, académie, département, etc.)

---

### 🔗 Schéma relationnel

```sql
Contrat.Code_dep_code_commune = Region.Code_dep_code_commune

### 🔗📈 Analyses & résultats clés

Le projet a permis de répondre à 12 problématiques métier.

💰 1. Analyse de la tarification
Cotisation moyenne : 19,33 €
Top départements :
Paris (75) : 36,4 €
Hauts-de-Seine (92) : 26,24 €

🏡 2. Statistiques immobilières
Surfaces maximales : jusqu'à 815 m²
Répartition :
22 720 contrats entre 0 et 25 000 €

🗺️ 3. Distribution géographique
Île-de-France : 14 177 contrats
Provence-Alpes-Côte d’Azur : 3 279 contrats

### 🔗 📦 Livrables

- 📄 [Document technique](Kamoune_Assia_1_document technique_092025.pdf) : Détail des types de données et contraintes. 
- 📄 [Méthodologie](Kamoune_Assia_3_méthodologie_092025.pdf) : Étapes de réalisation et captures d'écran de la BDD chargée.

✅ Critères de validation

Le projet a été validé selon les critères suivants :

✔️ Base de données intègre
30 335 lignes dans Contrat
38 916 lignes dans Region
✔️ Absence d'erreurs SQL
✔️ Schéma relationnel respectant les formes normales

