# Age Verification for Alcohol Sales Compliance

## Overview
This project evaluates the use of computer vision to help supermarket chain Good Seed comply with alcohol laws by verifying customers' ages at checkout. Using a dataset of 7.6k facial images with labeled ages, a neural network model is built and trained to predict age from photos. The goal is to determine whether the model can reliably prevent underage alcohol sales. The project employs Python with TensorFlow/Keras for model development, alongside exploratory data analysis (EDA) to assess data quality and model performance.

## Problem(s) to be addressed
- **Legal Compliance**: Ensure alcohol is not sold to underage customers by automating age verification at checkout.
- **Model Accuracy**: Address overfitting observed during training (validation loss increased from 78.44 to 93.41 over 20 epochs).
- **Resource Efficiency**: Handle large image datasets without excessive memory usage via `ImageDataGenerator`.

## Key Features
- **Data Preparation**: Sequential loading of images using `ImageDataGenerator` to optimize memory.
- **Neural Network Model**: 
  - Architecture tailored for age prediction from facial images.
  - Training monitored over 20 epochs with loss and MAE metrics.
- **Performance Analysis**: 
  - Training loss reduced from 95.35 to 17.02; MAE from 7.43 to 3.17.
  - Validation loss showed overfitting (peaked at 93.41).
- **Ethical Consideration**: Focus on minimizing false negatives (underage customers incorrectly approved).

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Training Performance**: Model learns effectively from training data (MAE: 3.17 final).
- **Validation Issues**: Overfitting detected (validation MAE increased to ~5.5 by epoch 20).
- **Data Insights**:
   - Dataset contains 7.6k diverse facial images (final_files/ + labels.csv).
   - Age distribution skewed toward younger ages (common in public facial datasets).

## Further Improvements
- **Overfitting Mitigation**:
   - Apply L1/L2 regularization and dropout layers to reduce model complexity.
   - Implement early stopping to halt training when validation metrics plateau.
- **Data Augmentation**:
   - Expand dataset variety using rotations/flips to improve generalization.
- **Model Tuning**:
   - Adjust learning rate and simplify architecture for better convergence.
- **Deployment Testing**:
   - Pilot in a controlled environment to evaluate real-world performance.
 
![image](https://github.com/user-attachments/assets/ddbd206f-2a97-4c38-90a0-10fd867d7771)

**Libraries**:
```bash
pip install tensorflow pandas numpy matplotlib seaborn
