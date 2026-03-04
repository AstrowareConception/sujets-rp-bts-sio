# RP n°1 — Développement et déploiement d’une API REST

## 1 — Description de la réalisation professionnelle

Dans de nombreuses organisations modernes, les applications communiquent entre elles par l’intermédiaire d’**API (Application Programming Interface)**.

Une API REST permet d’exposer des données ou des services afin qu’ils puissent être consommés par d’autres applications : site web, application mobile, client lourd ou service interne.

Dans cette réalisation professionnelle, l’étudiant développe **une API REST complète permettant d’accéder à des données métier** (produits, utilisateurs, événements, réservations, etc.).

L’API doit être :

* structurée
* documentée
* sécurisée
* testée
* déployée

Même si le projet reste de taille limitée, il correspond parfaitement à une **situation professionnelle réelle**, puisque les API constituent aujourd’hui un élément central de l’architecture des systèmes d’information.

Cette RP peut être réalisée en **quelques jours à une semaine** tout en restant très pertinente pour un portfolio.

---

# 2 — Exemples concrets de réalisations possibles

## Exemple 1 — API de gestion d’une bibliothèque

Contexte :
Une médiathèque souhaite permettre à plusieurs applications d’accéder à son catalogue.

Fonctionnalités :

* liste des livres
* recherche par auteur
* ajout d’un livre
* modification
* suppression

Endpoints possibles :

```
GET /books
GET /books/{id}
POST /books
PUT /books/{id}
DELETE /books/{id}
```

Technologies possibles :

* Node.js + Express
* Laravel
* Flask
* Spring Boot

Base de données :

* MySQL
* PostgreSQL
* SQLite

---

## Exemple 2 — API de gestion d’événements

Contexte :
Une association organise des événements et souhaite exposer ses données pour un futur site web.

Fonctionnalités :

* consultation des événements
* création d’événement
* inscription à un événement

Endpoints :

```
GET /events
GET /events/{id}
POST /events
POST /events/{id}/register
```

---

## Exemple 3 — API météo interne

Contexte :
Une entreprise souhaite centraliser les données météo issues d’une API externe.

L’API développée agit comme **proxy interne**.

Fonctionnalités :

* récupération météo
* cache des données
* historisation

Endpoints :

```
GET /weather/{city}
GET /weather/history/{city}
```

---

## Exemple 4 — API de gestion de tâches (type mini Trello)

Fonctionnalités :

* création de tâches
* changement d’état
* assignation à un utilisateur

Endpoints :

```
GET /tasks
POST /tasks
PUT /tasks/{id}
DELETE /tasks/{id}
```

---

# 3 — Technologies possibles

Cette RP peut être réalisée avec quasiment n’importe quelle stack moderne.

Exemples :

### Backend

* Node.js (Express / NestJS)
* Python (Flask / FastAPI / Django)
* PHP (Laravel / Symfony)
* Java (Spring Boot)
* C# (.NET)

### Base de données

* MySQL
* PostgreSQL
* MongoDB
* SQLite

### Outils

* Postman
* Swagger / OpenAPI
* Docker (optionnel)
* GitHub

Ces outils correspondent parfaitement à l’environnement technologique attendu dans le BTS SIO (frameworks, gestion de versions, SGBD, tests). 

---

# 4 — Ce que l’étudiant doit produire

Pour que la RP soit exploitable dans le portfolio, il faut plusieurs livrables.

### Code source

* API complète
* structure claire
* organisation du projet

### Base de données

* script SQL
* ou migrations

### Documentation API

exemple :

Swagger / OpenAPI

ou

document décrivant les endpoints

### Tests

tests avec :

* Postman
* curl
* scripts automatisés

### Documentation technique

courte documentation expliquant :

* architecture
* technologies
* installation
* utilisation

---

# 5 — Pourquoi cette réalisation est pertinente pour le BTS

Cette RP correspond parfaitement à plusieurs éléments du référentiel.

Elle permet notamment de démontrer :

### Conception d’une solution applicative

L’étudiant :

* analyse un besoin
* modélise les données
* conçoit une architecture API

### Exploitation des technologies web

L’étudiant met en œuvre :

* HTTP
* REST
* JSON
* framework backend

### Gestion des données

L’étudiant :

* conçoit une base
* écrit des requêtes
* gère la persistance

Ces compétences font explicitement partie des capacités attendues dans l’épreuve de conception et développement d’applications. 

---

# 6 — Compétences mobilisées (SLAM)

Cette RP peut couvrir notamment :

### Concevoir et développer une solution applicative

* architecture API
* endpoints REST
* logique métier

### Exploiter les technologies Web

* HTTP
* JSON
* API

### Utiliser des composants d’accès aux données

* ORM
* requêtes SQL

### Réaliser les tests nécessaires

* tests d’API
* vérification des réponses

### Rédiger une documentation technique

* documentation des endpoints

---

# 7 — Points forts de cette RP

Cette réalisation est très intéressante pour plusieurs raisons.

### Très représentative du monde professionnel

Les API sont aujourd’hui **au cœur de presque toutes les architectures modernes**.

### Facilement démontrable

On peut montrer :

* les endpoints
* les requêtes
* les réponses JSON

### Réutilisable

L’API peut servir ensuite pour :

* un client web
* un client mobile
* un client lourd

### Compatible avec beaucoup de stacks

Chaque étudiant peut utiliser :

* son langage préféré
* son framework préféré

---

# 8 — Ce qu’il faut absolument valoriser dans le portfolio

Pour que la RP soit convaincante, il faut mettre en avant certains éléments.

### 1 — L’analyse du besoin

Expliquer :

* pourquoi l’API existe
* quel problème elle résout

---

### 2 — La conception

Montrer :

* schéma de la base de données
* architecture API

---

### 3 — Les endpoints

Documenter clairement :

```
GET /users
POST /users
PUT /users/{id}
DELETE /users/{id}
```

---

### 4 — Les tests

Captures :

* Postman
* requêtes HTTP

---

### 5 — Le déploiement

Même simple :

* serveur local
* Docker
* VPS

---

# 9 — Améliorations possibles (bonus)

Pour enrichir la RP, l’étudiant peut ajouter :

### authentification JWT

login + token

---

### pagination

```
GET /users?page=1
```

---

### validation des données

vérifier :

* email
* formats
* champs obligatoires

---

### documentation Swagger

interface interactive.

---

# 10 — Durée estimée

Selon le niveau :

* **minimum : 1 à 2 jours**
* **propre et documenté : 3 à 5 jours**

