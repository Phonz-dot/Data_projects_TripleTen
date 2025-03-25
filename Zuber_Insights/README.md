# Zuber Ride-Sharing Analysis: Chicago Passenger Preferences

## Overview
This project analyzes taxi ride data in Chicago to uncover passenger preferences and the impact of external factors (e.g., weather) on ride patterns for Zuber, a new ride-sharing company. The goal is to identify trends in ride frequency, popular neighborhoods, and the effect of weather conditions on ride durations. The analysis involves SQL data processing, exploratory data analysis (EDA), and statistical hypothesis testing using Python with pandas, numpy, and Plotly for visualizations.

## Problem(s) to be addressed
- **Competitor Insights**: Analyze competitor data (e.g., top taxi companies, busy neighborhoods) to inform Zuber’s market strategy.
- **Weather Impact**: Test whether rainy weather affects ride durations, which could influence pricing and driver allocation.
- **Data Gaps**: Link disjointed datasets (e.g., `trips` and `weather_records`) using timestamps to enable cross-factor analysis.

## Key Features
- **SQL Data Processing**: Extracts and aggregates data from multiple tables (`trips`, `cabs`, `neighborhoods`, `weather_records`).
- **Exploratory Analysis**:
  - Identifies top neighborhoods for drop-offs (e.g., The Loop, River North).
  - Ranks taxi companies by ride volume (e.g., Flash Cab leads with 19,558 trips).
- **Hypothesis Testing**: Uses a t-test to confirm that rainy Saturdays significantly increase ride durations to O’Hare International Airport (p-value < 0.05).
- **Visualizations**: Includes interactive bar charts (Plotly) to compare ride volumes by company and neighborhood.

## Prerequisites
To replicate this analysis, you’ll need:
- **Python 3.7+**
- **Jupyter Notebook**

## Key Findings
- **Top Neighborhoods**: 
  - The Loop has the highest average drop-offs (10,727 rides), followed by River North (9,524 rides).
- **Top Taxi Companies**: 
  - Flash Cab dominates with 19,558 trips, nearly double its closest competitor.
- **Weather Impact**: 
  - Rainy Saturdays increase ride durations to O’Hare by an average of 20% (p-value: 6.52e-12), likely due to traffic or slower driving.

## Further Improvements
- **Dynamic Pricing Model**: Integrate weather data to adjust pricing during peak demand (e.g., rainy weekends).
- **Driver Incentives**: Use neighborhood demand patterns to optimize driver placement and bonuses.
- **Extended Weather Analysis**: Investigate other weather conditions (e.g., snow, fog) and their impact on ride frequency.

## Python Libraries:
  ```bash
  pip install pandas numpy scipy plotly