# RP n°2 — Développement d’une interface Web consommant une API

## 1 — Description de la réalisation professionnelle

Dans de nombreux systèmes d’information modernes, les applications sont séparées en deux parties :

* **le backend** qui expose des données (souvent via une API REST)
* **le frontend** qui permet aux utilisateurs d’interagir avec ces données

Dans cette réalisation professionnelle, l’étudiant développe **une interface web permettant de consommer une API existante et d’afficher ses données de manière exploitable par un utilisateur**.

L’application web peut être :

* un tableau de bord
* une interface de consultation
* une application métier simplifiée

L’objectif n’est pas de créer un site complexe mais de démontrer la capacité à :

* exploiter un service distant
* manipuler des données JSON
* construire une interface utilisateur
* gérer les erreurs et les interactions

Cette réalisation est **très réaliste professionnellement**, car une grande partie du développement web consiste précisément à créer des interfaces consommant des API.

---

# 2 — Exemples concrets de réalisations possibles

## Exemple 1 — Tableau de bord météo

Contexte :
Une entreprise souhaite afficher la météo de plusieurs villes sur un tableau de bord interne.

L’application :

* interroge une API météo
* affiche les températures
* montre l’évolution météo

Fonctionnalités :

* sélection d’une ville
* affichage météo
* icônes météo

API possibles :

* OpenWeatherMap
* WeatherAPI

---

## Exemple 2 — Visualisation des dépôts GitHub

Contexte :
Un responsable technique souhaite consulter les informations des projets d’une organisation GitHub.

Fonctionnalités :

* liste des dépôts
* nombre de stars
* dernières mises à jour

API utilisée :

GitHub API

---

## Exemple 3 — Tableau de bord de suivi d’utilisateurs

Contexte :
Une application interne expose une API de gestion des utilisateurs.

L’interface permet :

* afficher les utilisateurs
* rechercher
* trier
* consulter un profil

Fonctionnalités :

* tableau dynamique
* filtre
* pagination

---

## Exemple 4 — Application de gestion de films

L’interface utilise une API de films :

* OMDb
* TMDB

Fonctionnalités :

* recherche de films
* affichage affiche
* description

---

# 3 — Technologies possibles

Cette RP peut être réalisée avec de nombreuses technologies.

### Frontend simple

* HTML
* CSS
* JavaScript

avec :

```javascript
fetch("https://api.example.com/data")
```

---

### Frameworks frontend

* Vue.js
* React
* Angular

---

### Librairies UI

* Bootstrap
* Tailwind
* Material UI

---

### Visualisation de données

* Chart.js
* ApexCharts
* D3.js

Ces technologies correspondent aux compétences liées à l’exploitation des technologies web dans les solutions applicatives du référentiel. 

---

# 4 — Ce que l’étudiant doit produire

Pour transformer ce projet en **réalisation professionnelle exploitable dans le portfolio**, plusieurs éléments doivent être fournis.

### Code source

application web fonctionnelle

structure claire :

```
src/
components/
services/
api/
```

---

### Documentation technique

explication :

* architecture
* API utilisée
* installation

---

### Captures d’écran

* interface
* résultats

---

### Tests

exemples :

* capture des appels API
* console navigateur
* gestion des erreurs

---

# 5 — Pourquoi cette réalisation est pertinente pour le BTS

Cette réalisation correspond parfaitement à plusieurs compétences attendues dans la conception et le développement d’applications.

Elle démontre notamment la capacité à :

* exploiter une API distante
* construire une interface utilisateur
* manipuler des données

Le référentiel indique explicitement que les solutions applicatives doivent être capables **d’échanger des données avec des services applicatifs distants**, ce qui correspond exactement à ce type de projet. 

---

# 6 — Compétences mobilisées (SLAM)

Cette RP peut mobiliser plusieurs compétences importantes.

### Exploiter les technologies Web

* HTTP
* JSON
* appels API

---

### Développer une interface utilisateur

* affichage dynamique
* interaction utilisateur

---

### Exploiter des composants logiciels

* frameworks frontend
* bibliothèques graphiques

---

### Tester une solution applicative

* vérification des réponses
* gestion des erreurs

---

### Documenter une solution

* documentation utilisateur
* documentation technique

---

# 7 — Points forts de cette RP

Cette réalisation possède plusieurs avantages pédagogiques.

### Très réaliste

La majorité des applications web modernes sont :

**des interfaces consommant des API**.

---

### Facile à démontrer

Pendant une soutenance ou dans un portfolio on peut montrer :

* les appels API
* l’affichage dynamique

---

### Visuellement valorisant

Contrairement à une API seule, une interface permet de montrer :

* design
* interaction
* ergonomie

---

### Compatible avec d’autres RP

Cette réalisation peut facilement être liée à :

* une **API développée par l’étudiant**
* une **base de données existante**

On peut ainsi produire **plusieurs RP à partir d’un même projet**.

---

# 8 — Ce qu’il faut valoriser dans le portfolio

Pour que la RP soit convaincante, il faut insister sur plusieurs éléments.

---

## 1 — Le besoin

Expliquer :

* pourquoi une interface est nécessaire
* quels utilisateurs sont concernés

---

## 2 — L’architecture

Illustrer :

```
Frontend → API → Base de données
```

---

## 3 — Les appels API

Exemple :

```javascript
fetch("https://api.example.com/users")
```

---

## 4 — L’affichage dynamique

Exemple :

* tableau
* cartes
* graphiques

---

## 5 — La gestion des erreurs

exemples :

* API indisponible
* erreur réseau
* données invalides

---

# 9 — Améliorations possibles (bonus)

Les étudiants peuvent enrichir la RP avec des fonctionnalités supplémentaires.

---

### recherche dynamique

exemple :

champ de recherche filtrant les résultats.

---

### tri

par :

* date
* popularité
* nom

---

### pagination

chargement progressif des données.

---

### graphiques

exemple :

* statistiques
* évolution

---

### cache

pour limiter les appels API.

---

# 10 — Durée estimée

Selon les fonctionnalités :

* **minimum : 1 à 2 jours**
* **version complète : 3 à 5 jours**
