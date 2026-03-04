# RP n°5 — Développement et déploiement d’un micro-service Dockerisé

## 1 — Description de la réalisation professionnelle

Dans les architectures modernes, les applications sont souvent découpées en **micro-services**.

Un micro-service est un **petit service autonome**, spécialisé dans une fonction précise du système d’information et accessible via une API.

Par exemple :

* un service de gestion des utilisateurs
* un service de gestion des commandes
* un service de notification
* un service de génération de rapports

Chaque micro-service peut être **déployé indépendamment**, souvent dans un conteneur Docker.

Dans cette réalisation professionnelle, l’étudiant développe **un micro-service simple exposant une API et déployé dans un conteneur Docker**.

L’objectif est de démontrer :

* la conception d’un service applicatif
* sa conteneurisation
* son déploiement

Ce type d’architecture est très courant dans les systèmes modernes et correspond à l’utilisation de **services applicatifs distants permettant l’échange de données entre applications**, notion explicitement attendue dans les solutions applicatives du BTS. 

---

# 2 — Exemples concrets de réalisations possibles

## Exemple 1 — Micro-service de gestion des utilisateurs

Fonction :

gérer les utilisateurs d’un système.

Endpoints :

```id="hbo9e3"
GET /users
GET /users/{id}
POST /users
DELETE /users/{id}
```

Le service :

* stocke les utilisateurs
* expose une API
* fonctionne dans un conteneur Docker

---

## Exemple 2 — Micro-service de notifications

Contexte :
Une application doit envoyer des notifications aux utilisateurs.

Fonctionnalités :

* création de notification
* consultation des notifications

Endpoints :

```id="syrukn"
GET /notifications
POST /notifications
```

---

## Exemple 3 — Micro-service de statistiques

Contexte :
Une application souhaite afficher des statistiques.

Fonctionnalités :

* calcul des statistiques
* renvoi des résultats

Endpoints :

```id="y05h6h"
GET /stats
```

---

## Exemple 4 — Micro-service de génération de rapports

Fonction :

* générer des rapports PDF
* récupérer les rapports

Endpoints :

```id="ehj3fu"
POST /report
GET /report/{id}
```

---

# 3 — Architecture du projet

Une architecture typique peut être :

```id="yvtbn5"
Client
   ↓
API Gateway / Application
   ↓
Micro-service
   ↓
Base de données
```

Dans une petite RP, l’architecture peut être simplifiée :

```id="rxye4s"
Client → Micro-service → Base de données
```

---

# 4 — Technologies possibles

Cette RP peut être réalisée avec de nombreuses technologies.

---

## Backend

* Node.js
* Python (Flask / FastAPI)
* Java (Spring Boot)
* PHP (Laravel)
* .NET

---

## Base de données

* PostgreSQL
* MySQL
* MongoDB
* SQLite

---

## Docker

Le service est conteneurisé.

Exemple de Dockerfile :

```dockerfile id="nh7gq6"
FROM node:18
WORKDIR /app
COPY . .
RUN npm install
CMD ["node", "app.js"]
```

---

## Docker Compose (optionnel)

Permet de lancer plusieurs services :

```yaml id="8mjuip"
services:
  api:
    build: .
    ports:
      - "3000:3000"
```

---

# 5 — Ce que l’étudiant doit produire

Pour que cette RP soit exploitable dans le portfolio, plusieurs éléments doivent être présentés.

---

## Code source

micro-service complet :

* API
* logique métier
* accès base de données

---

## Dockerfile

permettant de construire le conteneur.

---

## Script de lancement

par exemple :

```id="okm2ab"
docker build -t service .
docker run -p 3000:3000 service
```

---

## Documentation technique

expliquant :

* architecture
* endpoints
* déploiement

---

## Tests

tests possibles :

* appels API
* vérification des réponses

---

# 6 — Pourquoi cette réalisation est pertinente pour le BTS

Cette réalisation correspond parfaitement à plusieurs éléments du référentiel :

* développement d’un service applicatif
* communication entre applications
* exploitation de technologies web
* déploiement d’un service

Elle montre également que l’étudiant est capable de produire **une solution applicative opérationnelle dans un environnement de production**, ce qui correspond aux attentes du référentiel. 

---

# 7 — Compétences mobilisées (SLAM)

Cette RP permet de démontrer plusieurs compétences importantes.

---

### Concevoir et développer une solution applicative

* conception du micro-service
* endpoints API

---

### Exploiter les technologies Web

* HTTP
* JSON
* REST

---

### Utiliser des composants d’accès aux données

* accès base de données

---

### Tester une solution applicative

* tests des endpoints

---

### Exploiter un environnement de développement

* Docker
* outils de build

---

# 8 — Points forts de cette RP

Cette réalisation possède plusieurs avantages.

---

### Architecture moderne

Les micro-services sont utilisés dans :

* les grandes plateformes web
* les architectures cloud

---

### Introduction au DevOps

Elle permet de montrer :

* conteneurisation
* déploiement

---

### Réutilisable

Le micro-service peut être utilisé par :

* un site web
* un client lourd
* une application mobile

---

### Très démonstratif

On peut montrer :

* l’API
* le conteneur
* le déploiement

---

# 9 — Ce qu’il faut valoriser dans le portfolio

Pour rendre la RP convaincante, certains éléments doivent être mis en avant.

---

## 1 — Le besoin

Expliquer :

* pourquoi ce service existe
* quel problème il résout

---

## 2 — L’architecture

Illustrer la place du micro-service dans le système.

---

## 3 — Les endpoints

Documenter :

```id="vpt5b6"
GET /users
POST /users
DELETE /users/{id}
```

---

## 4 — La conteneurisation

Expliquer :

* Dockerfile
* construction de l’image
* lancement du service

---

## 5 — Les tests

montrer :

* requêtes API
* réponses

---

# 10 — Améliorations possibles (bonus)

Les étudiants peuvent enrichir la RP avec plusieurs éléments.

---

### logs

journalisation des requêtes.

---

### authentification

protection des endpoints.

---

### monitoring

statistiques du service.

---

### CI/CD

déploiement automatique.

---

# 11 — Durée estimée

Selon la complexité :

* **version simple : 2 à 3 jours**
* **version complète : 4 à 6 jours**
