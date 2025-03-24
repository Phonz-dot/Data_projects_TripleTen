# Age Determination for Alcohol Usage

## Overview  
This project was developed for the supermarket chain Good Seed to help them adhere to alcohol laws by ensuring they do not sell alcohol to underage individuals. Using a dataset of 7,591 facial images with corresponding age labels, a deep learning model was trained to predict a person's age from their photo. The goal is to integrate this model into their point-of-sale systems to automatically verify a customer's age before completing an alcohol purchase.

### Key Features  
- **Data Preprocessing**: Cleaned and organized the dataset for analysis.  
- **Exploratory Data Analysis (EDA)**: Analyzed the distribution of ages in the dataset to understand key trends.  
- **Model Training**: Built and trained a neural network using ResNet50 as a backbone for age prediction.  
- **Validation**: Evaluated the model's performance using Mean Absolute Error (MAE) to ensure accuracy.    

---

## Prerequisites  
To run this project, you will need:  
- Python 3.7 or higher  
- TensorFlow 2.x  
- Pandas, Matplotlib, and other standard data science libraries  
- GPU support (recommended for faster training)  

---

## Technologies  
- **Deep Learning**: TensorFlow, Keras  
- **Model Architecture**: ResNet50 (pretrained on ImageNet) with custom dense layers  
- **Data Handling**: Pandas for CSV processing, ImageDataGenerator for efficient image loading  
- **Visualization**: Matplotlib for EDA and performance metrics  

---

### Findings  
- The dataset had a mean age of 31.2 years and was slightly positively skewed.  
- The model achieved a training MAE of 3.17 but showed signs of overfitting, with validation MAE fluctuating around 6-8.  
- Factors like lighting, facial expressions, and accessories (e.g., glasses, hats) may impact prediction accuracy.

---

## Installation  
1. Clone the repository:  
   ```bash  
   git clone [repository-url]  
