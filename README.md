# 🫀 Heart Disease Prediction: Classification Summary

This project builds a complete classification pipeline to predict heart disease using structured medical data. It includes EDA, preprocessing with pipelines, multiple model comparisons, and final interpretation using feature importance.

- [Google Colab Notebook](https://colab.research.google.com/drive/1iQEdq75flEdsWjRvhsOlINi9Fob26P-R?usp=sharing)
- [Dataser Source](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data)

## 📊 What the Project Covers

### 1. Data Loading & Cleaning

* Downloaded via Kaggle Hub.
* Inspected structure, types, and missing values.
* Dataset includes clinical features like chest pain type, max heart rate, vessels, and cholesterol.

### 2. Exploratory Data Analysis (EDA)

* Target distribution is relatively balanced.
* Key observations:

  * Lower max heart rate often corresponds to heart disease.
  * Chest pain type strongly differentiates classes.
  * Correlation heatmap highlights medically relevant patterns.

### 3. Preprocessing with Pipelines

* Numerical features: imputation + scaling.
* Categorical features: imputation + one-hot encoding.
* Combined via ColumnTransformer.
* Train-test split with stratification to preserve class balance.

### 4. Model Building

Four models trained using the same preprocessing pipeline:

* Logistic Regression (baseline)
* Random Forest (ensemble)
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)

### 5. Evaluation

* Metrics: accuracy, precision, recall, F1-score, confusion matrix.
* SVM and Random Forest performed best overall.
* Random Forest achieved strong accuracy and consistent detection across classes.

### 6. Feature Importance

Random Forest identified key predictors:

* `ca` (major vessels)
* `thalach` (max heart rate)
* `thal` (thalassemia)
* `cp` (chest pain type)

### ⭐ Conclusion

This project demonstrates a full classification workflow:

* Solid EDA
* Clean preprocessing with pipelines
* Multiple model comparison
* Clear, interpretable results

Random Forest and SVM emerged as the strongest models, with clinically meaningful feature insights that align with real-world medical reasoning.
