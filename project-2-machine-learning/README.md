# Project-2 Machine Learning
🤖 Project: Superstore Profitability Forecasting (ML)
Goal: Build and optimize a high-precision Regression model to predict transaction profit and identify financial drivers.

🚀 Machine Learning Roadmap (8-Step Pipeline)
1️⃣ Data Audit & Pruning
Action: Handled latin1 encoding and dropped non-predictive features (Row ID, Postal Code).
Result: A refined dataset structured for mathematical modeling.
2️⃣ Feature Engineering
Action: Engineered Days_to_Ship and extracted Order_Month from timestamps.
Splitting: Data split into 80% Training and 20% Testing sets.
3️⃣ Automated Preprocessing (Scikit-Learn Pipeline)
Numerical: Applied StandardScaler to normalize sales and quantity data.
Categorical: Utilized OneHotEncoder for regions, categories, and segments.
Integrity: Used ColumnTransformer to prevent data leakage.
4️⃣ Model Selection: Random Forest
Algorithm: RandomForestRegressor.
Logic: Selected for its ability to handle non-linear relationships and complex interactions between features.
5️⃣ Optimization (Hyperparameter Tuning)
Method: GridSearchCV with 3-Fold Cross-Validation.
Best Parameters: * max_depth: 20
n_estimators: 200
min_samples_split: 2
📊 Model Performance & Metrics
Metric	Final Value	Business Meaning
R² Score	-0.0444	Indicates high variance in the current data model.
MAE	 26.69∗∗|Averagedeviationofpredictionfromactualprofit.||∗∗ActualProfitMean∗∗|∗∗ 20.50	The average profit observed in the real data.
Predicted Profit Mean	$29.94	The model's average forecasted value.
🔑 Business Insights (Feature Importance)
The model analyzed which factors have the most "weight" in determining profit:

Sales (73.92%): 🌟 The primary driver of profitability magnitude.
Discount (15.84%): 📉 The second most influential factor (negative impact).
Quantity (1.24%): Minimal impact compared to price and discount.
Sub-Category Binders: The most predictive product type in this model.
📈 Final Validation: Actual vs. Predicted
To confirm the reliability of our forecast, we compare the model's predictions against the ground truth.

🛠️ Technical Stack
Language: Python 3.x
ML Library: Scikit-Learn
Data Ops: Pandas, NumPy
Viz: Matplotlib, Seaborn
Author: Sahel
Project: Superstore Analytics Series (Part 2: Machine Learning)n
