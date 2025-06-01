Projet Machine Learning 2025

Ce projet va nous permettre de mettre en place des modèles de régression et de classification, permettant respectivement de prédire le taux de saturation de l'oxygène dans l'eau, et de déduire si une personne est "riche" ou non.

### 1. Classification
Prédiction du pourcentage de saturationdu niveau d'oxygène dans de l'eau de mer en fonction de :
- son Ph
- la température de l'eau
- son niveau de chlorophyll
- l'oxygène déjà présent 

### 2. Régression
Prédiction du niveau de richesse d'une personne, en fonction de : 
- son âge
- son statut marital 
- son nombre d'heures par semaine
- son gain et perte de capital
- son  iveau d'éducation

---

## Structure du projet

### data/
- `adult.csv` : Données sur des personnes
- `water_quality.csv` : Données sur l'état d'une mer/océan

### Notebooks/
- `classification_2.ipynb` : Modèles pour cibles binaires  
- `Regression.ipynb` : Modèles pour cibles continues  

### Autres fichiers
- `environment_classification.yml` : Dépendances Conda
- `environment_classification.yml` : Dépendance Conda
- `README.md` : Présentation du projet  

---

## Installation et lancement

```bash
conda env create -f environment_classification.yml
conda env create -f environment-regression.yml
conda activate Projt_machine_learning_2
```

## Méthodologie Machine Learning

Le deux projets reposent sur des méthodes de machine learning supervisé : 

### Étapes principales

- Séparation des données en jeu d'entraînement / validation
- Imputation des valeurs manquantes (médiane ou constante)
- Encodage des variables catégorielles (OneHotEncoder)
- Standardisation des variables numériques (StandardScaler)
- Sélection de features pertinentes selon la cible
- Validation croisée (cross-validation à 5 folds)
- Évaluation des modèles avec des métriques adaptées

### Évaluation

- Classification : `accuracy`, `Courbe ROC`, `Matrice de confusion`
- Régression : `MAE`, `MSE`, `R²`

### Modèles testés

#### Classification :
- `BaggingClassifier` (méthode ensembliste)
- `AdaBoostClassifier` (méthode ensembliste)
- `SupportVectorMachine` 
- `SGDClassifier` (non vu en cours, descente de gradient)

#### Régression :
- `RandomForestRegressor` (méthode ensembliste)
- `GradientBoostingRegressor` (méthode ensembliste)
- `DecisionTreeRegressor` (Support Vector Regression)
- `GaussianProcessRegressor` (non vu en cours)


## Par 

**LAPORTE Martint**  
Étudiant en 4e année à l’ESEO (Angers) 
