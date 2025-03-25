# Beta Bank Customer Churn Prediction  

## Overview  
This project aims to predict customer churn for Beta Bank using historical client behavior and contract termination data. The goal is to build a classification model that can identify customers likely to leave the bank soon, allowing the bank to implement retention strategies. The project involves data preprocessing, exploratory analysis, handling class imbalance, and evaluating multiple machine learning models (Decision Tree, Random Forest, and Logistic Regression) to achieve the best F1 score (target: ≥0.59). The final Logistic Regression model achieved satisfactory performance, with additional evaluation using AUC-ROC metrics.  

## Problem(s) to be addressed  
- **Customer Retention**: Predicting churn helps Beta Bank retain customers more cost-effectively than acquiring new ones.  
- **Class Imbalance**: The dataset is highly imbalanced (20% churn vs. 80% non-churn), requiring techniques like upsampling to improve model performance.  
- **Model Selection**: Comparing multiple classifiers (Decision Tree, Random Forest, Logistic Regression) to identify the best-performing model based on F1 score and AUC-ROC metrics.  

## Key Features  
- **Data Preprocessing**:  
  - Handled missing values in the `Tenure` column.  
  - Dropped irrelevant columns (`RowNumber`, `CustomerId`, `Surname`).  
  - Encoded categorical variables (`Geography`, `Gender`) using One-Hot Encoding.  
  - Scaled numeric features using `StandardScaler`.  
- **Class Imbalance Fix**: Applied upsampling to balance the target variable (`Exited`).  
- **Model Training & Evaluation**:  
  - Trained and tuned Decision Tree, Random Forest, and Logistic Regression models.  
  - Evaluated models using F1 score, precision, recall, and AUC-ROC metrics.  
  - Selected Logistic Regression as the best model (F1 > 0.59 on the test set).  

## Prerequisites  
To run this project, you'll need:  
- **Python 3.7+**  
- **Jupyter Notebook** 

## Key Findings
- **Data Insights**:
  - The dataset had 909 missing values in the `Tenure` column, which were dropped
  - The target variable (`Exited`) was highly imbalanced (20.4% churn vs. 79.6% non-churn)
  
- **Model Performance**:
  - **Logistic Regression**:
    - Achieved the highest F1 score (>0.59)
    - Demonstrated strong AUC-ROC performance
  - **Decision Tree & Random Forest**:
    - Underperformed in F1 score despite hyperparameter tuning
    - Showed low recall on the validation set

## Further Improvements
- **Feature Engineering**:
  - Create interaction terms (e.g., `Age × Balance`)
  - Develop tenure-based customer segments
  - Add time-based features from historical data

- **Model Enhancements**:
  - Experiment with gradient boosting methods (XGBoost, LightGBM)
  - Implement stacked ensemble models
  - Test neural network approaches

- **Deployment Optimization**:
  - Build API for real-time churn prediction
  - Integrate with CRM for automated retention campaigns
  - Implement monitoring for model drift

- **Libraries**:  
  ```bash  
  pip install pandas numpy matplotlib scikit-learn  