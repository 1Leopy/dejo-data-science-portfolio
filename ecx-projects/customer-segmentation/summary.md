# 🛍️ Customer Segmentation with K-Means Clustering

## 🧠 Project Overview
This project focused on segmenting a mall's customers based on their spending habits and income levels. The goal was to help the business identify customer types and develop strategies to better engage, retain, or assist each group.

---

## 👥 Customer Demographics

- **Gender Distribution:** 56% Female, 44% Male
- **Age Distribution:**  
  - Young Adults (18–35): 89 customers  
  - Adults (35–55): 81 customers  
  - Older Adults (55–70): 28 customers  
- **Income Distribution:**  
  - First Class Earners (>$70k) and Middle Class ($40k–$70k) = 76.2%  
  - Lower Class (<$40k) = 23.7%

---

## ⚙️ Model Description

### 🔄 Pipeline Workflow
- Used a `Pipeline` and `ColumnTransformer` for clean preprocessing.
- Applied `StandardScaler` to numerical columns.

### 📈 Model Used
- **KMeans Clustering**
- Features: `Annual Income (k$)` and `Spending Score (1–100)`

### 🔍 Optimal K Selection
- Used both **Elbow Method (Inertia vs K)** and **Silhouette Score** to choose the number of clusters.
- Chose **K = 5** based on:
  - Inertia in the range of 50–75
  - Silhouette Score of **0.555**
  - Business logic: 5 customer personas felt reasonable for real-world behavioral segmentation

---

## 🔎 Cluster Descriptions

| Cluster | Description | Strategy |
|--------|-------------|----------|
| **0 (Engage)** | Mid-income, balanced spenders (~40% of customer base) | Maintain product quality and affordability |
| **1 (Retain)** | High-value customers spending within means | Retain through loyalty programs and special care |
| **2 (Manage)** | Low-income, high spenders | Support with financial literacy or safer credit programs |
| **3 (Encourage)** | High-income, low spenders | Stimulate with tailored deals and incentives |
| **4 (Assist)** | Low-income, low spenders | Provide more budget-friendly products and services |

---

## 📌 Key Insights

- The clustering was successful in revealing actionable customer groups with distinct behavior patterns.
- Pipeline and scaling helped maintain consistency in feature engineering.
- This analysis can directly inform marketing, product, and financial strategies.

---

## 💡 Takeaway
Combining clustering with domain knowledge leads to high-impact customer insights. The five segments offer a solid foundation for tailored business strategies.
