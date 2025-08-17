# Boiler-Efficiency-Prediction-XG-Boost-
# Boiler Outlet Steam Temperature Prediction

This project uses **XGBoost Regression** to predict the **Boiler Outlet Steam Temperature** based on process data.  
It evaluates model performance using common regression metrics and provides detailed error analysis.

---

## Features
- Data preprocessing (handling missing values, train-test split).
- XGBoost regression with hyperparameter tuning using `RandomizedSearchCV`.
- Performance metrics:
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score (Train & Test)
  - Mean Absolute Error (MAE)
- Error analysis:
  - Minimum and maximum absolute/percentage errors.
  - Identifies samples with highest/lowest prediction errors.
- Visualization of **Actual vs Predicted** values.

---
Main libraries used:
pandas
numpy
scikit-learn
xgboost
matplotlib

The project expects a CSV file (data_modified19.csv) containing boiler data.

Target column:
Boiler outlet steam temperature
Non-feature column removed:
date

sample o/p:

📊 Mean Absolute Error (MAE): 0.2079
📌 Minimum Absolute Error: 0.0000
📉 Minimum % Absolute Error: 0.0000%
📈 Maximum % Absolute Error: 1.5614%

🔍 Sample with MIN Absolute Error:
Actual = 539.8600, Predicted = 539.8600, Error = 0.0000

🔍 Sample with MIN % Error:
Actual = 539.8600, Predicted = 539.8600, % Error = 0.0000%

🔍 Sample with MAX % Error:
Actual = 525.2900, Predicted = 533.4920, % Error = 1.5614%
