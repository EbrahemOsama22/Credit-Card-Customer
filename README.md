

---

## Credit Card Customer Clustering Analysis 💳🔍

An unsupervised machine learning project that segments credit card customers into distinct behavioral groups using the **CC GENERAL** dataset from Kaggle.

📎 **Dataset:** [Kaggle — Credit Card Dataset for Clustering](https://www.kaggle.com/datasets/arjunbhasin2013/ccdata)

---

### 📌 What This Project Does

- **Data Cleaning** — Handles missing values in `CREDIT_LIMIT` and `MINIMUM_PAYMENTS` using **KNN Imputation**, removes duplicates, and drops the non-informative `CUST_ID` column.
- **Outlier Detection** — Detects outliers across all numeric columns using the **IQR method**.
- **Skewness Correction** — Detects and fixes skewed features using **Yeo-Johnson Power Transformation**.
- **Dimensionality Reduction** — Applies **PCA (2 components)** to reduce feature space while preserving ~58% of variance, enabling efficient clustering and visualization.
- **Clustering** — Applies **K-Means** (k=4, selected via Elbow Method) on PCA-transformed data.
- **Cluster Profiling** — Summarizes each cluster's average behavior across all features to derive business insights.
- **Visualization** — 2D PCA scatter plots and cluster size bar charts for clear interpretation.

---

### 📊 Clustering Evaluation Metrics

| Metric | Description |
|---|---|
| **Silhouette Score** | Measures how similar each point is to its own cluster vs others |
| **Davies-Bouldin Index** | Lower = better separated clusters |
| **Calinski-Harabasz Index** | Higher = denser, better-defined clusters |

---

### 🛠️ Tech Stack

`Python` · `Pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Scikit-learn` · `SciPy`

---
