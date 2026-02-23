# Source Code

This folder contains the Jupyter Notebook used to implement the full machine learning pipeline for the misinformation classification project.

## File

**4630_Project(1).ipynb**

The notebook includes:

- Exploratory data analysis  
- Data cleaning and feature selection  
- Preprocessing pipeline construction using `ColumnTransformer`  
  - One-hot encoding (categorical features)  
  - Standard scaling (numeric features)  
  - TF-IDF vectorization (text features)  
- Stratified 70/30 train–test split  
- Model training and tuning  
- Performance evaluation (accuracy, ROC-AUC, recall, etc.)  
- Comparative model analysis  

All preprocessing steps are embedded within scikit-learn pipelines to prevent data leakage and ensure consistent transformations across models.

## Reproducibility

To reproduce results:

1. Install required packages:
   - pandas  
   - numpy  
   - scikit-learn  
   - xgboost  
   - matplotlib / seaborn (if used for visualization)  

2. Place the dataset in the appropriate `data/` directory.
3. Run the notebook sequentially from top to bottom.

A fixed random seed is used for the train–test split to ensure reproducibility of results.
