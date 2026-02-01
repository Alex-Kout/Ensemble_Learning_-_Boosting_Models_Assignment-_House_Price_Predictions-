🏠 House Price Prediction

Predict house prices using ensemble learning and boosting models with advanced data preprocessing and feature engineering.

🔹 Project Overview

This project implements multiple regression models to predict house prices, including:

Decision Tree

Random Forest

Gradient Boosting

XGBoost

Gradient Boosting achieved the best performance.

🔹 Key Features

Handling missing data (median for numeric, 'None' for categorical)

Log transformation for skewed features and target variable

One-hot encoding of categorical variables

Hyperparameter tuning with GridSearchCV

### Model Evaluation

| Model              | RMSLE  | MAE    | RMSE   | R²    |
|------------------- |-------:|-------:|-------:|------:|
| Gradient Boosting  | 0.0251 | 3,586  | 4,738  | 0.996 |
| XGBoost            | 0.0443 | 5,802  | 8,275  | 0.989 |
| Random Forest      | 0.0532 | 6,617  | 12,592 | 0.975 |
| Linear Regression  | 0.0922 | 11,345 | 17,828 | 0.950 |
| Decision Tree      | 0.1255 | 15,938 | 25,641 | 0.896 |
| Dummy Regressor    | 0.3993 | 55,616 | 80,676 | -0.032 |


Insight: Gradient Boosting is the most accurate; XGBoost offers faster training with competitive results.

🔹 Feature Importance (Top 5)

OverallQual – Overall material & finish

GrLivArea – Above-grade living area

TotalBsmtSF – Basement square footage

GarageCars – Garage capacity

1stFlrSF – First-floor area

🔹 Limitations

Underestimates high-priced houses

Residuals show heteroscedasticity for expensive properties


🔹 Conclusion

Gradient Boosting delivers the best predictions, balancing accuracy and interpretability. XGBoost is a faster alternative with slightly lower performance.
