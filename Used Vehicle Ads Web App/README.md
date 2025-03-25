# Used Vehicle Advertisement Analysis Dashboard

## Overview
This project develops a web application dashboard to analyze used vehicle advertisement data. The tool allows users to explore key metrics, visualize trends in vehicle pricing and features, and filter data interactively. The application is built using Python with Streamlit for the frontend and Plotly Express for visualizations. Key insights include price distributions by vehicle type, mileage trends, and correlations between vehicle features.

The application is deployed on Render and accessible to the public, demonstrating full-stack data science skills from exploratory analysis to cloud deployment.

## Problem(s) to be addressed
- **Data Exploration**: Provide an interactive way to explore used vehicle market trends and patterns.
- **Visualization Needs**: Create dynamic visualizations that help users understand price distributions, mileage trends, and feature correlations.
- **Accessibility**: Make the analysis publicly available through cloud deployment rather than keeping it confined to local notebooks.

## Key Features
- **Interactive Dashboard**:
  - Filter data by vehicle type, price range, and other features using checkboxes and sliders
  - Dynamic visualizations that update based on user selections
- **Data Visualizations**:
  - Histograms showing price distributions by vehicle type
  - Scatter plots revealing relationships between mileage, age, and price
  - Comparative analysis of different vehicle conditions
- **Cloud Deployment**:
  - Fully hosted web application accessible from any device
  - Automated deployment pipeline via GitHub integration

## Key Findings
- **Price Distribution**:
    - Most used vehicles are priced between 5,000 − 20,000
    - Luxury vehicles show a bimodal price distribution
- **Mileage Trends**:
    - Strong inverse correlation between mileage and price for most vehicle types
    - Electric vehicles show different mileage patterns compared to combustion engines
- **Feature Impact**:
    - 4WD vehicles command approximately 15-20% price premium
    - Newer model years maintain value better after 5+ years

## Further Improvements
- **User Authentication**: 
    - Add login functionality to save user preferences and analysis history.
- **Price Prediction**: 
    - Implement a machine learning model to estimate fair market value based on vehicle features.
- **Market Alerts**: 
    - Add functionality to notify users when vehicles matching their criteria become available.

## Prerequisites
To run this project locally, you'll need:
- **Python 3.7+**
- **pip package manager**
- **Web browser** (for local testing)

## Running the app locally:
- **Clone the repository**: 
    - (Insert Following into CLI) git clone https://github.com/Phonz-dot/4_sprint_project.git cd 4_sprint_project
-**Install Dependencies**: 
    - (Insert Following into CLI) pip install -r requirements.txt
- **Run App Locally**: 
    - (Insert Following into CLI) python app2.py
- **Web App Link**: 
    - https://four-sprint-project.onrender.com
