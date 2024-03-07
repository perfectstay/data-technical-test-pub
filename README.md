# Technical Test for Data Engineers

> :warning: This test can be done in Python or in GOLANG.

## Objective

The goal of this test is to assess your practical data engineering skills, especially in data manipulation and analysis with SQL, database usage, and writing unit tests to validate your code.

## Instructions

### 1. Environment Setup

Choose between SQLite and PostgreSQL for this test. If you opt for PostgreSQL, please run it in a Docker container. Installation instructions for Docker and PostgreSQL are not covered in this document, but many resources are available online.

### 2. Data Import

In the 'resources' directory, you will find three CSV files: `customers.csv`, `orders.csv`, and `products.csv`. Your first task is to load these files into your chosen database.

### 3. First Query: 'Sales Report'

- **Objective**: Create a `Sales_Report` table that compiles and analyzes sales data by product category, region, and month.
- **`Sales_Report` Table Content**:
  - `Category`
  - `Region`
  - `Month`
  - `Total_Sales`: Total sales for the category and region in the month.
  - `Margin`: Difference between the selling price and the purchase price, aggregated by category and region.

**Execution and Exportation**: After executing the query, export the result into a CSV file named `sales_report.csv`.

### 4. Second Query: 'Customer Analysis'

**Objective**: Create a `Customer_Analysis` table that will provide valuable insights into customer buying behavior and product performance by category and region. This table will include metrics such as the total amount spent by each customer, the most purchased product by category, and the purchase frequency.

### Query Description

The `Customer_Analysis` table will contain the following columns:
- `Customer_ID`: Unique identifier of the customer.
- `Region`: Customer's region.
- `Favorite_Category`: The most purchased product category by the customer.
- `Total_Spent`: The total amount spent by the customer.
- `Favorite_Product`: The name of the most purchased product by the customer across all categories.
- `Purchase_Frequency`: Average number of days between purchases.

**Execution and Exportation**: After executing the query, export the result into a CSV file named `customer_analysis.csv`.

### 5. Unit Tests

Write at least one unit test for each SQL query to demonstrate your ability to validate the logic and results of your queries. Use a testing framework of your choice (for example, `unittest` in Python).

## Evaluation Criteria

- Clarity and organization of the code.
- Accuracy of the SQL queries relative to the defined objectives.
- Quality and relevance of the unit tests.
- Instructions for running the tests and application.

## Submission

Please submit your source code, SQL scripts, exported CSV files, and any other relevant file (such as a Dockerfile if applicable) in a compressed (ZIP) directory or via a Git repository link.


----------------------------------------------------------------------------------------------------------------------------

## French Version

# Test Technique pour Ingénieur de Données

> :warning: Ce test pourra etre réalisé en Python ou en GOLANG

## Objectif

L'objectif de ce test est d'évaluer vos compétences pratiques en ingénierie de données, notamment en matière de manipulation et d'analyse de données avec SQL, de l'utilisation de bases de données, et de l'écriture de tests unitaires pour valider votre code.

## Instructions

### 1. Préparation de l'Environnement

Choisissez entre SQLite et PostgreSQL pour ce test. Si vous optez pour PostgreSQL, veuillez l'exécuter dans un conteneur Docker. Les instructions d'installation de Docker et de PostgreSQL ne sont pas couvertes dans ce document, mais de nombreuses ressources sont disponibles en ligne.

### 2. Importation des Données

Vous trouverez le repertoire 'resources' trois fichiers CSV : `customers.csv`, `orders.csv`, et `products.csv`. Votre première tâche consiste à charger ces fichiers dans votre base de données de choix.


### 3. Première Requête: 'Rapport Ventes'

- **Objectif** : Créer une table `Rapport_Ventes` qui compile et analyse les données de vente par catégorie de produit, région, et mois.
- **Contenu de la Table `Rapport_Ventes`** :
  - `Categorie`
  - `Region`
  - `Mois`
  - `Total_Ventes` : Total des ventes pour la catégorie et la région dans le mois.
  - `Marge` : Différence entre le prix de vente et le prix d'achat, agrégé par catégorie et région.

**Exécution et Exportation** : Après avoir exécuté la requête, exportez le résultat dans un fichier CSV nommé `rapport_ventes.csv`.


### 4. Deuxième Requête: 'Analyse_Clients'

**Objectif** : Créer une table `Analyse_Clients` qui fournira des insights précieux sur le comportement d'achat des clients et la performance des produits par catégorie et par région. Cette table inclura des mesures telles que le montant total dépensé par chaque client, le produit le plus acheté par catégorie, et la fréquence d'achat.

### Description de la Requête

La table `Analyse_Clients` contiendra les colonnes suivantes :
- `ID_Client` : Identifiant unique du client.
- `Region` : Région du client.
- `Categorie_Preferee` : La catégorie de produits la plus achetée par le client.
- `Depense_Totale` : Le montant total dépensé par le client.
- `Produit_Prefere` : Le nom du produit le plus acheté par le client toutes catégories confondues.
- `Frequence_Achat` : Nombre moyen de jours entre les achats.

**Exécution et Exportation** : Après avoir exécuté la requête, exportez le résultat dans un fichier CSV nommé `analyses_client.csv`.

### 5. Tests Unitaires

Écrivez au moins un test unitaire pour chaque requête SQL pour démontrer votre capacité à valider la logique et les résultats de vos requêtes. Utilisez un framework de test de votre choix (par exemple, `unittest` en Python).

## Critères d'Évaluation

- Clarté et organisation du code.
- Exactitude des requêtes SQL par rapport aux objectifs définis.
- Qualité et pertinence des tests unitaires.

## Soumission

Veuillez soumettre votre code source, les scripts SQL, les fichiers CSV exportés, et tout autre fichier pertinent (comme un fichier Dockerfile si applicable) dans un répertoire compressé (ZIP) ou via un lien de dépôt Git.
