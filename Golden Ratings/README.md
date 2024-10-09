### Golden Ratings: Investigating the Impact of Votes on TV Show Ratings During the Golden Age of Television

#### Overview
This project delves into the entertainment industry dataset, focusing on the "Golden Age" of television, which began in 1999 with the release of The Sopranos and continues to this day. The primary aim is to investigate how the number of votes a TV show receives from IMDb users impacts its ratings.

#### Questions/Commands
- **What does this project do?**
  - Filters the dataset to include only shows released in 1999 or later.
  - Groups scores into 1-10 integer buckets to simplify analysis without compromising research quality.
  - Identifies and excludes outliers with few votes to enhance result accuracy.
  - Calculates and verifies the average votes for each score bucket against the initial assumption.

#### Prerequisites
- Access to the required dataset.
- Basic understanding of data manipulation and analysis in Python.

#### Functionality
- **Filtering**: Selects TV shows released from 1999 onwards for analysis.
- **Grouping Scores**: Rounds scores to the nearest integer for clearer data visualization.
- **Outlier Detection**: Identifies and removes scores with an unusually low number of votes.
- **Averages Calculation**: Computes average votes for each score, verifying alignment with the hypothesis.

#### Technologies
To build this project, the following tools and technologies were utilized:
- **Python**
- **Pandas**
- **Jupyter Notebook** for interactive analysis

#### Installing
Clone the repository and install the required dependencies to run the analysis on your local machine:
```bash
git clone [repo link]
cd [repo name]
pip install -r requirements.txt
jupyter notebook
