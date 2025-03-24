# Customer Churn Prediction for Interconnect Telecom

## Overview  
This project was developed for Interconnect Telecom to help them predict and reduce customer churn. Using a dataset combining contract details, internet services, personal information, and phone services, machine learning models were trained to identify customers at risk of leaving. The goal is to enable proactive retention strategies by flagging high-risk customers before they churn.

### Key Features  
- **Data Integration**: Merged 4 separate datasets (contract, internet, personal, phone) into a unified dataset.  
- **Feature Engineering**: Created new temporal features from contract dates and handled categorical variables.  
- **Class Imbalance Handling**: Addressed skewed target distribution using upsampling techniques.  
- **Model Comparison**: Evaluated 6 different classifiers to identify the best-performing model.  

---

## Prerequisites  
To run this project, you will need:  
- Python 3.7 or higher  
- Scikit-learn, XGBoost, LightGBM, CatBoost  
- Pandas, NumPy, Matplotlib, Seaborn  
- SHAP for model interpretation  

---

## Technologies  
- **Machine Learning**: Scikit-learn, XGBoost, LightGBM, CatBoost  
- **Model Optimization**: GridSearchCV and RandomizedSearchCV for hyperparameter tuning  
- **Data Processing**: Pandas for data wrangling, StandardScaler for feature normalization  
- **Visualization**: Seaborn for correlation heatmaps, Matplotlib for feature distributions  

---

### Findings  
- The LightGBM model performed best with 0.93 AUC-ROC and 0.86 accuracy.  
- Key churn indicators included contract type (month-to-month highest risk), fiber optic internet users, and higher monthly charges.  
- Total charges showed a significant negative correlation with contract start year.  
- The original dataset had 27% churn rate, requiring upsampling for balanced training.  

---

## Installation  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-repo/telecom-churn-prediction.git  
