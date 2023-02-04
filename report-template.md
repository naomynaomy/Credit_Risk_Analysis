# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to create a model that can predict whether a loan is high-risk or not.

The dataset used contained the historical lending activity from a peer-to-peer lending services company.

Variables within the dataset included: loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, and total debt. The goal was to accurately predict the loan status where 0 = Healthy Loan and 1 = High-Risk Loan.

The original dataset contained the information of 75,036 healthy loans and 2500 high-risk loans. 

* Describe the stages of the machine learning process you went through as part of this analysis.

The steps taken for the analysis were as follows:

1) Split data to create training and testing datasets.

2) Create a Linear Regression Model

3) Fit model with training dataset

4) Use the model with the testing dataset

5) Evaluate the performance of model using the following metrics:
  - balanced_accuracy_score
  - confusion_matrix
  - classification_report_imbalanced

6) The training dataset was oversampled 


To begin the analysis, the data was first split into two datasets that would be used to train and test using the `train_test_split`. Then, a Linear Regression model was generated and fit with the training variables generated in the first step. Once the model was fit using the training data the model used the features from the test dataset to predict the loan status. The performance of the model was evaluated using the following metrics:

- balanced_accuracy_score
- confusion_matrix
- classification_report_imbalanced






* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
