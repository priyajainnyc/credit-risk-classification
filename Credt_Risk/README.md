# credit-risk-classification
Homework 20 for the supervised machine learning module of Datavis bootcamp

# Credit Risk Analysis Report

## Overview of the Analysis

**Description**

This analysis aims to leverage various machine learning techniques to train and evaluate the performance of Logistic Regression Models in identifying the creditworthiness of borrowers. The models were trained using different methods, and their performances were compared to determine the better-performing model. The predictive variables in the model are the labels 0 (healthy loan) and 1 (high-risk loan).

In the process of constructing the models, the dataset was split into features and labels, and further divided into training and testing sets. 
* Machine Learning Model 1 was built by instantiating a logistic regression model and training with the original training sets (X_train, y_train), fitting it to the training sets, and using it to generate predictions. 
* Machine Learning Model 2 was created by resampling the original training data using the RandomOverSampler module, instantiating a logistic regression model and fitting the resampled training sets (X_resample, y_resample) to the model, and generating predictions.

The performance of each model was evaluated based on the balance accuracy score, the confusion matrix, as well as the precision score, recall score, and f1-score in the classification report.

## Results

* **Machine Learning Model 1:**

  Model 1, trained on the original data, gives an accuracy of 94.4% in predicting the 2 labels. The model is very good at predicting the healthy loans, with both precision and recall scores of 1.00. However, the model's performance in predicting the high-risk loans can be improved. The precision score for high-risk loans is 0.87, indicating that only 87% of actual high-risk loans were correctly predicted. The recall score for high-risk loans is 0.89, indicating that the model only identified 89% of all high-risk loans in the dataset.

* **Machine Learning Model 2:**

  Model 2 , trained on the resampled data, has an accuracy of 99.6% in predicting the 2 labels. The model peforms well at predicting the healthy loans, with both precision and recall scores of 1.00. The precision score for high-risk loans remains at 0.87, but the recall score has improved to 1.00, indicating that the model can now predicting all high-risk loans in the dataset.

## Summary
    
Based on the analysis, it appears that Model 2 outperforms Model 1 in predicting high-risk loans and has an overall higher accuracy in predicting both labels. Specifically, Model 2 achieved a relatively high precision in predicting high-risk loans while correctly identifying all high-risk loans in the dataset, which is considered a relatively good performance in this context. Therefore, I would recommend using Model 2 in identifying high-risk loans and overall better accuracy in predicting labels.
