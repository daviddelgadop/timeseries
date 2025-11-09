# Projet Séries Temporelles – David Delgado

## Présentation du projet
Ce dépôt contient deux notebooks Jupyter retraçant l’évolution complète du projet d’analyse et de modélisation de séries temporelles, du traitement initial des données jusqu’à la prévision finale.

### Notebooks inclus
1. **TP_Initial_time_series_David_DELGADO.ipynb**  
   → Analyse exploratoire, préparation des données, tests de stationnarité, premières modélisations simples.

2. **TP_Final_time_series_David_DELGADO.ipynb**  
   → Modélisation avancée (ARIMA, SARIMA, SARIMAX), évaluation des modèles, prévisions à long terme, interprétation des résultats.

---

## Objectifs pédagogiques
- Comprendre la logique de traitement et de transformation des séries temporelles.  
- Appliquer les tests de stationnarité (ADF, KPSS).  
- Identifier et ajuster les paramètres optimaux des modèles ARIMA / SARIMA.  
- Évaluer les performances via les critères AIC, BIC et la validation visuelle.  
- Produire des prévisions fiables à moyen terme et les interpréter graphiquement.

---

## Dépendances nécessaires

Avant d’exécuter les notebooks, assurez-vous d’installer les bibliothèques suivantes :

```bash
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn jupyter
```

Optionnel :
```bash
pip install pmdarima
```

---

## 📂 Structure du dépôt

```
├── TP_Initial_time_series_David_DELGADO.ipynb
├── TP_Final_time_series_David_DELGADO.ipynb
└── README_Time_Series_David_Delgado_FR.md
```

---

## 🚀 Exécution des notebooks

1. Ouvrir un terminal dans le répertoire du projet.  
2. Lancer Jupyter Notebook ou JupyterLab :

```bash
jupyter notebook
```
ou
```bash
jupyter lab
```
3. Exécuter les cellules dans l’ordre.  
4. Les visualisations (tendances, autocorrélations, prévisions) seront générées automatiquement.

---

## Contenu des notebooks

### **TP Initial**
- Chargement et nettoyage des données
- Visualisation des tendances saisonnières
- Tests ADF et différenciation
- Identification des ordres (p,d,q)
- Premier modèle ARIMA simple

### **TP Final**
- Sélection des meilleurs paramètres (AIC, BIC)
- SARIMA et SARIMAX (prise en compte saisonnalité et variables exogènes)
- Prévisions log-différenciées et reconstruction des valeurs réelles
- Analyse des intervalles de confiance
- Interprétation économique des résultats

---

## Résultats attendus
- Détermination du modèle le plus performant pour la série analysée.
- Prévision fiable sur plusieurs périodes futures (ex : 60 mois).  
- Graphiques clairs montrant la tendance et la qualité d’ajustement.

---

## Auteur
**David Delgado**  
IA School – Master 2025‑2027  
Projet : *Modélisation et prévision de séries temporelles en Python*

