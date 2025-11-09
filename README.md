# Projet Séries Temporelles – David Delgado

## Présentation du projet
Ce dépôt contient deux notebooks Jupyter retraçant l’évolution complète du projet d’analyse et de modélisation de séries temporelles, du traitement initial des données jusqu’à la prévision finale.
L'objectif est de partir d'une série brute, la comprendre, la transformer, tester sa stationnarité, puis construire et comparer plusieurs modèles de prévision.

Deux notebooks structurent la démarche :

1. **TP_Précedent_time_series_David_DELGADO.ipynb**  
   Analyse exploratoire et construction des briques fondamentales de traitement des séries temporelles.

2. **TP_Final_time_series_David_DELGADO.ipynb**  
   Approfondissement de la modélisation, sélection des modèles, prévisions finales et mise en forme pédagogique.

---

## Objectifs pédagogiques

- Comprendre les spécificités des séries temporelles (tendance, saisonnalité, bruit).
- Savoir transformer une série pour la rendre exploitable (log, différenciation, moyenne mobile, décalages).
- Vérifier la stationnarité (test ADF).
- Identifier et ajuster des modèles ARIMA / SARIMA (et dérivés).
- Utiliser les critères d’information (AIC, BIC) pour comparer les modèles.
- Produire et interpréter des prévisions sur plusieurs périodes futures.
- Illustrer la démarche complète de bout en bout dans un cadre reproductible.

---

## Contenu des notebooks

### TP_Précedent_time_series_David_DELGADO.ipynb

Notebook de construction et de compréhension :

- Chargement et mise en forme de la série temporelle.
- Indexation temporelle et manipulation de base.
- Transformations :
  - Passage en log.
  - Lissage et moyennes mobiles.
  - Décalages temporels (différences).
- Gestion des valeurs manquantes induites par les transformations.
- Premiers tests de stationnarité (ADF).
- Introduction aux premiers modèles ARIMA / SARIMA sur la série des broilers.

### TP_Final_time_series_David_DELGADO.ipynb

Notebook final, structuré comme un support de cours complet :

- Rappel du contexte : consommation de poulet (broilers) comme cas d'étude.
- Analyse visuelle détaillée :
  - Tendances globales.
  - Changements de régime et comportements saisonniers.
  - Zoom sur certaines périodes.
- Approche modélisation :
  - Construction et comparaison de modèles ARIMA et SARIMA.
  - Utilisation des critères AIC pour sélectionner les paramètres.
  - Vérification des résidus et validité du modèle.
  - Introduction à SARIMAX / variables exogènes (structure prête).
  - Introduction à Prophet comme alternative de modélisation.
- Génération de prévisions sur plusieurs périodes futures.
- Visualisation des intervalles de confiance et interprétation des résultats.

---

## Jeu de données

- Série temporelle : consommation de poulet (broilers).
- Données agrégées dans le temps (fréquence régulière).
- Utilisée comme fil conducteur pour illustrer toutes les étapes :
  préparation → tests → modélisation → prévisions.

---

## Dépendances nécessaires

Installer les bibliothèques suivantes avant d'exécuter les notebooks :

```bash
pip install pandas numpy matplotlib statsmodels jupyter
```

Pour les parties avancées (recommandé) :

```bash
pip install pmdarima prophet scipy
```

> Remarque : selon l’environnement, le package Prophet peut être installé sous le nom `prophet` ou `cmdstanpy` + `prophet`. Vérifier la documentation officielle si nécessaire.

---

## Exécution

1. Cloner le dépôt :

```bash
git clone https://github.com/daviddelgadop/timeseries.git
cd timeseries
```

2. Lancer Jupyter :

```bash
jupyter notebook
```
ou

```bash
jupyter lab
```

3. Ouvrir et exécuter dans l’ordre :
   - `TP_Précedent_time_series_David_DELGADO.ipynb`
   - `TP_Final_time_series_David_DELGADO.ipynb`

---

## Résultats attendus

- Identification d’un (ou plusieurs) modèles pertinents pour la série étudiée.
- Prévisions lisibles et cohérentes avec le comportement historique.
- Support pédagogique clair montrant :
  - la logique des transformations,
  - la construction des modèles,
  - la lecture critique des sorties (AIC, graphiques, résidus, intervalles).

---

## 👤 Auteur

**David Delgado**  
IA School – Master 2025‑2027  
*Modélisation et prévision de séries temporelles en Python*
