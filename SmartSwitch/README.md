### SmartSwitch: Optimizing Plan Recommendations for Megaline Subscribers

#### Overview
This project delves into the mobile carrier Megaline's subscriber behavior data, aiming to recommend the optimal plan (Smart or Ultra) for each user. By analyzing data on calls, messages, internet usage, and current plans, the goal is to develop a model that accurately predicts the best plan for subscribers. With a focus on achieving high accuracy, this project involves data preprocessing, model development, and evaluation using a test dataset, ultimately enhancing customer satisfaction and optimizing plan recommendations.

#### Questions/Commands
- **What does this project do?**
  - Identifies and removes inconsistent or unusual data entries to enhance result accuracy.
  - Trains, fine-tunes, and evaluates different models to recommend the optimal plan with the highest accuracy.
  - Checks the model’s accuracy using the test dataset, aiming for a threshold of 0.75.
  - Performs a final validation of the ideal model to ensure robust and reliable findings.

#### Prerequisites
- Access to the required dataset.
- Basic understanding of data manipulation, analysis (EDA/SDA) & model creation in Python.

#### Functionality

- **Data Cleaning**: Cleans and organizes subscriber behavior data, including calls, messages, internet usage, and current plans, to ensure it's ready for analysis.
- **Model Training**: Develops a classification model to recommend the optimal plan (Smart or Ultra) by training it on the cleaned dataset.
- **Model Tuning**: Fine-tunes the model by adjusting hyperparameters and testing different algorithms to achieve the highest accuracy.
- **Model Evaluation**: Evaluates the model's performance using a test dataset, aiming for an accuracy threshold of 0.75, and performs a sanity check to validate the results.

#### Technologies
To build this project, the following tools and technologies were utilized:
- **Python**
- **Pandas**
- **SKLearn**
- **Jupyter Notebook** for interactive analysis

#### Installing
Clone the repository and install the required dependencies to run the analysis on your local machine:
```bash
git clone [repo link]
cd [repo name]
pip install -r requirements.txt
jupyter notebook


