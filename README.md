# Toxic Comments Detection

## 🎯 Résultats
- **88.67% de précision** avec XGBoost sur 160 554 commentaires
- 6 modèles comparés — 4 dépassent le seuil cible de 85%
Ce projet est un script Python d'apprentissage automatique conçu pour détecter et évaluer la toxicité dans des commentaires (NLP). Il entraîne, compare, et combine plusieurs modèles d'intelligence artificielle pour identifier et classifier le degré et les raisons de la toxicité dans un texte.

## 🚀 Fonctionnalités 

- **Nettoyage de texte avancé (NLP)** : Suppression des abréviations, uniformisation du texte et retrait des caractères spéciaux.
- **Vectorisation TF-IDF** : Analyse des mots fréquents.
- **Équilibrage des classes (SMOTE)** : Gestion des déséquilibres entre commentaires toxiques et non toxiques.
- **Comparaison de 6 Modèles de Machine Learning** : 
  - XGBoost (optimisé)
  - Random Forest
  - Linear SVC
  - Decision Tree
  - Neural Network (MLP)
  - Ensemble Model (Soft Voting combinant XGBoost, SVC et MLP)
- **Scoring (1 à 10)** : Évaluation des commentaires selon un score de gravité précis allant de "Non Toxique" à "Extrêmement Toxique".
- **Visualisations Data (Matplotlib/Seaborn)** : Nuages de mots, matrice de confusion, et graphiques de comparaison des performances (Accuracy).

## 🗂 Les données (Datasets)
Le projet repose sur 2 fichiers CSV qui **ne sont pas inclus dans ce dépôt GitHub** car ils sont trop volumineux :
1. `train.csv` et `train.csv.zip`
2. `youtoxic_english_1000.csv`

Veillez à ajouter ces fichiers à la racine du projet avant d'exécuter l'application.

## 🛠 Installation et Lancement

1. Cloner le repo :
   ```bash
   git clone <Lien_de_votre_repo>
   cd Projet
   ```

2. Installer les bibliothèques requises :
   ```bash
   pip install pandas numpy matplotlib seaborn wordcloud scikit-learn xgboost imbalanced-learn
   ```

3. Exécuter le script :
   ```bash
   python3 toxic-com-detection.py
   ```
