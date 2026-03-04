# RP n°3 — Développement d’un client lourd consommant une API

## 1 — Description de la réalisation professionnelle

Dans certains contextes professionnels, les applications ne sont pas accessibles via un navigateur web mais via **des logiciels installés directement sur les postes utilisateurs**.

Ces applications sont appelées **clients lourds** (desktop applications). Elles permettent généralement :

* de manipuler des données métier
* de communiquer avec un serveur
* d’offrir une interface riche aux utilisateurs

Dans cette réalisation professionnelle, l’étudiant développe **une application desktop capable de communiquer avec une API distante pour récupérer ou modifier des données**.

L’application peut par exemple :

* consulter des données
* ajouter des éléments
* modifier des informations
* supprimer des données

Cette réalisation est particulièrement pertinente dans le cadre du BTS SIO car le référentiel prévoit explicitement que les solutions applicatives puissent comporter **du code exécuté sur un poste client (client lourd)**. 

---

# 2 — Exemples concrets de réalisations possibles

## Exemple 1 — Client de gestion de tâches

Contexte :
Une petite entreprise souhaite un logiciel simple permettant de gérer les tâches de son équipe.

L’application permet :

* afficher les tâches
* créer une tâche
* modifier une tâche
* marquer une tâche comme terminée

Le logiciel communique avec une API.

Interface :

* liste des tâches
* formulaire d’ajout
* boutons d’action

---

## Exemple 2 — Client de gestion de contacts

Contexte :
Un service commercial souhaite gérer ses contacts via une application simple.

Fonctionnalités :

* afficher les contacts
* ajouter un contact
* modifier un contact
* supprimer un contact

L’application consomme une API REST.

---

## Exemple 3 — Client de consultation d’articles

Contexte :
Une application interne permet de consulter les articles d’un catalogue.

Fonctionnalités :

* liste des produits
* fiche produit
* recherche

---

## Exemple 4 — Client de réservation

Contexte :
Une association dispose d’une API permettant de gérer des réservations.

L’application desktop permet :

* consulter les événements
* réserver une place
* voir les réservations

---

# 3 — Technologies possibles

Cette RP peut être réalisée avec plusieurs technologies adaptées au développement desktop.

### Java

* Java Swing
* JavaFX

Très pertinent dans le BTS.

---

### Python

* PyQt
* Tkinter

---

### C#

* WinForms
* WPF

---

### Electron

Applications desktop basées sur :

* HTML
* CSS
* JavaScript

---

### Communication API

Les appels peuvent se faire via :

HTTP / JSON.

Exemple en Java :

```java id="x92qu6"
HttpURLConnection connection = (HttpURLConnection) url.openConnection();
connection.setRequestMethod("GET");
```

---

# 4 — Ce que l’étudiant doit produire

Pour que cette réalisation soit exploitable dans un portfolio, plusieurs livrables sont nécessaires.

---

## Code source

Application complète :

* interface utilisateur
* communication API
* gestion des réponses

---

## Documentation technique

explication :

* architecture
* API utilisée
* structure du code

---

## Captures d’écran

* interface principale
* interaction avec les données

---

## Tests

démonstration :

* récupération de données
* création
* modification

---

# 5 — Pourquoi cette réalisation est pertinente pour le BTS

Cette réalisation est particulièrement intéressante car elle permet de démontrer une architecture complète :

```
Client lourd → API → Base de données
```

Elle illustre donc :

* la communication entre applications
* l’utilisation de services distants
* la conception d’interfaces utilisateurs

Le référentiel du BTS prévoit explicitement que les solutions applicatives puissent inclure **du code exécuté sur un système d’exploitation client**, ce qui correspond précisément à ce type de projet. 

---

# 6 — Compétences mobilisées (SLAM)

Cette RP peut démontrer plusieurs compétences importantes.

### Concevoir et développer une solution applicative

* architecture client / serveur
* logique métier

---

### Exploiter les technologies web

* appels HTTP
* échanges JSON

---

### Développer une interface utilisateur

* fenêtres
* formulaires
* interactions

---

### Utiliser des composants d’accès aux données

* récupération des données depuis l’API

---

### Tester une application

* vérification des fonctionnalités
* gestion des erreurs

---

# 7 — Points forts de cette RP

Cette réalisation présente plusieurs avantages pédagogiques.

---

### Architecture complète

Elle permet d’illustrer :

```
client → serveur → base de données
```

---

### Démonstration concrète

L’étudiant peut montrer :

* l’application
* les interactions
* les requêtes API

---

### Diversification des technologies

La majorité des projets étudiants sont :

* web

Cette RP permet de montrer :

* un autre type d’application.

---

### Forte valeur pédagogique

Elle démontre la capacité à :

* développer une application complète
* gérer une interface utilisateur
* communiquer avec un service distant

---

# 8 — Ce qu’il faut valoriser dans le portfolio

Pour que la RP soit convaincante, il faut mettre en avant plusieurs éléments.

---

## 1 — Le contexte

Expliquer :

* pourquoi une application desktop est utilisée
* quels utilisateurs sont concernés

---

## 2 — L’architecture

Illustrer :

```
Application Desktop
        ↓
API REST
        ↓
Base de données
```

---

## 3 — L’interface utilisateur

Captures :

* fenêtre principale
* formulaire
* interactions

---

## 4 — La communication API

exemple :

```
GET /tasks
POST /tasks
```

---

## 5 — La gestion des erreurs

exemples :

* API indisponible
* erreur réseau

---

# 9 — Améliorations possibles (bonus)

Les étudiants peuvent enrichir la RP avec plusieurs fonctionnalités.

---

### authentification

login / mot de passe

---

### synchronisation automatique

rafraîchissement des données.

---

### notifications

exemple :

* tâche ajoutée
* réservation confirmée

---

### mode hors ligne

stockage temporaire des données.

---

# 10 — Durée estimée

Selon la complexité :

* **version simple : 2 à 3 jours**
* **version complète : 4 à 6 jours**
