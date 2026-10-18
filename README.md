# Semaine 9 - Jour 1 - Introduction aux bases de données

# NOM : MATSINKOU TAKOUDJOU MEGANE KASSANDRA

## 1. Définition d'une base de données relationnelle

Une base de données relationnelle est un système qui permet de stocker et d'organiser des données dans des tables composées de lignes et de colonnes, avec la possibilité de relier ces tables entre elles.

## 2. Rôle d'une clé primaire

Une clé primaire (PRIMARY KEY) permet d'identifier chaque ligne d'une table de manière unique. Elle ne peut pas contenir de doublons.

## 3. Différence entre SQLite et PostgreSQL

SQLite stocke les données dans un fichier et ne nécessite pas de serveur séparé. PostgreSQL utilise un serveur de base de données et convient mieux aux applications multi-utilisateurs nécessitant une gestion avancée des accès simultanés.

## 4. Exercices réalisés

Exercice 1 : Création de la table students.

Exercice 2 : Création de la table courses.

Exercice 3 : Comparaison entre SQLite et PostgreSQL et compréhension des bases de données relationnelles.

## Exercice 1 : Questions de compréhension

### 1. Pourquoi chaque table devrait-elle posséder une clé primaire ?

Chaque table devrait posséder une clé primaire (PRIMARY KEY) pour identifier de manière unique chaque ligne. Elle permet d'éviter les doublons d'identification et facilite les relations entre les tables.

### 2. Quelle différence faites-vous entre une ligne et une colonne ?

Une ligne représente un enregistrement complet dans une table, par exemple les informations d'un étudiant.

Une colonne représente un attribut ou une caractéristique des enregistrements, par exemple le nom, l'âge ou l'adresse email d'un étudiant.

### 3. Pourquoi email est-il stocké en TEXT et age en INTEGER ?

L'email est stocké en TEXT parce qu'il contient des caractères, des lettres et des symboles. Il ne sert pas à effectuer des calculs mathématiques.

L'âge est stocké en INTEGER parce qu'il représente un nombre entier et peut être utilisé dans des comparaisons numériques.


## Exercice 2 : comparaison des tables

| Critère | students | courses |
|---|---|---|
| Clé primaire | `id` | `id` |
| Colonnes TEXT | `first_name`, `last_name`, `email`, `created_at` | `title`, `description`,`level`, `created_at` |
| Colonnes INTEGER | `age` | `duration_hours` |
| Valeur par défaut | `created_at` = `CURRENT_TIMESTAMP` | `level` = `'Beginner'`,`created_at` = `CURRENT_TIMESTAMP` |
| Colonnes obligatoires | `first_name`, `last_name`, `email` | `title` |


