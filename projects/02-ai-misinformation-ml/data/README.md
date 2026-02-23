# Data

This folder contains the dataset used in the misinformation classification project.

## Dataset Description

The data is a **synthetically generated social media misinformation dataset** sourced from Kaggle. It contains 500 observations and 31 variables representing a mixture of:

- Temporal metadata (date, time, month, weekday)
- Platform and regional categorical variables
- Engagement metrics (likes, shares, comments, CTR, views)
- Content quality indicators (sentiment, toxicity score, readability)
- Fact-checking signals (credibility score, verification status)
- Raw post text

The target variable, `is_misinformation`, is binary:
- 0 = authentic post  
- 1 = misinformation  

## Important Note

The dataset is synthetic and designed for experimentation and model comparison. While it reflects structural patterns commonly associated with AI-generated misinformation, it does not capture the full complexity of real-world social media behavior.

As a result, model performance in this project should be interpreted as comparative within this dataset, not as a benchmark for real-world misinformation detection.
