# 📊 End-to-End Sales Analytics & Business Strategy Project
---

## 📝 Project Overview
This project is a comprehensive Data Science study conducted on a Retail Sales dataset sourced from **Kaggle.com**. The core dataset, `sales.csv`, was retrieved from the `data` folder and utilized across three distinct analytical phases. This project covers the entire data pipeline—from initial exploration to predictive modeling and rigorous statistical hypothesis testing. The ultimate goal is to identify profit drivers and provide data-driven strategic recommendations for business growth.

---

## 🚀 Key Project Modules

### 1️⃣ Phase 1: Exploratory Data Analysis (EDA)
* **Objective:** Understand data distributions, identify outliers, and uncover hidden correlations.
* **Key Findings:** The 'Technology' category exhibits the highest volatility but also the strongest profit potential. A significant negative correlation was discovered between aggressive discounting and net profitability.
* **Tools:** `Pandas`, `Seaborn`, `Matplotlib`.

### 2️⃣ Phase 2: Predictive Modeling (Machine Learning)
* **Objective:** Predict the **Profit** of an order based on features such as Discount, Product Category, and Region.
* **Algorithm:** Implemented a **Random Forest Regressor** optimized via `GridSearchCV` (evaluating 36 different parameter combinations).
* **Business Insight:** The "Discount" variable was identified as the single most critical factor impacting profit margins.
* **Result:** The model successfully quantifies how business decisions directly affect the bottom line.

### 3️⃣ Phase 3: A/B Testing (Statistical Inference)
* **Objective:** Scientifically prove whether the profit difference between 'Technology' and 'Office Supplies' is statistically significant or merely due to random chance.
* **Method:** Conducted a **Welch’s T-Test** (chosen due to unequal variances and varying sample sizes).
* **Statistical Result:** Obtained a P-Value of $1.17 \times 10^{-8}$, confirming a highly significant difference.
* **Conclusion:** We are 95% confident that Technology products earn an average of **$58.42** more profit per transaction than Office Supplies.

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Data Science:** `NumPy`, `Pandas`
* **Machine Learning:** `Scikit-Learn` (Pipelines, GridSearchCV)
* **Statistics:** `Scipy.stats`, `Statsmodels`
* **Visualization:** `Seaborn`, `Matplotlib`

---

## 📈 Executive Summary & Recommendations
1.  **Discount Management:** Data proves that discounts exceeding 20% exponentially destroy profit. A revised discounting ceiling is highly recommended.
2.  **Tech-First Strategy:** Statistical evidence confirms the Technology category is the primary engine of net profit. Inventory and marketing should prioritize this sector.
3.  **Model-Driven Decisions:** The developed ML model can serve as a decision-support tool for sales teams to estimate expected profit before finalizing contracts.

---

## 📂 Project Structure
```text
├── data/
│   └── sales.csv          # Raw Dataset from Kaggle.com
├── notebooks/
│   ├── 01_EDA.ipynb       # Cleaning & Visualization
│   ├── 02_ML_Model.ipynb  # Modeling & Hyperparameter Tuning
│   └── 03_AB_Testing.ipynb # Statistical Hypothesis Testing
└── README.md              # Final Project Report (This file)

