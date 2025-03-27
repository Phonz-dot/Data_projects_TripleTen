# Megaline Telecom Plan Revenue Analysis

## Overview
This project analyzes the revenue performance of Megaline's two prepaid plans, Surf and Ultimate, using data from 500 customers in 2018. The goal is to determine which plan generates more revenue by examining user behavior, including call duration, text messages, and internet usage. Key findings include revenue comparisons, usage patterns, and statistical hypotheses testing. The analysis is conducted using Python with pandas, numpy, and matplotlib for data visualization.

## Problem(s) to be addressed
- **Revenue Comparison**: The commercial department needs insights into which plan (Surf or Ultimate) generates higher revenue to optimize the advertising budget.
- **User Behavior Analysis**: Understanding how customers use their plans (e.g., call minutes, texts, data consumption) helps identify trends and potential areas for plan adjustments.
- **Data Quality**: The dataset requires cleaning and preprocessing, including handling missing values and converting data types for accurate analysis.

## Key Features
- **Data Cleaning and Preparation**:
  - Handles missing values in the `churn_date` field.
  - Converts date fields (`reg_date`, `call_date`, etc.) to datetime format.
  - Rounds call durations and data usage according to Megaline's policies.
- **Exploratory Analysis**:
  - Compares average call duration, text messages, and internet usage between plans.
  - Analyzes monthly revenue trends for Surf and Ultimate users.
- **Statistical Testing**:
  - Tests hypotheses about revenue differences between plans and regions (e.g., NY-NJ area vs. others).
- **Visualizations**:
  - Includes bar charts, histograms, and boxplots to illustrate usage patterns and revenue distribution.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
**Revenue**:
- Ultimate users generate higher average monthly revenue (72.25) compared to Surf users (60.42).
- Surf users exhibit higher variance in revenue, indicating more variability in their usage and costs.
**Usage Patterns**:
- Surf users frequently exceed plan limits, leading to additional charges.
- Ultimate users generally stay within plan limits due to higher allowances.
**Statistical Insights**:
- The null hypothesis that average revenue between plans is equal was rejected, confirming a significant difference.
- No significant revenue difference was found between users in the NY-NJ area and other regions.

## Further Improvements
**Seasonal Analysis**: 
- Investigate how revenue and usage vary by season (e.g., holiday months).
**Customer Segmentation**: 
- Cluster users by usage behavior (e.g., heavy callers, frequent texters) to tailor marketing strategies.
**Predictive Modeling**: 
- Use historical data to predict future revenue trends or customer churn.

![image](https://github.com/user-attachments/assets/d9154c1b-f443-4130-8571-e7de4b27e47a)

**Libraries**:
  ```bash
  pip install pandas numpy matplotlib scipy
