### GameChanger: Predicting Video Game Success through Data Analysis and Strategic Campaign Planning

#### Overview
This project explores a dataset from the video game industry, focusing on user and expert reviews, genres, platforms, and historical sales data to identify patterns that predict game success. By analyzing these patterns, the goal is to spot potential big winners and plan effective advertising campaigns for the online store, Ice. The dataset includes ESRB ratings, which assess game content and assign age ratings, providing valuable insights into the factors influencing game success.

#### Questions/Commands
- **What does this project do?**
  - Filters the dataset to include only video games released up to 2016.
  - Groups video games based on genres, platforms (e.g., Xbox, PlayStation), and ESRB ratings to simplify analysis without compromising research quality.
  - Identifies and excludes outliers with minimal sales or reviews to enhance result accuracy.
  - Calculates and verifies patterns in user and expert reviews, genres, and platforms to identify potential big winners and plan effective advertising campaigns.
  - Performs statistical hypothesis testing to validate relationships between variables, ensuring the findings are robust and reliable.
 
#### Prerequisites
  - Access to the required dataset.
  - Basic understanding of data preprocessing and analysis (EDA/SDA) in Python.
 
#### Functionality
- **Filtering**: Selects video games released up to 2016 for analysis.
- **Grouping Features**: Organizes video games based on genres, platforms (e.g., Xbox, PlayStation), and ESRB ratings for clearer data visualization.
- **Outlier Detection**: Identifies and removes games with minimal sales or reviews to enhance result accuracy.
- **Pattern Analysis**: Calculates and verifies patterns in user and expert reviews, genres, and platforms to spot potential big winners and plan effective advertising campaigns.
- **Statistical Hypothesis Testing**: Formulates and tests hypotheses to validate relationships between variables, ensuring robust and reliable findings.

#### Technologies
To build this project, the following tools and technologies were utilized:
- **Python**
- **Pandas**
- **Plotly**
- **Scipy**
- **Jupyter Notebook** for interactive analysis

#### Installing
Clone the repository and install the required dependencies to run the analysis on your local machine:
```bash
git clone [repo link]
cd [repo name]
pip install -r requirements.txt
jupyter notebook
