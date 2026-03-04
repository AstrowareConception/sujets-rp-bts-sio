# RP n°7 — Automatisation d’une tâche métier par script

## 1 — Description de la réalisation professionnelle

Dans de nombreuses organisations, certaines tâches informatiques sont répétitives :

* traitement de fichiers
* génération de rapports
* analyse de données
* sauvegardes
* transformation de données

Ces tâches peuvent être automatisées grâce à des **scripts**.

Dans cette réalisation professionnelle, l’étudiant développe **un script permettant d’automatiser une tâche technique ou métier**, qui était auparavant réalisée manuellement.

Le script peut par exemple :

* analyser des données
* transformer des fichiers
* générer des rapports
* collecter des informations
* automatiser un processus technique

Ce type de réalisation est très réaliste, car l’automatisation est une pratique courante dans les métiers de l’informatique.

Dans le référentiel du BTS, ces activités correspondent notamment à la **mise en œuvre de solutions techniques permettant d’améliorer l’exploitation ou le fonctionnement d’un service informatique**. 

---

# 2 — Exemple de contexte professionnel

Dans une organisation, certaines opérations sont réalisées manuellement par les utilisateurs ou les administrateurs.

Par exemple :

* analyser un fichier de logs
* produire un rapport
* transformer des données
* récupérer des informations sur plusieurs systèmes

Ces tâches peuvent être longues et sources d’erreurs.

Une solution consiste donc à **automatiser ces opérations via un script**.

---

# 3 — Exemples concrets de réalisations possibles

## Exemple 1 — Script d’analyse de logs

Contexte :
Une application produit des logs volumineux.

Objectif :

analyser automatiquement les logs pour identifier les erreurs.

Fonctionnalités du script :

* lecture du fichier log
* détection des erreurs
* génération de statistiques

Exemple de résultat :

```id="s8p26j"
Nombre total d'erreurs : 12
Erreurs de connexion : 5
Erreurs API : 7
```

---

## Exemple 2 — Génération automatique d’un rapport

Contexte :
Une entreprise doit produire régulièrement un rapport d’activité.

Le script :

* récupère les données
* génère un rapport

Exemple :

```id="dt9nxq"
Rapport du 12/03/2026
---------------------
Nombre d'utilisateurs : 235
Nouvelles inscriptions : 18
Commandes : 54
```

---

## Exemple 3 — Conversion de fichiers

Contexte :
Un service reçoit des fichiers dans un format incompatible avec un logiciel interne.

Le script :

* lit les fichiers
* transforme les données
* produit un nouveau fichier.

Exemple :

CSV → JSON.

---

## Exemple 4 — Script de sauvegarde automatisée

Contexte :
Une base de données doit être sauvegardée régulièrement.

Le script :

* exporte la base
* archive les données
* stocke la sauvegarde

---

## Exemple 5 — Script de récupération d’informations

Contexte :
Un administrateur doit régulièrement vérifier l’état de plusieurs services.

Le script :

* interroge des API
* affiche les résultats

---

# 4 — Technologies possibles

Cette RP peut être réalisée avec plusieurs technologies.

---

## Python

Très utilisé pour l’automatisation.

Exemple :

```python id="3x6iqn"
with open("log.txt") as f:
    for line in f:
        if "ERROR" in line:
            print(line)
```

---

## Bash

Très courant sur Linux.

Exemple :

```bash id="qifbws"
grep "ERROR" app.log
```

---

## PowerShell

Très utilisé sous Windows.

Exemple :

```powershell id="akm73f"
Get-Content log.txt | Select-String "ERROR"
```

---

## JavaScript (Node.js)

Peut être utilisé pour :

* traitement de fichiers
* scripts automatisés.

---

# 5 — Ce que l’étudiant doit produire

Pour que la RP soit exploitable dans le portfolio, plusieurs éléments doivent être fournis.

---

## Script

programme complet permettant d’automatiser la tâche.

---

## Exemple de données

fichiers d’entrée.

---

## Résultat produit

exemple :

* rapport
* fichier transformé
* statistiques

---

## Documentation technique

explication :

* fonctionnement du script
* utilisation
* paramètres

---

## Tests

exemples :

* exécution du script
* résultats obtenus

---

# 6 — Pourquoi cette réalisation est pertinente pour le BTS

Cette RP correspond parfaitement à des activités professionnelles réelles :

* automatisation de tâches
* traitement de données
* amélioration d’un processus

Elle démontre la capacité à **identifier un besoin technique et proposer une solution automatisée**, ce qui est une compétence importante dans les métiers de l’informatique.

---

# 7 — Compétences mobilisées (SLAM)

Cette RP peut mobiliser plusieurs compétences.

---

### Concevoir une solution technique

identifier une tâche à automatiser.

---

### Développer un programme

écriture du script.

---

### Exploiter des données

lecture et traitement de fichiers.

---

### Tester une solution

vérification du résultat.

---

### Documenter une solution

explication du fonctionnement.

---

# 8 — Points forts de cette RP

### Très réaliste

L’automatisation est très fréquente en entreprise.

---

### Rapide à produire

Un script utile peut être développé en peu de temps.

---

### Facile à expliquer

On peut facilement montrer :

* le problème
* la solution

---

### Facile à intégrer dans un projet existant

Le script peut compléter :

* une application
* un service
* une analyse de données

---

# 9 — Ce qu’il faut valoriser dans le portfolio

Pour rendre la RP convaincante, il faut mettre en avant :

---

## le problème initial

tâche répétitive.

---

## la solution

script automatisé.

---

## le fonctionnement

exemple d’exécution.

---

## les résultats

rapport ou fichier produit.

---

# 10 — Améliorations possibles (bonus)

Les étudiants peuvent enrichir la RP avec plusieurs fonctionnalités.

---

### interface CLI

paramètres du script.

---

### planification automatique

exécution régulière.

---

### génération de graphiques

visualisation des données.

---

### export vers différents formats

PDF, CSV, JSON.

---

# 11 — Durée estimée

* **version simple : 1 jour**
* **version complète : 2 à 3 jours**
