# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* In this report we will use various techniques to train and evaluate a model based on loan risk. We used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

* Following infomation have been used:
Variables considered:
        -Loan size
        -interest rate
        -Borrower's income
        -Debt to income ratio
        -number of accounts the borrower has
        -derogatory marks against the borrower
        -the total debt
        -Loan Status
Data size :77536 borrowers 
Split the Data into Training and Testing Sets:

  Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
  Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
  Split the data into training and testing datasets by using train_test_split.

Create a Logistic Regression Model:
  Fit a logistic regression model by using the training data (X_train and y_train). 
  Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. 
  Evaluate the model’s performance by doing the following:
  Generate a confusion matrix. 
  Generate a classification report. 

## Results

                    First Logistic Regression (Model 1)             Second Logistic Regression (Model2)
Precision (true positives / selected elements)                  
    Healthy Loan        100%                                            100%
    High Risk Loan       87%                                            87%
Recall  (true positive/relevant elements)
    Healthy Loan        100%                                            100%
    High Risk Loan      89%                                             100%
Accuracy                99.148%                                         99.520%

## Summary
Both model identify healthy loan at 100% and Risky Loan at 87%. Both model have accuary rate of 99%. The Model 2 has slightly higher accuracy rate than first model. 

for this model it is more important to find high-risk borrowers (1) based on their obtain information. Risky loan precision rate 87 in both model, the accuracy rate of the second model higher. therefore, it  is recommended that second model should be used to identfy high risk customer.


