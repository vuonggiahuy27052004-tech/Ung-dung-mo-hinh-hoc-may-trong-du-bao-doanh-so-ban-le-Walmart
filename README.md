# Ung-dung-mo-hinh-hoc-may-trong-du-bao-doanh-so-ban-le-Walmart
📌 Overview

This project applies machine learning models to forecast weekly retail sales for Walmart stores. The goal is to improve demand prediction by incorporating economic indicators, seasonal patterns, and holiday effects.

The project evaluates multiple regression models and identifies the most effective approach for real-world deployment.

🎯 Objectives
Analyze and preprocess large-scale retail data (420k+ records)
Capture seasonality and holiday effects in sales patterns
Build and compare machine learning models:
Decision Tree
Random Forest
XGBoost
Optimize forecasting accuracy using advanced evaluation metrics
📂 Dataset
Source: Walmart Store Sales dataset (Kaggle)
Size: ~421,570 rows, 16 features
Time range: Feb 2010 – Nov 2012
Key features:
Weekly_Sales (target)
Store, Dept, Type, Size
Date → engineered into Year, Month, Week
Economic variables: CPI, Fuel_Price, Unemployment
IsHoliday (holiday indicator)
⚙️ Methodology
1. Data Preprocessing
Converted date to time features (Year, Month, Week)
Removed noisy variables (Markdown features)
Checked missing values (none found)
Train/Test split: 80/20
2. Exploratory Data Analysis (EDA)
Identified strong seasonality (Nov–Dec peaks)
Holiday weeks show:
Higher mean sales
Higher variance
Store size & department strongly impact sales
3. Models Implemented
Decision Tree Regressor
Random Forest Regressor
XGBoost Regressor
4. Evaluation Metrics
MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)
R² Score
Out-of-Sample R² (OOS R²)
📈 Results
Model	Performance Summary
Decision Tree	High variance, overfitting
Random Forest	⭐ Best performance
XGBoost	Good but underperformed RF
✅ Best Model: Random Forest
OOS R² ≈ 0.96
RMSE ≈ 3273
Strong generalization (no overfitting)
