# Sure Tomorrow Insurance Machine Learning Analysis

## Overview
This project evaluates the potential of machine learning to address key business tasks for Sure Tomorrow Insurance. The goal is to analyze customer data to improve marketing, predict insurance benefit likelihood, and protect sensitive client information. The analysis includes similarity modeling, classification, regression, and data obfuscation techniques. Key findings demonstrate the effectiveness of kNN for customer similarity, the superiority of trained models over dummy models, and the feasibility of data masking without degrading model performance. The project is implemented using Python with libraries like pandas, scikit-learn, and NumPy.

## Problem(s) to be addressed
- **Customer Similarity**: Identify similar customers to enhance targeted marketing efforts.
- **Benefit Prediction**: Determine if a new customer is likely to claim insurance benefits and predict the number of benefits they might receive.
- **Data Privacy**: Develop a method to obfuscate personal data while preserving model accuracy.
- **Model Validation**: Compare trained models against baseline dummy models to ensure effectiveness.

## Key Features
- **Task 1: Similar Customer Identification**:
  - Implemented kNN algorithm with Euclidean and Manhattan distance metrics.
  - Evaluated the impact of data scaling on model performance.
- **Task 2: Benefit Likelihood Prediction**:
  - Built a kNN classifier and compared it to a random dummy model using F1 score.
  - Addressed class imbalance through upsampling.
- **Task 3: Benefit Quantity Prediction**:
  - Developed a linear regression model to predict the number of benefits.
  - Measured performance using RMSE and R2 metrics.
- **Task 4: Data Obfuscation**:
  - Applied matrix multiplication to mask sensitive data while maintaining model integrity.
  - Verified that transformed data does not affect regression results.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Customer Similarity**:
  - Data scaling significantly impacts kNN results, with scaled features providing more accurate neighbor identification.
  - Manhattan and Euclidean metrics yield similar results, with minor variations in distance calculations.
- **Benefit Prediction**:
  - The trained kNN classifier outperformed the dummy model, achieving an F1 score of 1.0 for scaled data.
  - Class imbalance correction via upsampling improved model robustness.
- **Regression Performance**:
  - Linear regression achieved an RMSE of 0.34 and R2 of 0.66, with no difference between scaled and unscaled data.
- **Data Obfuscation**:
  - Personal data was successfully masked using an invertible matrix, and original data could be recovered when needed.
  - Model performance remained unchanged after obfuscation, proving the method's validity.

## Further Improvements
- **Enhanced Similarity Metrics**: 
  - Experiment with other distance metrics (e.g., Cosine similarity) to improve customer matching.
- **Advanced Classification**: 
  - Test other classifiers (e.g., Random Forest, SVM) to compare performance with kNN.
- **Dynamic Obfuscation**: 
  - Implement a dynamic matrix generation system for enhanced data security.
- **Feature Engineering**: 
  - Explore additional features (e.g., customer region, health history) to improve prediction accuracy.
 
![image](https://github.com/user-attachments/assets/1b8b7e8c-670d-4627-8c91-9e9958da7e31)

- **Libraries**:
  ```bash
  pip install pandas numpy scikit-learn matplotlib seaborn
