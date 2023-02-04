# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to create a model that can predict whether a loan is high-risk or not.

The dataset used contained the historical lending activity from a peer-to-peer lending services company. Variables within the dataset included: 
- loan size
- interest rate
- borrower income
- debt-to-income ratio
- number of accounts
- derogatory marks
- total debt

The goal was to accurately predict the loan status where 0 = Healthy Loan and 1 = High-Risk Loan. The original dataset contained the information of 75,036 healthy loans and 2500 high-risk loans. 

The steps taken for the analysis were as follows:

1) Split data to create training and testing datasets using `train_test_split`

2) Create a `LogisticRegression` Model

3) Fit model with training dataset

4) Use the model with the testing dataset to predict the loan status

5) Evaluate the performance of model using the following metrics:
  - `balanced_accuracy_score`
  - `confusion_matrix`
  - `classification_report_imbalanced`

6) The training dataset was oversampled and resulted in 56,269 healthy and high-risk loans

7) A second Linear Regression Model was created and fit with the resampled data

8) The second model was used to predict the loan status

9) The performance of the second model was evaluated using the metrics in step 5


## Results

* Machine Learning Model 1:
  * Accuracy: 94.4% 
  * Precision: Healthy Loans - 100%, High-Risk Loans 88%
  * Recall: Healthy Loans - 100%, High-Risk Loans 89%



* Machine Learning Model 2 (with oversampled data):
  * Accuracy: 99.5%
  * Precision: Healthy Loans - 100%, High-Risk Loans 88%
  * Recall: Healthy Loans - 100%, High-Risk Loans 100%

## Summary

Overall I would recommend using the second machine learning model. The accuracy and recall increased and there was no change in precision. 


## Additional Information

Evaluation metric results:

Machine Learning Model 1

<img width="792" alt="Screenshot 2023-02-04 at 3 40 26 PM" src="https://user-images.githubusercontent.com/112917950/216794135-d6306da4-0648-4120-aae7-42fcdc025618.png">


Machine Learning Model 2:

<img width="792" alt="Screenshot 2023-02-04 at 3 40 02 PM" src="https://user-images.githubusercontent.com/112917950/216794125-102a0219-e8fd-4684-b224-bdb04bb97181.png">



