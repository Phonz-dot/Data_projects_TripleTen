# Movie Review Classification System  

## Overview  
This project develops an automated system for classifying movie reviews as positive or negative, designed for the Film Junky Union community. The system analyzes IMDB movie reviews using natural language processing (NLP) techniques and machine learning models to detect sentiment with high accuracy. The final model achieves an F1 score exceeding 0.85, meeting the project requirements.  

## Key Features  
- Classifies movie reviews as positive or negative with high accuracy  
- Implements multiple NLP preprocessing techniques (NLTK and spaCy)  
- Tests various machine learning models (Logistic Regression, LGBMClassifier)  
- Includes comprehensive evaluation metrics (F1 score, ROC AUC, accuracy)  
- Demonstrates performance on custom review examples  

## Prerequisites  
To run this project, you'll need:  
- Python 3.7+  
- Jupyter Notebook  
- The following Python libraries:  
  - pandas  
  - numpy  
  - matplotlib  
  - seaborn  
  - scikit-learn  
  - nltk  
  - spacy  
  - lightgbm

## Key Findings
- The dataset was well-balanced between positive (49.9%) and negative (50.1%) reviews
- Both Logistic Regression models (using NLTK and spaCy) achieved F1 scores > 0.85
- The best performing model was Model 1 (NLTK + TF-IDF + Logistic Regression) with:
  - Test Accuracy: 0.88
  - Test F1 Score: 0.88
  - ROC AUC: 0.95

Install the required packages using:  
```bash  
pip install pandas numpy matplotlib seaborn scikit-learn nltk spacy lightgbm  
