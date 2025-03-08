# ML Pipeline for Airfoil Noise Prediction

## Description
Le projet "ML Pipeline for Airfoil Noise Prediction" vise à créer un pipeline d'apprentissage automatique complet pour prédire le niveau sonore généré par des profils aérodynamiques (airfoils) en fonction de différentes caractéristiques. Ce projet utilise un ensemble de données modifié de NASA, connu sous le nom de *Airfoil Self-Noise Dataset*, pour nettoyer, transformer et entraîner un modèle de régression. 

Le pipeline développé dans ce projet suit une approche en quatre étapes :
1. **ETL** : Préparation et nettoyage des données.
2. **Machine Learning** : Création d'un modèle de régression pour prédire le niveau sonore.
3. **Évaluation du modèle** : Utilisation de mesures de performance pour évaluer la précision du modèle.
4. **Persistance du modèle** : Sauvegarde du modèle pour une utilisation future.

## Objectifs
- Charger un dataset CSV et le nettoyer (suppression des doublons et des valeurs nulles).
- Créer un pipeline d'apprentissage automatique pour prédire le niveau sonore (`SoundLevel`).
- Évaluer la performance du modèle avec des métriques appropriées.
- Sauvegarder le modèle entraîné pour une utilisation ultérieure.

## Structure du projet

### Dossiers et fichiers principaux :
- **data/** : Contient les fichiers de données brutes et nettoyées (au format `.csv` et `.parquet`).
- **src/** : Code source pour le traitement des données, l'entraînement du modèle, l'évaluation et la persistance du modèle.
  - **etl.py** : Script pour effectuer les activités ETL (chargement, nettoyage, transformations).
  - **train_model.py** : Script pour créer et entraîner le modèle de Machine Learning.
  - **evaluate.py** : Script pour évaluer la performance du modèle.
  - **persist_model.py** : Script pour sauvegarder et charger le modèle.
- **models/** : Contient les modèles sauvegardés.
- **notebooks/** : (Optionnel) Jupyter notebooks pour l'exploration et les tests intermédiaires.

### Technologies utilisées :
- **Python** : Langage principal du projet.
- **Pandas** et **NumPy** : Manipulation des données.
- **Scikit-learn** : Création et évaluation du modèle de Machine Learning.
- **PySpark / Spark ML** : Traitement distribué et apprentissage automatique à grande échelle.
- **Apache Parquet** : Format de stockage des données nettoyées.
  
## Installation

### Prérequis :
1. Python 3.7 ou supérieur.
2. Installe les dépendances avec `pip` :

```bash
pip install -r requirements.txt
