# 17_1_model_comparison


# Bank Term Deposit Subscription Prediction

## Problem Statement
Financial institutions need to identify customers most likely to subscribe to a term deposit in order to optimize marketing resources and improve conversion rates. This project uses the **bank-additional.csv** dataset to predict subscription outcomes based on demographic, financial, and campaign interaction data.

## Solution Approach
1. **Deep Exploratory Data Analysis**  
   - Descriptive and inferential statistics (t-tests, chi-squared tests)  
   - Rich visualizations: correlation heatmap, pairplots, violin/swarm plots, density and bar charts.

2. **Data Preprocessing**  
   - Encoding categorical variables  
   - Feature scaling  
   - Handling class imbalance using **SMOTE**

3. **Modeling & Hyperparameter Tuning**  
   - Evaluated six classifiers:  
     - Support Vector Machine (SVM)  
     - Decision Tree  
     - Logistic Regression  
     - K-Nearest Neighbors (KNN)  
     - Random Forest  
     - XGBoost  
   - Grid search with 5‑fold cross-validation on resampled data

4. **Model Evaluation**  
   - Cross‑validation F1-scores comparison  
   - ROC and Precision‑Recall curve analyses  
   - Confusion matrices grid for detailed error inspection  
   - Interpretation of logistic regression coefficients and feature importances for tree‑based models

## Key Insights
- **XGBoost** and **SVM** achieved the highest F1-scores and ROC AUC, making them strong candidates for deployment.  
- **Logistic Regression** offers valuable interpretability, highlighting key predictors such as **age**, **call duration**, and **euribor3m**.  
- **Decision Tree** and **Random Forest** provide transparent rules and feature importances, useful for business heuristics.  
- **KNN** remains competitive but is less scalable for large datasets.


## Jupyter Notebook Location
All code, analysis, and visualizations are provided in the Jupyter Notebook:

https://github.com/psnana-us/17_1_model_comparison/blob/main/final_deep_comprehensive_analysis.ipynb

