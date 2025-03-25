# Instacart Grocery Shopping Habits Analysis

## Overview
This project analyzes customer shopping habits using Instacart's grocery delivery platform data. The goal is to clean the dataset, remove duplicates and missing values, and uncover insights into when, how often, and what customers buy. Key findings include peak shopping times, popular products, and reordering patterns. The analysis is conducted using Python with pandas, numpy, and matplotlib for data visualization.

## Problem(s) to be addressed
- **Data Quality**: The dataset contains intentional duplicates and missing values that need to be cleaned for accurate analysis.
- **Customer Insights**: Understanding shopping habits (e.g., peak times, popular products) can help Instacart optimize inventory, delivery logistics, and marketing strategies.
- **Behavioral Trends**: Analyzing reorder rates and order frequency can reveal customer loyalty and preferences.

## Key Features
- **Data Cleaning**: Removes duplicate and missing values across multiple tables (`instacart_orders`, `products`, `order_products`).
- **Exploratory Analysis**: Investigates:
  - Peak shopping hours and days (e.g., most orders occur between 9 AM–3 PM, Saturdays are busiest).
  - Popular products (e.g., bananas, organic strawberries).
  - Reorder patterns (e.g., 30-day wait between orders is most common).
- **Visualizations**: Includes histograms and bar charts to illustrate trends.

## Prerequisites
To run this project, you'll need:
- **Python 3.7+**
- **Jupyter Notebook**
- **Libraries**:

## Key Findings
- Peak Shopping Times:
    - Most orders are placed between 9 AM and 3 PM.
-   Saturday is the busiest day, followed by Sunday.
- Popular Products:
    - Top items are fruits and vegetables (e.g., bananas, organic spinach).
- Order Frequency:
    - 30 days is the most common gap between orders.
    - Most customers place fewer than 5 orders total.
- Reorder Behavior:
    - Over 60% of products in orders are reorders.

## Further Improvements
- Seasonal Analysis: Investigate how holidays or seasons affect shopping habits (e.g., holiday spikes in organic produce).
- Customer Segmentation: Cluster users by purchase frequency or product preferences to tailor promotions.
- Inventory Recommendations: Use reorder data to predict stock needs for high-demand products.

## Python Libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn