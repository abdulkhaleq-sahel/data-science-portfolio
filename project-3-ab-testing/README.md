# 🧪 Project: A/B Testing - Profitability Analysis
---
> **Goal:** Statistically verify if the profit difference between 'Technology' and 'Office Supplies' is significant or just random noise.

---

## 📊 Project Methodology (The 8-Step Statistical Workflow)

### 1️⃣ Hypothesis Definition
* **H₀ (Null Hypothesis):** Mean Profit of Technology = Mean Profit of Office Supplies.
* **H₁ (Alternative Hypothesis):** Mean Profit of Technology ≠ Mean Profit of Office Supplies.
* **Alpha ($\alpha$):** 0.05 (Standard significance level).

### 2️⃣ Sampling & Descriptive Stats
* **Group A (Technology):** 1,847 orders | Mean Profit: **$78.75**
* **Group B (Office Supplies):** 6,026 orders | Mean Profit: **$20.33**
* **Observed Gap:** **$58.42** per transaction.

### 3️⃣ Normality Check (Shapiro-Wilk Test)
* **Result:** P-Value ≈ 0.0000
* **Conclusion:** Data is **Not Normally Distributed** (common in financial data due to outliers).

### 4️⃣ Variance Equality (Levene’s Test)
* **Result:** P-Value ≈ 0.0000
* **Conclusion:** Variances are **Unequal**. 
* **Action:** Proceed with **Welch’s T-Test** (designed for unequal variances/sample sizes).

### 5️⃣ Statistical Execution (Welch's T-Test)
* **T-Statistic:** 5.7271
* **P-Value:** $1.1750 \times 10^{-8}$ (Extremely low)
* **Decision:** **Reject H₀**. The difference is statistically significant.

### 6️⃣ Confidence Intervals (Effect Size)
* **95% Confidence Interval:** **$38.42 to $78.43**
* **Meaning:** We are 95% sure that Technology products will always earn at least **$38.42** more profit than Office Supplies per order.

---

## 📈 Visualizing the Evidence
The following charts confirm that the profit distribution of Technology is shifted towards higher values compared to Office Supplies.



---

## 🔑 Final Business Insights
* **Statistical Confirmation:** The $58 profit gap is **REAL** and not a result of random luck or sampling bias.
* **Risk Assessment:** Technology shows higher variance (more risk/reward), while Office Supplies is more stable but less profitable.
* **Executive Strategy:** 1.  **Prioritize Inventory:** Increase stock for Technology category.
    2.  **Marketing Focus:** Redirect ad spend toward Technology to maximize overall net profit.
    3.  **Stability:** Use Office Supplies as a "buffer" for consistent, low-risk revenue.

---

## 🛠️ Tools Used
* **Stats Engine:** `Scipy.stats`, `Statsmodels`
* **Visualization:** `Seaborn`, `Matplotlib`
* **Data Ops:** `Pandas`, `NumPy`

---
**Author:** Sahel  
**Project:** Superstore Analytics Series (Part 3: Inferential Statistics)
