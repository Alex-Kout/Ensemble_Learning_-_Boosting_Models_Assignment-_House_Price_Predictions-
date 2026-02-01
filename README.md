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

🔹 Model Evaluation
Model	RMSLE	MAE	RMSE	R²
Gradient Boosting	0.0251	3586	4738	0.996
XGBoost	0.0443	5802	8275	0.989
Random Forest	0.0532	6617	12592	0.975
Linear Regression	0.0922	11345	17828	0.950
Decision Tree	0.1255	15938	25641	0.896
Dummy Regressor	0.3993	55616	80676	-0.032

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
