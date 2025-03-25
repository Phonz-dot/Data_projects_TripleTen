# Video Game Sales Analysis

## Overview
This project analyzes video game sales data to identify patterns that determine a game's success. The goal is to uncover trends in platform performance, genre popularity, and regional preferences to help plan effective advertising campaigns. The analysis covers data from 1985-2016, with a focus on recent trends (2013-2016) for actionable insights. Key findings include leading platforms, profitable genres, and regional differences in gaming preferences. The analysis was conducted using Python with pandas, numpy, and plotly for visualization.

## Problem(s) to be addressed
- **Data Quality**: The dataset contains missing values in critical columns (e.g., user scores, release years) that needed cleaning.
- **Platform Analysis**: Identifying which gaming platforms are growing or declining helps allocate advertising resources effectively.
- **Regional Preferences**: Understanding differences in genre popularity across North America, Europe, and Japan enables targeted marketing.
- **Review Impact**: Determining how critic and user scores correlate with sales helps prioritize review-based marketing strategies.

## Key Features
- **Data Cleaning**:
  - Handled missing values in `user_score`, `critic_score`, and `year_of_release`
  - Converted data types (e.g., string scores to numeric)
  - Added calculated `total_sales` column
- **Exploratory Analysis**:
  - Platform lifecycle analysis (average platform lasts ~8 years)
  - Identified top-performing platforms (PS4, XOne, 3DS)
  - Regional preference analysis:
    - NA/EU: Action/Shooter games on consoles
    - JP: Role-Playing games on handhelds
  - Review impact analysis (critic scores correlate more strongly with sales)
- **Visualizations**:
  - Interactive line/bar charts showing platform trends
  - Box plots comparing sales across genres
  - Scatter plots analyzing review-score relationships

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Platform Trends**:
  - Average platform lifespan is 8 years
- **Current leading platforms**: 
  - PS4, XOne, 3DS
- **Growing platforms**: 
  - PS4, XOne
- **Declining platforms**: 
  - PC, WiiU, 3DS, PSV
- **Genre Performance**:
  - Most profitable genres globally: Shooter, Platform, Racing
- **Regional differences**:
  - NA/EU: Action and Shooter dominate
  - JP: Role-Playing and Platform games lead
- **Review Impact**:
  - Critic scores show moderate positive correlation with sales (r=0.41)
  - User scores show very weak correlation (r=-0.08)
  - ESRB ratings have minimal influence on sales

## Further Improvements
- **Platform-Specific Analysis**:
  - Fix platform lifecycle calculations by incorporating hardware release dates to achieve more accurate platform longevity estimates.
- **Temporal Analysis**:
  - Implement time-series forecasting using ARIMA to predict 2017 sales based on historical trends.
- **Review Sentiment**:
  - Add natural language processing of user reviews to supplement numerical scores for better prediction accuracy.

- **Libraries**:
  ```bash
  pip install pandas numpy matplotlib plotly scipy