# Applications_Distribues
# Java JDBC avec PostgreSQL 16

## 📌 Description
Ce projet est une application Java utilisant **JDBC** pour se connecter à une base de données **PostgreSQL 16**, insérer des utilisateurs et les récupérer.

---

## 🚀 Fonctionnalités
- Connexion à PostgreSQL via JDBC
- Création d’une table `users`
- Insertion de nouveaux utilisateurs
- Récupération et affichage des utilisateurs existants

---

## 🛠️ Installation et Exécution

### 1️⃣ Prérequis
- **Java JDK 8+** ([Télécharger ici](https://www.oracle.com/java/technologies/javase-downloads.html))
- **PostgreSQL 16** ([Télécharger ici](https://www.postgresql.org/download/))
- **Driver JDBC PostgreSQL** (`postgresql-42.7.2.jar`)

---

### 2️⃣ Création de la base de données PostgreSQL
Ouvrez **psql** et exécutez :
```sql
CREATE DATABASE my_jdbc_db;
\c my_jdbc_db;

CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL
);
