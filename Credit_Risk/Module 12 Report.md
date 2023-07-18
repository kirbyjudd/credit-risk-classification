# Module 12 Report

## Overview of the Analysis

- Our goal was to build a model that can identify the creditworthiness of borrowers and predict the loan status as a healthy loan or high-risk loan. 
- The purpose of this analysis was to evaluate model based on loan risk using the finincial information dataset of historical lending activity from a peer-to-peer lending services company. 

The stages I went through in the machine learning process include:
1. Split the data into training and testing sets
2. Create a Logistic Regression Model with the Original Data and save the predictions
3. Evaluate the models performance using accuracy score, confusion matrix and classification report.

Some of the methods used included creating Logistic Regression model and using RandomOverSampler to resample the data so it was not imbalanced.

## Results

* Machine Learning Model 1: (Original Data)
  * Model 1 had a balanced accuracy score of 0.95. The 0 (healthy loan) had a precision score of 1.00 and recall score of .99 while the 1 (high-risk loan) had a precision score of 0.85 and recall score of .91.
  * This model is less accurate when prediction high-risk loans when compared to the healthy loan based on the lower precision and recall scores
  * The model has imbalanced data so the scores would need to be reasample in order to get an accurate model



* Machine Learning Model 2: (Resampled Data)
  * Model 2 had a balanced accuracy score of 0.99. The 0 (healthy loan) had a precision score of 1.00 and recall score of 0.99 while the 1 (high-risk loan) had a precision score of 0.84 and recall score of .99.
  * The recall score improved dramatically for the high-risk loan when using the Resampled Data.
  * Because of the icnrease in recall score, the model is better at prediction high-risk loans than the origianl model.

## Summary

The initial Logistic Regression model had very nice looking accuracy scores, however, the data was imbalanced as there were far more 0 (healthy loans) than there were 1 (high-risk loans). After resampling the data, we improed the Logistic Regression models recall for the high-risk loan and kept the high accuracy scores. I would reccomend using the second resampled Logistic regression model, as it takes into account the imbalanced data and has a very accurate fit.