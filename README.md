# Task-4-Churn-Prediction-Model
Task 4: Churn Prediction Model

*NAME* : KAVANASHREE

*COMPANY NAME* : SaiKET SYSTEMS

*INTERN CODE* : SKS/A2/C24561

*PROJECT DESCRIPTION*: 

This project focuses on building a machine learning model to predict customer churn using logistic regression. Customer churn refers to customers leaving a service or subscription, and predicting it helps businesses take proactive measures to retain customers.

Steps Involved
1.Data Loading & Exploration

-The dataset (Telco_Customer_Churn_Dataset.csv) is loaded using Pandas.

-Basic dataset information (shape, first few rows) is displayed to understand the structure.

2.Data Preprocessing

-A numeric column (Churn_numeric) is created by mapping "Yes" to 1 and "No" to 0 for binary classification.

-Features (X) and target (y) are separated, dropping irrelevant columns like customerID.

-Categorical and numerical features are identified for transformation.

3.Feature Engineering

-Numerical features (tenure, MonthlyCharges, TotalCharges) are standardized using StandardScaler.

-Categorical features (e.g., gender, Contract) are one-hot encoded using OneHotEncoder.

-Data is split into training (80%) and testing (20%) sets.

4.Data Cleaning

-Non-numeric values in numerical columns are checked and cleaned.

-Missing values are filled with the median of the respective column to avoid bias.

5.Model Training

-A logistic regression model is built using scikit-learn with balanced class weights to handle imbalanced data.

-The model is trained on the preprocessed training data.

6.Model Evaluation

-Predictions are made on the test set, and key metrics (accuracy, precision, recall, F1-score, ROC AUC) are calculated.

-A confusion matrix visualizes true vs. predicted churn.

-ROC curve and precision-recall curve assess model performance.

7.Results & Insights

-The model achieves 75% accuracy, with 83% recall (identifying true churn cases well) but lower precision (52%), indicating some false positives.

-The ROC AUC score (86%) suggests good discriminatory power.
