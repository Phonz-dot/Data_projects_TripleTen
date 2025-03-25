# Gold Recovery Optimization Model

## Overview
This project develops a machine learning model to predict gold recovery rates from ore at different purification stages for Zyfra, a company specializing in heavy industry efficiency solutions. The goal is to optimize production by identifying unprofitable parameters. The analysis involves data preprocessing, exploratory analysis, and model training using Linear Regression, Decision Trees, and Random Forests, evaluated with sMAPE (symmetric Mean Absolute Percentage Error). Key findings include purification stage efficiencies and feature importance for recovery prediction.

## Problem(s) to be addressed
- **Data Quality**: Handle missing values and outliers across datasets (`gold_recovery_train.csv`, `gold_recovery_test.csv`, `gold_recovery_full.csv`).
- **Feature Availability**: Test set lacks target variables (`rougher.output.recovery`, `final.output.recovery`) and some features present in the training set.
- **Process Optimization**: Predict gold recovery rates to streamline flotation and purification stages, reducing inefficiencies.

## Key Features
- **Data Preprocessing**:
  - Filled missing values using forward-fill to maintain temporal consistency.
  - Removed outliers detected via IQR to improve model accuracy.
- **Exploratory Analysis**:
  - Compared metal concentrations (Au, Ag, Pb) across purification stages (raw feed → rougher → final concentrate).
  - Analyzed feed particle size distributions between training and test sets (rejected null hypothesis via t-tests).
- **Model Training**:
  - Evaluated Linear Regression, Decision Trees, and Random Forests using cross-validated MAE.
  - **Best Model**: Linear Regression (lowest MAE: 11.8).
- **Evaluation Metric**:
  - Custom sMAPE calculation for rougher (12.48%) and final recovery (11.32%), weighted to a total sMAPE of **11.61%**.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**
- **Libraries**:
  ```bash
  pip install pandas numpy matplotlib seaborn scikit-learn

## Key Findings
- **Purification Efficiency**:
  - Gold concentration increases through stages (raw: 405k → final: 906k units), while silver declines (raw: 246k → final: 108k).
  - Lead shows moderate increase (raw: 156k → final: 206k units).
- **Particle Size**:
  - Training and test sets have significantly different distributions (p-values < 0.05).
- **Model Performance**:
  - Linear Regression outperformed tree-based models with stable cross-validation MAE scores (avg: 11.8).

## Further Improvements
- **Feature Engineering**: Incorporate lag features for time-dependent parameters (e.g., `air amount`, `feed rate`) to capture process dynamics.
- **Hyperparameter Tuning**: Optimize Random Forest parameters (e.g., `max_depth`, `n_estimators`) to reduce overfitting and improve sMAPE.
- **Real-time Monitoring**: Deploy model with sensor data pipelines to adjust purification parameters dynamically.

## Data Description
### Stages and Parameters:
- **Rougher**: Flotation stage (input: feed size, reagents; output: Au concentrate).
- **Primary/Secondary Cleaner**: Purification stages (state: fluid levels; output: final concentrate).
- **Final**: Product characteristics (e.g., `final.output.concentrate_au`).

### Feature Naming Convention:
`[stage].[parameter_type].[parameter_name]`  
Example: `rougher.input.feed_ag` (silver in raw feed).

### Recovery Calculation:
\`Recovery = (C × (F − T)) / (F × (C − T)) × 100\`  
Where:  
- **C**: Gold share in concentrate post-flotation/purification.  
- **F**: Gold share in feed pre-flotation.  
- **T**: Gold share in tails.  

---
**Note**: Test set excludes target variables and calculation-based features (e.g., `rougher.calculation.au_pb_ratio`).  