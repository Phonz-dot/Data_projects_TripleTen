# Rusty Bargain Used Car Price Prediction

## Overview
This project develops a machine learning model to predict the market value of used cars for Rusty Bargain's customer app. Using historical data on technical specifications, trim versions, and prices, the model helps customers quickly estimate their car's worth. The analysis compares multiple regression models (Linear Regression, Random Forest, XGBoost, LightGBM, CatBoost, and Stacked models) in terms of prediction quality, speed, and training time. The project is implemented in Python using pandas, scikit-learn, and other ML libraries.

## Problem(s) to be addressed
- **Accurate Valuation**: Customers need reliable price estimates to trust the service.
- **Performance Trade-offs**: Balance between prediction quality (RMSE) and computational efficiency (training/prediction time).
- **Data Quality**: Handle potential issues in features like registration year, mileage, and repair status that could affect model accuracy.

## Key Features
- **Data Preprocessing**: Cleans and prepares car sales data (e.g., handling registration year outliers, encoding categorical features).
- **Model Comparison**: Evaluates 6 models on:
  - Prediction quality (RMSE)
  - Training time
  - Prediction speed
- **Optimization**: Uses techniques like hyperparameter tuning and regularization to reduce overfitting.
- **Visualizations**: Includes comparison charts of model performance metrics.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Performance Comparison**:
  - **Fastest Training**: Linear Regression and LightGBM (under 1 minute)
  - **Most Accurate**: XGBoost (lowest RMSE of 1596 on test set)
  - **Best Balance**: CatBoost (good accuracy with moderate training time)
- **Prediction Timing**:
  - Linear Regression was fastest for predictions
  - Stacked models showed increased latency
- **Overfitting**:
  - All models showed some overfitting (validation RMSE < test RMSE)
  - Regularization helped mitigate this effect

## Further Improvements
  - **Feature Engineering**: Create age-based features from registration year/month to improve accuracy.
  - **Model Optimization**: Implement Bayesian optimization for hyperparameter tuning to reduce training time while maintaining accuracy.
  - **Deployment Pipeline**: Build a Flask/FastAPI endpoint to serve predictions with latency monitoring.
  - **Geospatial Analysis**: Incorporate postal code data (with proper anonymization) to account for regional price variations.

- **Libraries**:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm catboost