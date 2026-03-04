# RP n°6 — Mise en place d’un système de logs et de monitoring pour une application existante

## 1 — Description de la réalisation professionnelle

Dans les environnements professionnels, les applications évoluent continuellement. Une fois un logiciel déployé, il est nécessaire de pouvoir :

* analyser son fonctionnement
* détecter les erreurs
* comprendre les incidents
* améliorer la qualité du service

Pour cela, les applications produisent des **journaux d’activité (logs)** et peuvent être supervisées par des outils de **monitoring**.

Dans cette réalisation professionnelle, l’étudiant intervient **sur une application déjà existante** afin d’y intégrer un système de :

* journalisation
* analyse des événements
* supervision du fonctionnement

L’application peut être par exemple :

* une API développée lors d’une RP précédente
* un site web
* un micro-service
* un client lourd
* un service interne

L’objectif est d’améliorer la solution existante afin de permettre :

* le diagnostic d’incidents
* l’analyse des erreurs
* l’amélioration de la qualité du service

Cette situation correspond parfaitement à une activité professionnelle réelle, où les développeurs interviennent souvent pour **maintenir ou améliorer une application existante**.

---

# 2 — Exemple de contexte professionnel

## Exemple typique dans un portfolio étudiant

Un étudiant a développé en début d’année :

* une API REST de gestion d’utilisateurs
* ou une application web
* ou un micro-service

Cependant, l’application ne possède **aucun système de suivi des erreurs ou d’analyse du fonctionnement**.

Une évolution est donc demandée :

> mettre en place un système de journalisation et de supervision afin de pouvoir analyser le fonctionnement de l’application et détecter les incidents.

Cette évolution constitue **une réalisation professionnelle autonome**, car elle répond à un besoin technique réel.

---

# 3 — Exemples concrets de réalisations possibles

## Exemple 1 — Ajout de logs à une API existante

Application existante :

API REST développée précédemment.

Évolution réalisée :

* journalisation des requêtes
* journalisation des erreurs
* journalisation des authentifications

Exemple de log :

```text
[INFO] 2026-02-10 10:25:03 - GET /users
[WARNING] 2026-02-10 10:25:07 - Invalid token
[ERROR] 2026-02-10 10:25:10 - Database connection failed
```

---

## Exemple 2 — Analyse des logs d’une application web

Application existante :

site web développé lors d’une autre RP.

Évolution :

* enregistrement des erreurs
* script d’analyse des logs
* statistiques des incidents

Exemple de résultat :

* nombre d’erreurs par jour
* pages les plus consultées

---

## Exemple 3 — Monitoring d’un micro-service

Application existante :

micro-service développé précédemment.

Évolution :

* collecte des métriques
* tableau de bord

Indicateurs surveillés :

* nombre de requêtes
* temps de réponse
* erreurs

---

## Exemple 4 — Système d’alertes

Application existante :

service web interne.

Évolution :

* détection des erreurs critiques
* génération d’alertes

Exemple :

```text
ALERTE : service indisponible
```

---

# 4 — Architecture de la solution

Avant amélioration :

```
Application → Base de données
```

Après amélioration :

```
Application → Logs → Analyse / Monitoring
              ↓
         Base de données
```

---

# 5 — Technologies possibles

Cette RP peut être réalisée avec plusieurs outils.

## Logging intégré dans l’application

Exemples :

* Python → logging
* Java → Log4j
* Node.js → Winston / Morgan
* PHP → Monolog

Exemple :

```python
logging.error("Erreur de connexion à la base de données")
```

---

## Analyse des logs

Possibilités :

* script Python
* dashboard web
* visualisation graphique

---

## Outils de monitoring (optionnel)

* Grafana
* Prometheus
* ELK Stack

---

# 6 — Ce que l’étudiant doit produire

Pour que cette RP soit exploitable dans le portfolio, plusieurs éléments doivent être présentés.

## Code source

modifications apportées à l’application existante :

* ajout de logs
* gestion des erreurs

---

## Fichiers de logs

exemples :

```
app.log
error.log
```

---

## Script ou outil d’analyse

par exemple :

* script Python
* tableau de bord

---

## Documentation technique

explication :

* structure des logs
* événements enregistrés
* utilisation

---

## Tests

simulation d’incidents :

* erreur base de données
* requête invalide
* erreur API

---

# 7 — Pourquoi cette réalisation est pertinente pour le BTS

Cette RP correspond très bien aux situations professionnelles attendues :

* amélioration d’une application existante
* analyse d’incidents
* amélioration de la qualité du service

Dans le référentiel, les solutions applicatives doivent être maintenues et améliorées, notamment par l’analyse des dysfonctionnements et l’évolution de la solution existante. 

---

# 8 — Compétences mobilisées (SLAM)

Cette RP permet de mobiliser plusieurs compétences importantes.

### Maintenance d’une solution applicative

* amélioration d’une application existante

### Analyse d’un dysfonctionnement

* détection d’erreurs
* analyse des logs

### Exploitation des données

* analyse des journaux d’activité

### Tests

* simulation d’incidents

### Documentation technique

* description du système de logs

---

# 9 — Points forts de cette RP

### Réalisation très réaliste

Dans le monde professionnel, une grande partie du travail consiste à :

* améliorer
* maintenir
* superviser

des applications existantes.

---

### Très complémentaire d’un autre projet

Elle peut s’appuyer sur :

* une API
* un site web
* un micro-service

développé précédemment.

---

### Valorise la capacité d’analyse

Elle montre que l’étudiant ne se limite pas au développement mais comprend :

* l’exploitation
* la maintenance

---

### Facile à produire

Cette RP peut être réalisée rapidement tout en restant crédible.

---

# 10 — Ce qu’il faut valoriser dans le portfolio

Pour que la RP soit convaincante, il faut mettre en avant :

### le problème initial

absence de logs.

---

### l’évolution réalisée

ajout du système de journalisation.

---

### les résultats

exemples de logs.

---

### l’amélioration apportée

meilleure capacité de diagnostic.

---

# 11 — Durée estimée

* **version simple : 1 à 2 jours**
* **version complète : 3 à 4 jours**
