## Version postgreSQL equivalente

CREATE TABLE products (
id INTEGER GENERATED ALWAYS AS IDENTITY PRIMARY KEY ,
name TEXT NOT NULL ,
price NUMERIC (10,2) NOT NULL ,
stock INTEGER DEFAULT 0
);

## Exercice 3 : Comparaison conceptuelle

### 1. Pourquoi SQLite est pratique pour apprendre et prototyper ?

SQLite est facile à utiliser, car il ne nécessite pas l'installation d'un serveur de base de données. Il est léger, rapide à configurer et permet de tester rapidement une application.

### 2. Pourquoi PostgreSQL est-il mieux adapté à une application web multi-utilisateur ?

PostgreSQL est conçu pour gérer plusieurs utilisateurs et de nombreuses opérations simultanées. Il offre une bonne gestion des transactions, des permissions et de la sécurité, ce qui le rend adapté aux applications web.

### 3. Que signifie « base basée sur un fichier » dans le cas de SQLite ?

Cela signifie que la base de données est stockée directement dans un fichier, par exemple `academy.db`, sur le disque. Les tables et les données sont conservées dans ce fichier, sans nécessiter un serveur de base de données séparé.

### 4. Pourquoi une application Django peut-elle fonctionner avec SQLite en développement puis PostgreSQL en production ?

SQLite permet de développer et de tester facilement une application Django en local. En production, PostgreSQL peut être utilisé pour mieux gérer plusieurs utilisateurs, les accès concurrents et une quantité plus importante de données. Django prend en charge les deux systèmes grâce à sa configuration de base de données, sans nécessiter de réécrire toute l'application.
