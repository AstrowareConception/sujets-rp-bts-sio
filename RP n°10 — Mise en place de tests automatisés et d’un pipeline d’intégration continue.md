# RP n°10 — Mise en place de tests automatisés et d’un pipeline d’intégration continue

## 1 — Description de la réalisation professionnelle

Dans les environnements professionnels modernes, les équipes de développement doivent garantir la **qualité et la fiabilité des applications**.

Pour cela, plusieurs pratiques sont utilisées :

* tests automatisés
* intégration continue
* vérification automatique du code

Les tests automatisés permettent de vérifier que les fonctionnalités d’une application fonctionnent correctement.

L’intégration continue consiste à **exécuter automatiquement ces tests lorsqu’une modification est apportée au code**.

Dans cette réalisation professionnelle, l’étudiant met en place :

* des tests automatisés pour une application
* un pipeline d’intégration continue permettant d’exécuter ces tests automatiquement

Cette réalisation peut être appliquée à **une application existante développée dans une autre RP**.

Elle correspond à une pratique professionnelle essentielle visant à **assurer la qualité et la maintenabilité d’une solution applicative**.

---

# 2 — Exemple de contexte professionnel

Une application a été développée mais aucun mécanisme ne permet de vérifier automatiquement son bon fonctionnement.

Chaque modification du code peut potentiellement introduire :

* des erreurs
* des régressions
* des dysfonctionnements

Une solution consiste à mettre en place :

* des tests automatisés
* un système exécutant ces tests automatiquement lors des modifications du code.

---

# 3 — Exemples concrets de réalisations possibles

## Exemple 1 — Tests automatisés pour une API

Application existante :

API REST.

Tests réalisés :

* test de création d’utilisateur
* test de récupération de données
* test d’erreur

Exemple :

```id="5nac1o"
GET /users → status 200
POST /users → création réussie
```

---

## Exemple 2 — Tests d’une application web

Application existante :

site web.

Tests possibles :

* affichage d’une page
* validation d’un formulaire
* vérification d’un résultat

---

## Exemple 3 — Tests unitaires d’une application

Application existante :

programme comportant plusieurs fonctions.

Tests :

* vérification des calculs
* validation des entrées

---

## Exemple 4 — Pipeline d’intégration continue

Contexte :

le projet est hébergé sur GitHub ou GitLab.

Lorsqu’un développeur pousse du code :

* les tests sont exécutés automatiquement
* le résultat est affiché

---

# 4 — Architecture du processus

Avant amélioration :

```id="vde5nx"
Développeur → modification du code → déploiement
```

Après amélioration :

```id="37g8vu"
Développeur → commit
        ↓
Pipeline CI
        ↓
Tests automatisés
        ↓
Validation
```

---

# 5 — Technologies possibles

Cette RP peut être réalisée avec plusieurs outils.

---

## Tests automatisés

Selon le langage utilisé.

### JavaScript

* Jest
* Mocha

---

### Python

* Pytest
* unittest

---

### Java

* JUnit

---

### PHP

* PHPUnit

---

## Intégration continue

Plusieurs plateformes existent.

### GitHub Actions

Exemple :

```yaml id="h7nfq9"
name: tests

on: [push]

jobs:
  test:
    runs-on: ubuntu-latest
```

---

### GitLab CI

---

### Jenkins

---

# 6 — Ce que l’étudiant doit produire

Pour que la RP soit exploitable dans le portfolio, plusieurs éléments doivent être présentés.

---

## Code des tests

fichiers de tests automatisés.

---

## Configuration du pipeline

fichier CI :

```id="k9o71q"
.github/workflows/test.yml
```

---

## Exemples d’exécution

captures montrant :

* tests réussis
* tests échoués

---

## Documentation technique

explication :

* fonctionnement des tests
* pipeline CI

---

## Dépôt Git

le projet doit être versionné.

---

# 7 — Pourquoi cette réalisation est pertinente pour le BTS

Cette RP correspond à des pratiques professionnelles essentielles :

* assurance qualité
* validation automatique du code
* gestion collaborative des projets

Elle démontre que l’étudiant comprend l’importance de **la qualité logicielle et de la maintenance des applications**.

---

# 8 — Compétences mobilisées (SLAM)

Cette RP peut mobiliser plusieurs compétences importantes.

---

### Développer une solution applicative

écriture des tests.

---

### Tester une application

tests unitaires et fonctionnels.

---

### Exploiter un environnement de développement

utilisation d’un outil CI.

---

### Maintenir une solution

détection des erreurs.

---

### Documenter une solution

explication du processus.

---

# 9 — Points forts de cette RP

### Très professionnelle

Les tests automatisés sont utilisés dans presque tous les projets modernes.

---

### Valorise la qualité du code

Elle montre que l’étudiant applique :

* bonnes pratiques
* méthodologies professionnelles.

---

### Facile à intégrer dans un projet existant

Elle peut s’appliquer à :

* une API
* un site web
* un micro-service
* une application desktop

---

### Très appréciée dans un portfolio

Peu d’étudiants montrent ces pratiques.

---

# 10 — Ce qu’il faut valoriser dans le portfolio

Pour rendre la RP convaincante, il faut mettre en avant :

---

## le problème initial

absence de tests.

---

## la solution

tests automatisés.

---

## le pipeline CI

exécution automatique.

---

## les résultats

tests réussis.

---

# 11 — Améliorations possibles (bonus)

Les étudiants peuvent enrichir la RP avec plusieurs éléments.

---

### couverture de code

mesurer les parties testées.

---

### linting automatique

vérification du style du code.

---

### déploiement automatique

CI/CD complet.

---

### badges GitHub

statut des tests.

---

# 12 — Durée estimée

* **version simple : 2 jours**
* **version complète : 3 à 4 jours**
