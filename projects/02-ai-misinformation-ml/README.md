# Predicting AI-Generated Misinformation in Social Media Posts

STAT 4630 Machine Learning Project  
Thad Felten  

## Overview

This project evaluates machine learning models for detecting AI-generated misinformation in social media posts. The objective is to compare linear, tree-based, and ensemble methods under a unified preprocessing and evaluation pipeline.

The dataset contains 500 synthetic social media posts with 31 variables spanning metadata, engagement metrics, content quality indicators, and text features. The target variable, `is_misinformation`, is binary (0 = authentic, 1 = misinformation).

---

## Data Characteristics

The predictors include:

- Temporal features (date, time, weekday, month)
- Categorical metadata (platform, region, language, topic)
- Engagement metrics (likes, shares, comments, CTR, views)
- Content quality indicators (sentiment, toxicity, readability)
- Fact-checking signals (credibility score, verification status)
- Raw post text

Exploratory analysis showed:

- No missing values  
- Near-balanced classes (~53–54% misinformation)  
- Weak linear correlation between predictors and the response  
- High-dimensional and weakly linearly separable feature space  

---

## Preprocessing Pipeline

All preprocessing steps were implemented inside scikit-learn pipelines to prevent data leakage and ensure consistent transformations across models.

- One-hot encoding for categorical variables  
- Standard scaling for numeric variables  
- TF-IDF (unigrams and bigrams, capped vocabulary) for text  
- 70/30 stratified train–test split  
- Reproducible random seed  

Identifier and non-predictive metadata fields were excluded from modeling.

---

## Models Evaluated

- Logistic Regression (baseline and tuned)
- Decision Tree (depth-constrained)
- Random Forest
- XGBoost (baseline and tuned)
- Linear Support Vector Machine

All models were trained using the same preprocessing structure for fair comparison.

---

## Results

Model performance was only modestly above random guessing, highlighting the difficulty of misinformation detection in this dataset.

- Tuned Logistic Regression achieved the highest accuracy.
- Tuned XGBoost performed best on ranking metrics (ROC-AUC / PR-AUC).
- Random Forest achieved the highest recall.

Results suggest nonlinear structure in the data but relatively weak predictive signals overall.

---

## My Role

This project was completed collaboratively.

My primary contributions focused on:

- Model comparison and performance evaluation  
- Interpretation of tradeoffs between accuracy, recall, and AUC  
- Error analysis and diagnostic reasoning  
- Writing structured conclusions and identifying future modeling directions  
- Contributing to portions of the coding pipeline  

---

## Future Directions

- Richer text representations (embeddings or transformer-based models)
- Additional feature engineering for interaction effects
- Larger or more complex datasets
- Neural network architectures for high-dimensional nonlinear patterns
