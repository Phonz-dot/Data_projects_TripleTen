# Megaline Subscriber Behavior Analysis

## Overview
This project aims to develop a classification model to analyze subscriber behavior and recommend the most suitable plan (Smart or Ultra) for Megaline's customers. The goal is to achieve an accuracy score above 0.75 by evaluating three machine learning models: Decision Tree, Random Forest, and Logistic Regression. The Random Forest model performed best with an accuracy of 0.81, meeting the business objective. The analysis was conducted using Python with libraries like pandas, scikit-learn, and GridSearchCV for hyperparameter tuning.

## Problem(s) to be addressed
- **Legacy Plan Usage**: Many Megaline subscribers are still on outdated plans, and the company wants to migrate them to newer plans (Smart or Ultra) based on their usage behavior.
- **Model Accuracy**: The model must accurately classify subscribers into the correct plan with an accuracy threshold of 0.75 or higher.
- **Behavioral Insights**: Understanding how call duration, text messages, and data usage influence plan choice can help tailor marketing strategies and improve customer satisfaction.

## Key Features
- **Data Preprocessing**: The dataset was checked for missing values and duplicates, ensuring clean and reliable data for modeling.
- **Model Development**: Three classification models were trained and evaluated:
  - **Decision Tree**: Achieved an accuracy of 0.80 after hyperparameter tuning.
  - **Random Forest**: Performed best with an accuracy of 0.81.
  - **Logistic Regression**: Reached an accuracy of 0.74, below the target threshold.
- **Hyperparameter Tuning**: GridSearchCV was used to optimize model parameters, improving accuracy.
- **Sanity Check**: The Random Forest model was validated against a baseline DummyClassifier, confirming its reliability.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Best Model**: 
  - The Random Forest classifier with max_depth=10 and n_estimators=100 achieved the highest accuracy (0.81) on the test set.
- **Feature Importance**: 
  - The model identified call duration (minutes) and data usage (mb_used) as significant predictors for plan recommendation.
- **Validation**: 
  - The model's performance was consistent across training, validation, and test sets, indicating no overfitting or underfitting.

## Further Improvements
- **Feature Engineering**: 
  - Explore creating new features (e.g., call-to-text ratio) to improve model accuracy.
- **Model Explainability**: 
  - Use SHAP or LIME to interpret the model's decisions and provide transparent recommendations to subscribers.
- **Real-Time Deployment**: 
  - Integrate the model into Megaline's customer portal for real-time plan recommendations.
- **Scalability Testing**: 
  - Evaluate the model's performance on larger datasets or additional features (e.g., customer demographics).

- **Libraries**:
  ```bash
  pip install pandas numpy scikit-learn plotly