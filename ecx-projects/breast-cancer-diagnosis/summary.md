# 🩺 Breast Cancer Diagnostics

## 🧠 Project Overview
This project involved building a machine learning model to classify breast cancer tumors as **malignant** or **benign** based on diagnostic features. The goal was to identify the best-performing model for accurate prediction, while analyzing important features that contribute to diagnosis.

---

## ⚙️ Model Description

### 🧪 Algorithms Used:
1. **DecisionTreeClassifier** (Baseline Model)
2. **RandomForestClassifier** (Preferred Model)

### 🔍 Preprocessing:
- The `id` column was dropped to prevent bias in model predictions.
- The target column, `diagnosis`, was encoded numerically for processing.
- Features with low impact (as observed in analysis and feature importance) were dropped to improve model efficiency.

---

## 📊 Evaluation

### 📈 Metrics:
- `DecisionTreeClassifier` yielded an **F1 Macro Avg** of **0.93**
- `RandomForestClassifier` improved performance to an **F1 Macro Avg** of **0.96**
- Confusion matrices showed that the **Random Forest** performed better overall without hyperparameter tuning.

### 🏆 Best Model:
- **RandomForestClassifier** was selected as the final model due to higher precision, recall, and F1-score across both classes.

---

## 🔎 Feature Importance

### Most Important Features:
- **Decision Tree:** `concave points_mean`
- **Random Forest:** `area_complexity`

### Key Shared Features:
Both models highlighted the following as strong predictors:
- `concave points_worst`
- `perimeter_worst`
- `concave points_mean`
- `radius_worst`

These features consistently influenced the prediction of tumor malignancy.

---

## 📈 Exploratory Analysis

Grouped visualizations based on the `diagnosis` label revealed:
- Columns with suffix `_se` had minimal impact on target classification.
- This was confirmed by both models’ feature importance analysis.

As a result, these features were dropped to streamline model training and reduce noise.

---

## 🧠 Takeaway
A well-preprocessed dataset combined with ensemble methods like Random Forest can yield robust medical classification systems. The focus on feature impact helped in simplifying the model while retaining high accuracy.
