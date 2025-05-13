# 🍋 Classification des maladies de la mangue avec Stacking et Deep Learning

Ce projet a été réalisé dans le cadre d’un défi scolaire. Il vise à classifier automatiquement les maladies affectant les feuilles de manguiers à partir d’images, en combinant les approches de **deep learning** pour l’extraction de caractéristiques visuelles et d’**apprentissage automatique** (stacking) pour la classification.

## 🎯 Objectif
Détecter et classer automatiquement les maladies de la mangue parmi les catégories suivantes :
- Alternaria
- Anthracnose
- Black Mould Rot
- Healthy
- Stem End Rot

## 🛠️ Méthodologie

### 1. 📷 Prétraitement des données
- Chargement des images du dataset `SenMangoFruitDDS_original`
- Redimensionnement des images (224x224)
- Augmentation des données
- Encodage des labels

### 2. 🧠 Extraction des caractéristiques
- Utilisation du modèle pré-entraîné **Restnet50** (sans la couche de classification)
- Extraction des *features* (embeddings) à partir des images

### 3. 🏗️ Classification par Stacking
- Modèles de base utilisés :
  - `LogisticRegression`
  - `RandomForestClassifier`
  - `SVC` (Support Vector Classifier)
- Méta-modèle final : **régression logistique**
- Implémentation avec `StackingClassifier` de `scikit-learn`

### 4. 📊 Évaluation
- Séparation des données : 80% entraînement / 20% test
- Évaluation avec :
  - Matrice de confusion
  - Classification report (accuracy, precision, recall, f1-score)

## 💻 Technologies utilisées
- Python
- TensorFlow / Keras
- Scikit-learn
- Numpy, Pandas
- Matplotlib, Seaborn

## 📁 Contenu du dépôt
- `projet_deep.ipynb` : notebook complet du projet


## 👨‍💻 Auteur
Projet réalisé par **Kamagate Youssouf**, étudiant en data science.

📧 kamagatey25@gmail.com  
📞 +225 0779837708
