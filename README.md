This repository contains my approach to solving the Kaggle House Prices - Advanced Regression competition. The goal is to build a robust regression model that predicts house prices based on 79 independent variables describing various house attributes.

I followed a structured approach to data preprocessing, feature engineering, and model tuning before making submissions. Approach & Methodology

1️⃣ Feature Selection 📊
Filtered independent variables that intuitively influence the target variable (SalePrice) using a manual analysis in Google Sheets.

2️⃣ Data Preprocessing & Feature Engineering 🏗️
Created new features by condensing multiple similar columns or introducing interaction terms.
Applied log transformation to SalePrice (SalePrice_log) to stabilize variance and improve model performance.

3️⃣ Handling Missing Values 🔍
Imputed missing values using a correlated column that had no missing values, ensuring minimal information loss.

4️⃣ Model Training & Hyperparameter Tuning 🤖
Used XGBoost Regressor (XGBRegressor) with RandomizedSearchCV for hyperparameter tuning and model selection.
Implemented cross-validation (5-fold CV) to improve generalization and prevent overfitting.
Applied early stopping using a validation set to stop training when performance no longer improved.

Next Steps 🚀
Further fine-tuning of feature selection and engineering.
Experimenting with ensemble methods like stacking or blending.
This notebook keeps things simple yet effective, focusing on core modeling principles while ensuring reproducibility.
