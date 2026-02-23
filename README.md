# Thad Felten — Applied Statistics & Machine Learning Portfolio

I’m a Statistics and Economics student focused on applied modeling, data visualization, and machine learning. My work emphasizes structured analysis, careful interpretation, and reproducible workflows.

---

## How the NBA Became a 3-Point League  
STAT 3280 Final Project

### Central Question
How has the three-point shot reshaped NBA offenses over time, and in the modern NBA, is leaning into the three-point shot associated with winning?

### Overview
This project traces the evolution of NBA offensive strategy across eras, examining league-wide efficiency trends, changes in shot allocation, stylistic divergence across teams, and how these shifts relate to success.

The analysis progresses from league-wide transformation to team-level and player-level adaptation, ultimately connecting strategic change to championship outcomes.

### Key Components

- League-wide offensive rating trends (points per 100 possessions)
- Examination of pace and true shooting percentage as partial explanations
- Season-normalized (z-score) three-point attempt rates to account for changing league context
- Era-separated analysis of three-point volume vs. win percentage
- Binned comparisons of win distributions by three-point attempt volume
- Team-level variance analysis in three-point attempts, pace, and offensive rating
- Champion comparisons relative to league averages
- Player usage rate shifts by position over time

### Findings

- Offensive improvement is not fully explained by pace or raw efficiency increases.
- The primary shift is in shot allocation toward higher-value attempts, particularly three-pointers.
- In earlier eras, three-point volume was weakly related to winning.
- In the modern era, higher three-point attempt rates are clearly associated with stronger win percentages.
- Most champions since 2000 take more threes than league average, often pairing strong defense with elevated three-point volume.

The project emphasizes association rather than causation and discusses confounding factors such as roster quality.

### Tools

- R and R Markdown  
- Plotly for interactive visualizations  
- Shiny applications for team comparison and team playstyle analysis  
- Tableau for embedded visualizations  
- Reproducible season-normalized metrics  

Project folder: `projects/01-nba-visualization`

---

## Predicting AI-Generated Misinformation in Social Media Posts  
STAT 4630 Machine Learning Project

### Problem
Can machine learning models distinguish between authentic posts and AI-generated misinformation?

### Dataset

- Synthetic misinformation dataset (Kaggle)  
- 500 posts, 31 variables  
- Mixed feature types:
  - Temporal features (date, time, day of week)
  - Categorical metadata (platform, region, language, topic)
  - Engagement metrics (likes, shares, comments, CTR, views)
  - Content quality indicators (sentiment, toxicity, readability)
  - Fact-checking signals (credibility score, verification status)
- Target variable: `is_misinformation` (binary)

Exploratory analysis showed no missing data, near-balanced classes, weak linear correlations with the response, and a high-dimensional feature space.

### Preprocessing

- One-hot encoding for categorical variables  
- Scaling numeric features  
- TF-IDF representation of text (unigrams and bigrams)  
- 70/30 stratified train-test split  
- Full preprocessing embedded within scikit-learn pipelines to prevent data leakage  

### Models Evaluated

- Logistic Regression (L2-regularized baseline and tuned)
- Decision Tree (depth-limited)
- Random Forest
- XGBoost (baseline and tuned)
- Linear SVM

### Results

- Tuned Logistic Regression achieved the highest accuracy.
- Tuned XGBoost performed best on ranking metrics (ROC-AUC / PR-AUC).
- Random Forest achieved the highest recall.
- Overall performance was only slightly above random guessing.

The results suggest weak linear separability and dispersed predictive signals. Nonlinear and ensemble methods provided modest gains, but the task remains inherently difficult in this dataset.

### My Contributions

This project was completed collaboratively.

My primary contributions focused on:

- Model comparison and evaluation  
- Interpretation of performance tradeoffs (accuracy, recall, AUC)  
- Error analysis and diagnostic reasoning  
- Translating results into structured conclusions and next steps  
- Contributing to portions of the coding and experimental design  

### Future Directions

- Richer semantic representations (embeddings or transformers)
- Additional feature engineering for interaction effects
- Larger or more complex datasets
- Neural network architectures for high-dimensional nonlinear patterns

Project folder: `projects/02-ai-misinformation-ml`

---

## Technical Skills Demonstrated

- End-to-end machine learning pipelines  
- Cross-validation and hyperparameter tuning  
- Text feature engineering (TF-IDF)  
- Tree-based ensembles and boosting  
- High-dimensional data handling  
- Interactive data visualization  
- Reproducible analytical workflows  
- Statistical interpretation beyond raw accuracy metrics  
