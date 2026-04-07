# Project 2 - Machine-learning
📊 Superstore Profit Prediction & Strategy Optimization
This repository contains a professional end-to-end Machine Learning project focused on predicting profitability and identifying key business drivers using the Superstore Sales dataset.

📂 Data Architecture
The primary dataset is stored in the following directory:
project-1-data-analysis/data/sales.csv

🚀 The 8-Step Machine Learning Framework
Step 1: Data Acquisition & Robust Loading
Technical Goal: Handle character encoding and initial cleaning.

Action: Loaded sales.csv using latin1 encoding to manage special characters. Removed non-predictive identifiers (IDs) to ensure the model focuses on patterns, not noise.

Step 2: Advanced Feature Engineering
Technical Goal: Extract time-based intelligence.

Action: Created Days_to_Ship (order-to-ship lead time) and Order_Month to capture seasonality. Split the data into 80% Training and 20% Testing to validate performance on unseen data.

Step 3: Production-Grade Preprocessing Pipeline
Technical Goal: Automated data transformation.

Action: Developed a ColumnTransformer pipeline. Numeric data was normalized via StandardScaler, and categorical data was encoded using OneHotEncoder. This ensures the model is ready for real-time deployment.

Step 4: Model Implementation (Random Forest)
Technical Goal: Leverage Ensemble Learning.

Action: Deployed a Random Forest Regressor. This algorithm was chosen for its superior ability to handle non-linear relationships and high-dimensional data common in retail analytics.

Step 5: Performance Benchmarking
Technical Goal: Initial accuracy assessment.

Action: Evaluated the baseline model using R-Squared (R2) and Mean Absolute Error (MAE). This stage identified the variance gaps that required hyperparameter optimization.

Step 6: Hyperparameter Tuning & Optimization
Technical Goal: Fine-tune model parameters for peak precision.

Action: Executed a GridSearchCV with 3-fold Cross-Validation.

Optimal Config: n_estimators: 200, max_depth: 20, min_samples_split: 2. This significantly improved the model's predictive power.

Step 7: Business Intelligence & Feature Importance
Technical Goal: Explainability for Stakeholders.

Action: Analyzed which variables drive profit. This revealed that Discount and Sales volume are the most critical factors, providing clear "levers" for management to adjust.

Step 8: Final Validation & Residual Analysis
Technical Goal: Visual proof of reliability.

Action: Created an Actual vs. Predicted scatter plot. This visualization demonstrates the model's reliability in forecasting financial outcomes, essential for executive-level presentations.

🛠️ Tech Stack
Environment: Google Colab / Jupyter

Core Engine: Scikit-Learn

Data Manipulation: Pandas & NumPy

Visualization: Matplotlib & Seaborn
