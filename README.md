# House-Prices-Advanced-Regression

This repository contains my approach to solving the Kaggle House Prices - Advanced Regression competition. The goal is to build a robust regression model that predicts house prices based on 79 independent variables describing various house attributes.
I followed a structured approach to preprocessing the data, feature engineering, and model tuning before making submissions. Key steps include:

1. Feature Selection 📊
  -Filtered independent variables that intuitively influence the target variable (SalePrice) using a manual analysis in Google Sheets.

2.Data Preprocessing & Feature Engineering 🏗️
  -Created new features by either condensing multiple similar columns or introducing interaction terms.
  -Took the log transformation of SalePrice (SalePrice_log) to stabilize variance and improve model performance.

3.Handling Missing Values 🔍
  -Imputed missing values using a correlated column that had no missing values, ensuring minimal information loss.

4. Model Training & Hyperparameter Tuning 🤖
  -Used XGBoost Regressor (XGBRegressor) with RandomizedSearchCV for hyperparameter tuning and model selection.
  -Implemented cross-validation (5-fold CV) to improve generalization and prevent overfitting.
  -Used early stopping based on a validation set, ensuring the model stops training when performance no longer improves.

Next Steps 🚀
1. Further fine-tuning of feature selection and engineering.
2. Experimenting with ensemble methods like stacking or blending.
