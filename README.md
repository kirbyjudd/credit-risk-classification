# Module 12 challenge - credit-risk-classification
# Background
In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

# Module 12 Report
## Overview of the Analysis

- Our goal was to build a model that can identify the creditworthiness of borrowers and predict the loan status as a healthy loan or high-risk loan. 
- The purpose of this analysis was to evaluate a model based on loan risk using the financial information dataset of historical lending activity from a peer-to-peer lending services company. 

The stages I went through in the machine learning process include:
1. Split the data into training and testing sets
2. Create a Logistic Regression Model with the Original Data and save the predictions
3. Evaluate the model's performance using the accuracy score, confusion matrix, and classification report.

Some of the methods used included creating a Logistic Regression model and using RandomOverSampler to resample the data so it was not imbalanced.

## Results

* Machine Learning Model 1: (Original Data)
  * Model 1 had a balanced accuracy score of 0.95. The 0 (healthy loan) had a precision score of 1.00 and a recall score of .99 while the 1 (high-risk loan) had a precision score of 0.85 and a recall score of .91.
  * This model is less accurate when predicting high-risk loans when compared to the healthy loan based on the lower precision and recall scores
  * The model has imbalanced data so the scores would need to be resampled in order to get an accurate model



* Machine Learning Model 2: (Resampled Data)
  * Model 2 had a balanced accuracy score of 0.99. The 0 (healthy loan) had a precision score of 1.00 and a recall score of 0.99 while the 1 (high-risk loan) had a precision score of 0.84 and a recall score of .99.
  * The recall score improved dramatically for the high-risk loan when using the Resampled Data.
  * Because of the increase in recall score, the model is better at predicting high-risk loans than the original model.

## Summary

The initial Logistic Regression model had very nice-looking accuracy scores, however, the data was imbalanced as there were far more 0 (healthy loans) than there were 1 (high-risk loans). After resampling the data, we improved the Logistic Regression models recall for the high-risk loan and kept the high accuracy scores. I would recommend using the second resampled Logistic regression model, as it takes into account the imbalanced data and has a very accurate fit.

## File Location

The main notebook is located in the "Credit_Risk" folder and is called 'credit_risk_classification.ipynb'.
The report is also in the "Credit_Risk" folder and is called 'Module 12 Report.md'.
