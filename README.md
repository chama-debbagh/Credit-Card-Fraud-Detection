# Credit-Card-Fraud-Detection
# 💳 Détection de Fraude Bancaire avec Machine Learning

Projet réalisé dans le cadre d’un apprentissage de Data Science. L’objectif est de détecter automatiquement les transactions frauduleuses à l’aide de modèles supervisés de classification.

---

## 📂 Dataset

- Source : [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- 284 807 transactions
- 30 features PCA (anonymisées) + montant (`Amount`) + cible (`Class`)
- Données fortement déséquilibrées : 0 = normal, 1 = fraude

---

## ⚙️ Méthodologie

- Nettoyage et normalisation (`StandardScaler`)
- Suppression de la colonne `Time`
- Équilibrage des classes avec **SMOTE**
- Séparation train/test avec **stratification**
- Entraînement de 3 modèles :
  - Régression Logistique
  - Random Forest
  - XGBoost
- Évaluation : `Precision`, `Recall`, `F1-score`, `ROC AUC`

---

## 🤖 Modèles et Résultats

| Modèle             | Recall (fraude) | Precision (fraude) | F1-score | ROC AUC |
|--------------------|------------------|---------------------|----------|---------|
| LogisticRegression | 0.92             | 0.06                | 0.11     | 0.9459  |
| RandomForest       | ...              | ...                 | ...      | ...     |
| XGBoost            | 0.90             | 0.20                | 0.32     | 0.9458  |

> XGBoost donne le meilleur compromis entre rappel et précision.

---

## 📈 Exemple de visualisations

- Distribution des montants
- Répartition des classes
- Matrice de confusion
- Importance des variables

---

## 🛠️ Stack technique

- Python
- Pandas, NumPy
- Scikit-learn
- imbalanced-learn (SMOTE)
- XGBoost
- Seaborn, Matplotlib

---

## 📁 Structure du projet
---

## 🧠 Auteur

Chama Debbagh  
Étudiante en Data Science – Juin 2025  
Projet à fort impact métier, appliqué à un contexte réel (assurances/banques)


