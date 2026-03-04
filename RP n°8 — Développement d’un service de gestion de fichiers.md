# RP n°8 — Développement d’un service de gestion de fichiers (upload / téléchargement)

## 1 — Description de la réalisation professionnelle

Dans de nombreuses applications professionnelles, les utilisateurs doivent pouvoir **envoyer, stocker et récupérer des fichiers**.

Exemples :

* dépôt de documents
* partage de fichiers internes
* stockage de pièces jointes
* gestion de médias

Dans cette réalisation professionnelle, l’étudiant développe **un service permettant la gestion de fichiers**, avec des fonctionnalités telles que :

* upload de fichiers
* téléchargement
* suppression
* consultation des fichiers disponibles

Le service peut être exposé via :

* une API
* une interface web
* une application desktop

Cette réalisation correspond à une problématique très fréquente dans les systèmes d’information : **la gestion sécurisée de fichiers utilisateurs**.

---

# 2 — Exemple de contexte professionnel

Une organisation souhaite permettre aux utilisateurs de :

* déposer des documents
* consulter les fichiers disponibles
* télécharger des documents

Actuellement, les fichiers sont partagés de manière non structurée (emails, stockage local, etc.).

Une solution informatique doit être mise en place pour :

* centraliser les fichiers
* simplifier leur gestion
* sécuriser leur accès.

---

# 3 — Exemples concrets de réalisations possibles

## Exemple 1 — Service d’upload de documents

Contexte :
Une application doit permettre aux utilisateurs de déposer des documents.

Fonctionnalités :

* upload de fichier
* liste des documents
* téléchargement

Exemple d’API :

```id="tqslq5"
POST /upload
GET /files
GET /files/{id}
DELETE /files/{id}
```

---

## Exemple 2 — Gestion de photos

Contexte :
Une application permet de stocker des photos.

Fonctionnalités :

* upload d’image
* affichage galerie
* suppression

---

## Exemple 3 — Partage de fichiers interne

Contexte :
Une entreprise souhaite partager des fichiers entre ses collaborateurs.

Fonctionnalités :

* upload
* téléchargement
* recherche de fichiers

---

## Exemple 4 — Gestion de pièces jointes

Contexte :
Une application de gestion doit permettre d’ajouter des fichiers aux dossiers.

Fonctionnalités :

* attacher un fichier à un enregistrement
* consulter les pièces jointes

---

# 4 — Architecture possible

Architecture simple :

```id="glg6ek"
Utilisateur → Application → Stockage fichiers
                       ↓
                    Base de données
```

La base de données peut stocker :

* nom du fichier
* taille
* date
* utilisateur

---

# 5 — Technologies possibles

Cette RP peut être réalisée avec de nombreuses technologies.

---

## Backend

* Node.js (Express)
* Laravel
* Django
* Spring Boot

---

## Stockage des fichiers

plusieurs possibilités :

* stockage local
* stockage cloud
* base de données

Exemple de structure :

```id="5kgkdd"
uploads/
  file1.pdf
  file2.jpg
```

---

## Base de données

table possible :

```id="8a2u1u"
files
-----
id
filename
path
size
uploaded_at
```

---

## Upload HTTP

Les fichiers sont envoyés via :

```id="3qmy45"
multipart/form-data
```

---

# 6 — Ce que l’étudiant doit produire

Pour que la RP soit exploitable dans le portfolio, plusieurs éléments doivent être présentés.

---

## Code source

application permettant :

* upload
* téléchargement
* suppression

---

## Structure de stockage

organisation des fichiers.

---

## Base de données

structure de la table fichiers.

---

## Documentation technique

explication :

* fonctionnement
* endpoints
* stockage

---

## Tests

exemples :

* upload réussi
* téléchargement
* suppression

---

# 7 — Pourquoi cette réalisation est pertinente pour le BTS

Cette RP correspond à des situations très fréquentes dans les applications professionnelles :

* gestion de documents
* manipulation de fichiers
* stockage de données

Elle démontre la capacité à **concevoir et développer une solution applicative permettant l’échange et la gestion de données**, ce qui correspond aux compétences attendues dans le référentiel. 

---

# 8 — Compétences mobilisées (SLAM)

Cette RP peut mobiliser plusieurs compétences importantes.

---

### Concevoir et développer une solution applicative

* architecture du service
* gestion des fichiers

---

### Gérer les données

* stockage des métadonnées
* base de données

---

### Exploiter les technologies web

* HTTP
* upload de fichiers

---

### Tester une solution

* vérification des uploads
* gestion des erreurs

---

### Documenter une solution

* explication du fonctionnement

---

# 9 — Points forts de cette RP

### Très réaliste

La gestion de fichiers est présente dans :

* intranets
* plateformes collaboratives
* applications métiers.

---

### Fonctionnalité visible

L’étudiant peut facilement démontrer :

* upload
* téléchargement

---

### Facile à combiner avec d’autres RP

Cette fonctionnalité peut être intégrée à :

* une API
* un site web
* un client lourd

---

### Possibilité d’ajouter des aspects sécurité

Par exemple :

* restriction d’accès
* validation de fichiers

---

# 10 — Ce qu’il faut valoriser dans le portfolio

Pour que la RP soit convaincante, il faut mettre en avant :

---

## le besoin

centralisation des fichiers.

---

## l’architecture

stockage + base de données.

---

## le fonctionnement

upload / téléchargement.

---

## les tests

exemples de fichiers envoyés.

---

# 11 — Améliorations possibles (bonus)

Les étudiants peuvent enrichir la RP avec plusieurs fonctionnalités.

---

### limitation de taille

contrôle des fichiers.

---

### validation des types

exemple :

* PDF
* images

---

### gestion des utilisateurs

fichiers associés à un utilisateur.

---

### génération de miniatures

pour images.

---

# 12 — Durée estimée

* **version simple : 2 jours**
* **version complète : 3 à 5 jours**
