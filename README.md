
# 🔥 Algerian Forest Fire Prediction using Machine Learning

A complete end-to-end **data science project** that explores and models the **Algerian Forest Fires dataset** using **Linear** and **Polynomial Regression**, feature engineering, cross-validation, and advanced data analysis techniques.

---

## 📌 Project Overview

This project focuses on predicting forest fires in Algeria using meteorological and fire weather indices. The goal is to build accurate regression models and evaluate them using cross-validation to ensure reliability and generalization.

---

## 📁 Dataset

- **Source**: Kaggle 

The dataset contains **weather measurements** and **fire indices** across two regions in Algeria (Region 0 and Region 1), with **target label: fire occurrence (Classes)**.

---

## 📊 Project Pipeline

### 1. 📥 Data Loading & Cleaning
- Combined two regional datasets into one
- Labeled regions and encoded categorical variables

### 2. 📊 Exploratory Data Analysis (EDA)
- Density plots for all features
- Heatmaps for correlation
- Monthly fire occurrence analysis
- Outlier detection using boxplots

### 3. 🧹 Feature Engineering
- Label encoding for 'Classes'
- Feature correlation filtering
- Feature scaling with `StandardScaler`

### 4. 🔁 Model Building with Pipelines
- Linear Regression (Baseline)
- Polynomial Regression (degree = 2, 3, 4)

### 5. 🧠 Cross-Validation
- Applied **5-fold cross-validation**
- Compared **R² Scores** and **standard deviations**

### 6. 📈 Evaluation Metrics
- R² Score
- Cross-validation mean & std
- Residual analysis

---

## 🚀 Results Snapshot

| Model                  | Mean R² Score | Std Dev |
|------------------------|---------------|---------|
| Linear Regression      | **0.9674**     | 0.0362  |
| Polynomial (Degree = 2)| *Try in notebook* | *Tunable* |

✅ Linear Regression showed high accuracy and consistent performance across all folds. Polynomial models showed similar or improved performance with careful tuning.

---

## 🧠 Key Concepts Applied

- `Pipeline` from Scikit-learn  
- `PolynomialFeatures` for non-linear terms  
- `cross_val_score` for model reliability  
- `StandardScaler` for scaling  
- Custom feature selection function

---

## 📌 Libraries Used

```python
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
