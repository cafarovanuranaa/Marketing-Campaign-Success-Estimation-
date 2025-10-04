Overview
This project predicts the success of a marketing campaign (response) using customer and campaign data. A Random Forest Classifier is used with preprocessing, model training, evaluation, and feature importance analysis. The model has been deployed and can be applied to new data with the same preprocessing.

Workflow / Steps

1. Data Reading & Exploration

Loaded dataset and checked for missing values
Dropped unnecessary columns: ID, pdays, previous
Encoded target variable result as 0/1 (yes → 0, no → 1)

2. Data Preprocessing & Encoding

Label encoding applied to: job, marital, contact, month, response
Binary features mapped: 0/1

3 Train-Test Split

Split data into train (70%) and test (30%) sets

4. Model Training

Trained Random Forest Classifier with 100 estimators, random state 42

5. Model Evaluation

Metrics calculated for train and test sets: ROC AUC, Gini coefficient, precision, recall
Evaluation done using predicted probabilities and class labels

6. Feature Importance

Identified most important features for campaign success prediction

7. Deployment

Model has been deployed and is operational
New data can be used directly with the same preprocessing and encoding steps
