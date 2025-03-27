# TV Show Ratings Analysis: The Golden Age of Television  

## Overview  
This project analyzes the relationship between IMDb ratings and vote counts for TV shows released during the "Golden Age" of television (1999-present). The research investigates whether highly-rated shows from this era receive more votes than lower-rated ones, using data preprocessing and statistical analysis techniques.  

## Problem(s) to be Addressed  
- Investigates the correlation between viewer engagement (vote counts) and perceived quality (ratings) during television's modern "Golden Age"  
- Provides insights for content creators and platforms about audience participation patterns  

## Key Features  
- **Data Cleaning Pipeline**:  
  - Standardized inconsistent column naming  
  - Handled missing values (6% of data)  
  - Removed 6,994 duplicate entries  
  - Corrected 6 variations of "SHOW" to a single format  
- **Focused Analysis**:  
  - Examined only TV shows from 1999-present  
  - Implemented robust outlier detection  
- **Statistical Analysis**:  
  - Grouped ratings into buckets  
  - Calculated average votes per rating  

## Prerequisites  
**Software Requirements**:  
- Python 3.7+  
- Jupyter Notebook  

## Key Findings
- The research confirms that highly-rated shows (scores 7-9) during television's "Golden Age" receive significantly more votes than lower-rated programs
- The anomaly at score 4 (higher votes than scores 5-6) warrants further investigation
- The dataset represents 94% of original data after cleaning, ensuring reliable results

## Improvements
- Implement visualizations (matplotlib/seaborn) to better illustrate the rating-vote relationship
- Investigate the anomalous score-4 results to identify potential data quality issues
- Expand analysis to examine genre-specific patterns in ratings and votes

![image](https://github.com/user-attachments/assets/7872d8c2-58ec-40aa-949f-c45f14c3abb5)


**Python Libraries**:  
```bash
pip install pandas numpy
