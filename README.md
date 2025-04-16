# Credit-Card-Fraud-Detection
# 💳 Détection de Fraude Bancaire avec Machine Learning

---

## Dataset

- Source () : [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Le fichier `creditcard.csv` n'est pas inclus dans ce dépôt (taille > 100 Mo).  
Vous pouvez le télécharger directement depuis Kaggle.
---

## Méthodologie

1. Nettoyage des données et normalisation via `StandardScaler`
2. Suppression de la variable `Time`, non pertinente pour le modèle
3. Équilibrage des classes fortement déséquilibrées avec la méthode **SMOTE**
4. Séparation du jeu de données en `train/test` avec stratification
5. Entraînement de trois modèles :
   - Régression Logistique
   - Random Forest
   - XGBoost
6. Évaluation des performances via :
   - `Precision`
   - `Recall`
   - `F1-score`
   - `ROC AUC`

---

## Modèles et Résultats

 Modèle             | Recall (fraude)  | Precision (fraude)  | F1-score  | ROC AUC|
____________________|__________________|_____________________|__________|_________|
 LogisticRegression | 0.92             | 0.06                | 0.11     | 0.9459  |
 RandomForest       | ...              | ...                 | ...      | ...     |
 XGBoost            | 0.90             | 0.20                | 0.32     | 0.9458  |

> XGBoost donne le meilleur compromis entre rappel et précision.

---

## Exemple de visualisations

- Distribution des montants de transaction
- Répartition des classes (fraudes vs normales)
- Matrice de confusion
- Importance des variables selon le modèle

---

## Stack technique

- Python
- Pandas, NumPy
- Scikit-learn
- imbalanced-learn (SMOTE)
- XGBoost
- Seaborn, Matplotlib

---


