# RP n°4 — Mise en place d’un système d’authentification sécurisé

## 1 — Description de la réalisation professionnelle

Dans la majorité des systèmes d’information modernes, l’accès aux applications doit être **contrôlé et sécurisé**.

Un système d’authentification permet :

* d’identifier un utilisateur
* de vérifier son identité
* de contrôler les actions qu’il peut réaliser

Dans cette réalisation professionnelle, l’étudiant met en place **un système complet de gestion des utilisateurs et d’authentification sécurisé** dans une application.

Le système doit inclure :

* création de compte
* connexion utilisateur
* sécurisation des mots de passe
* gestion de session ou de token
* éventuellement gestion des rôles

Cette réalisation peut être **intégrée dans une application existante** ou réalisée comme un **service indépendant**.

Elle correspond parfaitement aux exigences du développement d’applications professionnelles où **les accès aux données doivent être contrôlés conformément aux habilitations définies dans le cahier des charges**. 

---

# 2 — Exemples concrets de réalisations possibles

## Exemple 1 — Authentification pour une API

Contexte :
Une API interne permet de gérer des données sensibles.

Il est nécessaire de protéger l’accès.

Fonctionnalités :

* inscription utilisateur
* login
* génération d’un token JWT
* accès protégé aux endpoints

Architecture :

```
Utilisateur → login → API
                 ↓
             Token JWT
```

Endpoints :

```
POST /register
POST /login
GET /profile
```

---

## Exemple 2 — Authentification pour un site web

Contexte :
Un site web permet aux utilisateurs de gérer leurs données.

Fonctionnalités :

* création de compte
* connexion
* espace personnel
* déconnexion

Fonctionnalités sécurité :

* mot de passe hashé
* session sécurisée

---

## Exemple 3 — Authentification avec rôles

Contexte :
Une application de gestion comporte plusieurs types d’utilisateurs.

Exemples de rôles :

* utilisateur
* administrateur
* modérateur

Fonctionnalités :

* contrôle d’accès selon rôle
* interface différente selon rôle

---

## Exemple 4 — Authentification pour un client lourd

Contexte :
Une application desktop doit accéder à une API.

Processus :

1. l’utilisateur se connecte
2. l’API renvoie un token
3. le client utilise ce token pour les requêtes

---

# 3 — Technologies possibles

Cette RP peut être réalisée avec de nombreuses technologies.

### Backend

* Node.js (Express / NestJS)
* Laravel
* Django
* Spring Boot
* .NET

---

### Gestion des mots de passe

Les mots de passe doivent être **hachés**.

Exemples :

* bcrypt
* argon2

Exemple :

```javascript
bcrypt.hash(password, 10)
```

---

### Gestion de session

Deux approches principales :

#### Sessions

stockées sur le serveur.

---

#### JWT

token transmis dans les requêtes.

Exemple :

```http
Authorization: Bearer TOKEN
```

---

### Base de données

table utilisateurs :

```
users
-----
id
email
password
role
created_at
```

---

# 4 — Ce que l’étudiant doit produire

Pour que cette RP soit valorisable dans le portfolio, plusieurs éléments doivent être présentés.

---

## Code source

* système d’inscription
* login
* vérification du token
* protection des routes

---

## Base de données

script SQL ou migrations.

---

## Documentation technique

explication :

* fonctionnement de l’authentification
* technologies utilisées
* gestion de la sécurité

---

## Tests

tests possibles :

* login valide
* login invalide
* accès interdit sans token

---

# 5 — Pourquoi cette réalisation est pertinente pour le BTS

Cette réalisation est extrêmement représentative du développement professionnel.

Elle démontre notamment :

* la gestion des accès aux données
* la sécurisation des applications
* la gestion des utilisateurs

Dans les solutions applicatives, les accès aux données doivent être **contrôlés conformément aux habilitations définies**, ce qui correspond exactement à ce type de réalisation. 

---

# 6 — Compétences mobilisées (SLAM)

Cette RP permet de mobiliser plusieurs compétences importantes.

---

### Concevoir et développer une solution applicative

* conception du système d’authentification
* implémentation

---

### Gérer les données

* table utilisateurs
* gestion des identifiants

---

### Exploiter les technologies web

* HTTP
* tokens
* sessions

---

### Réaliser les tests nécessaires

* tests de connexion
* tests de sécurité

---

### Documenter une solution applicative

* description du mécanisme d’authentification

---

# 7 — Points forts de cette RP

Cette réalisation possède plusieurs avantages pédagogiques importants.

---

### Très réaliste

Toutes les applications modernes comportent :

**un système d’authentification.**

---

### Forte valeur technique

Elle démontre :

* gestion de la sécurité
* bonnes pratiques

---

### Facile à intégrer dans un projet existant

Elle peut être ajoutée à :

* une API
* un site web
* un client lourd

---

### Très valorisée par les jurys

Les jurys apprécient particulièrement les réalisations qui abordent :

* la sécurité
* la gestion des accès

---

# 8 — Ce qu’il faut valoriser dans le portfolio

Pour que la RP soit convaincante, certains éléments doivent être mis en avant.

---

## 1 — Le besoin

Expliquer :

* pourquoi l’application doit être sécurisée
* quels types d’utilisateurs existent

---

## 2 — Le modèle de données

Illustrer la table utilisateur.

---

## 3 — Le processus d’authentification

Schéma possible :

```
Utilisateur
    ↓
Login
    ↓
Vérification mot de passe
    ↓
Token
    ↓
Accès aux ressources
```

---

## 4 — La sécurité des mots de passe

expliquer :

* hash
* stockage sécurisé

---

## 5 — Les tests

montrer :

* login réussi
* login refusé
* accès protégé

---

# 9 — Améliorations possibles (bonus)

Pour enrichir la RP, les étudiants peuvent ajouter :

---

### vérification email

validation du compte.

---

### double authentification

code OTP.

---

### limitation des tentatives

protection contre brute force.

---

### récupération de mot de passe

réinitialisation par email.

---

# 10 — Durée estimée

Selon le niveau :

* **version simple : 2 à 3 jours**
* **version complète : 4 à 6 jours**
