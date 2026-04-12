# 📊 End-to-End Sales Analytics & Business Strategy Project
> **From Raw Retail Data to Machine Learning Insights & Statistical Proof.**

---

## 📝 Project Overview
This project is a comprehensive Data Science study conducted on a Retail Sales dataset (sourced from Kaggle.com). It demonstrates a complete data lifecycle—starting from **Advanced Data Engineering**, moving through **Visual Storytelling**, and concluding with **Predictive Modeling** and **Rigorous Hypothesis Testing**.

---

## 🚀 Key Project Modules

### 1️⃣ Phase 1: Advanced EDA & Data Engineering
* **Objective:** Cleanse raw data and uncover hidden trends using a professional-grade pipeline.
* **Refined Cleaning Pipeline:**
    * **Logical Validation:** Resolved anomalies where `Ship Date` preceded `Order Date`.
    * **Normalization:** Standardized categorical text and optimized `Postal Code` formats (5-digit padding).
    * **Lead Time Analysis:** Engineered a `Days_to_Ship` feature to measure operational efficiency across shipping modes.
* **Key Discovery:** Confirmed a **Negative Correlation (-0.22)** between discounts and profit; identifying a "Profit Danger Zone" for discounts > 20%.

### 2️⃣ Phase 2: Predictive Modeling (Machine Learning)
* **Objective:** Predict the **Profit** of an order based on transactional features.
* **Algorithm:** **Random Forest Regressor** optimized via `GridSearchCV` (evaluating 36 parameter combinations).
* **Feature Importance:** Data identifies "Discount" and "Product Category" as the primary predictors of the bottom line.
* **Value:** Provides sales teams with a tool to simulate profit outcomes before finalizing deals.

### 3️⃣ Phase 3: A/B Testing (Statistical Inference)
* **Objective:** Scientifically validate profit differences between Product Categories.
* **Method:** **Welch’s T-Test** (applied due to unequal variances and sample sizes).
* **Statistical Result:** P-Value of $1.17 \times 10^{-8}$.
* **Confidence:** 95% certainty that 'Technology' earns significantly more per transaction ($58.42 avg. delta) compared to 'Office Supplies'.

---

## 📈 Executive Summary & Recommendations
1. **Dynamic Discounting:** Implement a hard-cap on discounts. Data proves that aggressive discounting (e.g., 50%) leads to uncontrollable profit variance and net losses.
2. **Tech-Focused Inventory:** Statistical proof confirms the 'Technology' sector is the engine of profit. Recommend increasing inventory investment in this category.
3. **Logistics Optimization:** While 'Standard Class' is the volume leader, 'First Class' shipping is the most profitable per-unit mode. Aim to reduce Standard Class lead time (~5 days) to enhance customer retention.

---

## 🛠️ Tech Stack
* **Languages:** Python 3.x
* **Data Wrangling:** `Pandas`, `NumPy`
* **Machine Learning:** `Scikit-Learn` (Pipelines, GridSearchCV)
* **Statistics:** `Scipy.stats`, `Statsmodels`
* **Visualization:** `Seaborn`, `Matplotlib`

---

## 📂 Project Structure
```text
├── data/
│   └── sales.csv             # Raw Dataset (Source: Kaggle)
├── notebooks/
│   ├── sales_data_analysis.ipynb          # Adv. Cleaning, Lead-Time & Visual Trends
│   ├── Machine_Learning_Profit.ipynb     # Feature Engineering & Random Forest
│   └── A_B_testing.ipynb   # Statistical Validation & Hypothesis Testing
└── README.md                 # Executive Summary (This file)
