### Churn Prediction: Retention Strategies for Beta Bank

#### Overview
This project delves into the banking industry, focusing on Beta Bank's efforts to prevent customer churn. The primary aim is to analyze customer behavior and predict whether a client is likely to leave the bank. By building a highly accurate model, the goal is to enhance customer retention strategies and reduce churn rates, ensuring long-term customer loyalty and satisfaction.

#### Questions/Commands
- **What does this project do?**
- Filters the dataset to include only customer behavior data and termination of contracts with the bank.
  - Examines the balance of classes to understand the distribution of customers who left and those who stayed.
  - Identifies and applies at least two methods to address class imbalance, such as SMOTE or class weighting.
  - Develops a classification model with the goal of maximizing the F1 score to predict customer churn.
  - Measures and compares the AUC-ROC metric alongside the F1 score to evaluate model performance and ensure robust and reliable predictions.
    
#### Prerequisites
- Access to the required dataset: /datasets/Churn.csv file containing customer behavior data and termination of contracts.
- Basic understanding of data manipulation and analysis in Python.
- Familiarity with machine learning libraries such as Scikit-learn.
- Knowledge of classification algorithms and techniques.
- Experience with handling class imbalance in datasets.
- Understanding of evaluation metrics like F1 score and AUC-ROC.

#### Functionality
- **Data Preparation**: Gathers and prepares the customer behavior dataset for thorough analysis.
- **Class Balance Review**: Reviews the class balance to assess the distribution of customers who left versus those who stayed.
- **Initial Model Training**: Trains the initial model without addressing class imbalance to set a performance benchmark.
- **Addressing Class Imbalance**: Implements at least two methods to tackle class imbalance, such as resampling techniques or modifying class weights.
- **Model Optimization and Evaluation**: Trains and fine-tunes various models on training and validation sets, selecting the most accurate one.
- **Performance Metrics Assessment**: Calculates and compares the F1 score and AUC-ROC metric to evaluate and validate the model's effectiveness.

#### Technologies
To build this project, the following tools and technologies were utilized:
- **Python** for data manipulation and model building.
- **Pandas** for efficient data handling and analysis.
- **NumPy** for numerical operations and data processing.
- **Scikit-learn** for implementing machine learning algorithms and evaluation metrics.
- **Matplotlib** and **Seaborn** for data visualization and exploratory analysis.
- **Jupyter Notebook** for interactive and iterative development.

#### Installing
Clone the repository and install the required dependencies to run the analysis on your local machine:
```bash
git clone [repo link]
cd [repo name]
pip install -r requirements.txt
jupyter notebook
