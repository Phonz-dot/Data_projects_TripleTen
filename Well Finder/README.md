# Oil Well Region Selection Analysis

## Overview
This project aims to identify the optimal region for OilyGiant mining company to develop new oil wells by analyzing geological exploration data from three potential regions. The goal is to maximize profit while minimizing risks. The analysis involves data preprocessing, exploratory data analysis (EDA), model training using linear regression, and profit calculation with Bootstrapping. Key findings include the average predicted reserves, RMSE for each region, and the associated risks of loss. The project is implemented using Python with pandas, numpy, scikit-learn, and matplotlib for data analysis and visualization.

## Problem(s) to be addressed
- **Region Selection**: Determine which of the three regions offers the highest profit potential for oil well development while meeting the risk threshold.
- **Data Analysis**: Clean and preprocess the data, ensuring it is ready for model training and analysis.
- **Model Training**: Use linear regression to predict the volume of reserves in new wells, adhering to the constraint that only linear regression is suitable.
- **Profit and Risk Calculation**: Evaluate potential profit and risks using Bootstrapping to ensure the selected region meets the business criteria (risk of losses < 2.5%).

## Key Features
- **Data Preprocessing**: 
  - Dropped the non-contributory 'id' column.
  - Scaled numeric features to ensure uniformity.
- **Exploratory Data Analysis (EDA)**:
  - Checked for null values and duplicates (none found).
  - Analyzed the distribution of reserves across regions.
- **Model Training**:
  - Split data into training and validation sets (75:25 ratio).
  - Trained linear regression models for each region.
  - Evaluated models using RMSE and average predicted reserves.
- **Profit and Risk Analysis**:
  - Calculated the minimum volume of reserves needed to break even (112 thousand barrels).
  - Used Bootstrapping to estimate average profit, confidence intervals, and risk of loss for each region.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Region 0**:
  - Average Predicted Reserves: 92.59 thousand barrels.
  - RMSE: 37.58.
  - Risk of Loss: 10.0%.
- **Region 1**:
  - Average Predicted Reserves: 68.73 thousand barrels.
  - RMSE: 0.89.
  - Risk of Loss: 1.3%.
- **Region 2**:
  - Average Predicted Reserves: 94.97 thousand barrels.
  - RMSE: 40.03.
  - Risk of Loss: 12.8%.
- **Selected Region**: 
  - Region 1, as it has the lowest risk of loss (1.3%) and meets the business requirement of being below 2.5%, while also offering competitive average revenue.

## Further Improvements
- **Model Enhancement**: 
  - Experiment with feature engineering or other linear regression variants (e.g., Ridge or Lasso) to improve prediction accuracy.
- **Data Expansion**: 
  - Incorporate additional geological features or historical data to refine the model's predictions.
- **Dynamic Budgeting**: 
  - Adapt the analysis to accommodate varying budgets or well counts to simulate different business scenarios.
- **Risk Sensitivity Analysis**: 
  - Explore how changes in oil prices or development costs impact the risk of loss and profit margins.

- **Libraries**:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn