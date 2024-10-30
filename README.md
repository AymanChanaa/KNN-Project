# Prédiction de la Présence de Diabète avec K-Nearest Neighbors (KNN)

Ce projet développe un modèle de **classification** pour prédire la présence de diabète chez des patients à partir de diverses caractéristiques médicales. Nous utilisons l'algorithme **K-Plus Proches Voisins** (K-Nearest Neighbors, KNN) pour classer les patients en fonction de leur probabilité d'avoir ou non le diabète.

## Dataset

Le jeu de données utilisé est `diabetes.csv`, qui contient des informations médicales de patients anonymisés avec les caractéristiques suivantes :

- **Pregnancies** : Nombre de grossesses.
- **Glucose** : Niveau de glucose dans le sang.
- **BloodPressure** : Pression artérielle.
- **SkinThickness** : Épaisseur de la peau (mm).
- **Insulin** : Niveau d'insuline.
- **BMI** : Indice de masse corporelle (poids en kg / taille en m²).
- **DiabetesPedigreeFunction** : Fonction d'hérédité du diabète.
- **Age** : Âge du patient.
- **Outcome** : Présence de diabète (0 : Non, 1 : Oui).

## Objectif

L'objectif de ce projet est de :
1. **Construire un modèle de classification** pour prédire la présence de diabète chez un patient.
2. **Entraîner et évaluer** ce modèle en utilisant l'algorithme des K-Plus Proches Voisins (KNN).
3. **Optimiser** le choix du paramètre **K** pour améliorer la performance du modèle.

## Prérequis

- Python 3.11
- Jupyter Notebook
- Bibliothèques Python :
  - pandas
  - numpy
  - scikit-learn
  - matplotlib

## Installation des dépendances

Pour installer les bibliothèques nécessaires, exécutez la commande suivante :

```bash
pip install pandas numpy scikit-learn matplotlib
```

## Structure du Projet
diabetes.csv : Fichier de données contenant les informations médicales des patients.
diabetes_knn.ipynb : Notebook Jupyter contenant le code pour charger les données, entraîner le modèle KNN, et évaluer les résultats.
Explication du Notebook
Chargement des Données : Utilisation de pandas pour charger le jeu de données à partir du fichier diabetes.csv.

## Prétraitement des Données :

Gestion des valeurs manquantes et normalisation des données pour optimiser la performance de KNN.
Sélection des caractéristiques les plus importantes pour la classification.

## Division des Données :

Séparation des données en ensemble d'entraînement et de test avec **train_test_split** de sklearn.model_selection.

## Implémentation du Modèle KNN :

Entraînement d’un classificateur KNN avec KNeighborsClassifier de sklearn.neighbors.

Optimisation du paramètre K pour obtenir les meilleures performances en utilisant la validation croisée.

## Évaluation du Modèle :

Utilisation de métriques comme la précision, la Matrice de Confusion, et la Score F1 pour évaluer la performance du modèle.

Affichage de la matrice de confusion pour analyser les prédictions correctes et incorrectes.

## Utilisation :

Clonez ce dépôt et ouvrez le fichier diabetes_knn.ipynb dans Jupyter Notebook.

Exécutez chaque cellule dans l'ordre pour importer les données, entraîner le modèle, et visualiser les résultats.

## Exemple de Résultat : 

Le modèle KNN permet de prédire avec une certaine précision la présence ou non de diabète chez les patients. Les résultats de l'évaluation montrent la capacité du modèle à bien classifier les individus et l'impact du choix du paramètre K sur les performances.

## Conclusion :
Ce projet illustre comment utiliser l'algorithme K-Plus Proches Voisins pour un problème de classification médical. La prédiction de la présence de diabète peut fournir des indications utiles pour une détection précoce, et l'algorithme KNN est adapté aux ensembles de données de taille modérée grâce à sa simplicité et son efficacité.
