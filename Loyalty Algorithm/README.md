# Interconnect Customer Churn Prediction

## Overview
This project analyzes customer data for Interconnect, a telecom provider, to predict client churn. The goal is to identify customers likely to cancel services so targeted retention strategies (e.g., promotional codes, special plans) can be deployed. The analysis combines contract, personal, internet, and phone service data, processed using Python with pandas and scikit-learn. A LightGBM classifier achieved 0.93 AUC-ROC and 0.86 accuracy in predicting churn.

## Problem(s) to be addressed
- **Churn Prediction**: Identify at-risk customers before they cancel services to enable proactive retention efforts.
- **Data Integration**: Combine fragmented customer data from multiple sources (`contract.csv`, `personal.csv`, `internet.csv`, `phone.csv`) into a unified analysis.
- **Model Performance**: Meet business metrics (AUC-ROC ≥ 0.75 for actionable predictions) while avoiding overfitting.
- **Feature Engineering**: Improve relationship understanding between customer attributes and churn likelihood.

## Key Features
- **Data Integration**: Merges four datasets using `customerID` as a unique key.
- **Feature Engineering**: Creates meaningful predictors from raw contract and service data.
- **Model Training**: Evaluates multiple classifiers (including LightGBM, Random Forest) with hyperparameter tuning.
- **Performance Metrics**: Focuses on AUC-ROC (primary) and accuracy (secondary) per business requirements.
- **Interpretability**: Includes feature importance analysis to explain churn drivers.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Top Performing Model**:
   - LightGBM achieved 0.93 AUC-ROC and 0.86 accuracy after tuning.
- **Critical Churn Indicators**:
   - Contract type (monthly vs. long-term)
   - Internet service type (fiber vs. DSL)
   - Additional services usage (TechSupport, OnlineBackup)
- **Validation Insight**:
   - Consistent random state values across train/validation/test splits proved crucial to prevent overfitting.

## Further Improvements
- **Feature Engineering**:
   - Implement PolynomialFeatures to explore nonlinear relationships between predictors.
   - Create interaction terms between service types and contract durations.
- **Model Deployment**:
   - Build an API to score new customers in real-time using Flask/Django.
- **Monitoring**:
   - Add data drift detection to identify when model retraining is needed.
- **Customer Segmentation**:
   - Cluster churn-prone users to tailor retention offers (e.g., heavy streaming users vs. business clients).
  
![image](https://github.com/user-attachments/assets/4d3e33d4-63d4-44ba-ad0c-9175d18a769e)
![image](https://github.com/user-attachments/assets/0e7ebd72-2d3d-4871-86cf-84851abbfb8d)

**Libraries**:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn lightgbm catboost xgboost
