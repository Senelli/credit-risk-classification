# credit-risk-classification

## Overview of the Analysis
* The purpose of the analysis is to create a machine learning model aimed at comprehending credit lending dynamics and the accompanying risks.
* The dataset contained details such as loan amount, interest rate, borrower earnings, debt compared to income, consumer account count, negative marks on credit history, overall consumer debt, and loan status.
* The variables I attempted to forecast were "Healthy Loan," identified by the value "0," and "High-Risk Loan," identified by the value "1."
* First data was pre-processed by doing the following:
    * The lending_data.csv data from the Resources folder was read into a Pandas DataFrame.
    * The labels set (y) was created from the “loan_status” column, and then the features (X) DataFrame was created from the remaining columns.
    * The data was split into training and testing datasets by using train_test_split.
* Used the Logisitic Regression model then generated a confusion matrix and a classification report.

## Results
* Machine Learning Model 0 (Healthy Loan):
    * The model attained a 99% accuracy, signifying that 99% of the predictions aligned with the actual loan statuses. The precision for predicting healthy loans stood at 100%, indicating that when the model predicted a loan as healthy, it was accurate 100% of the time. The recall score for Healthy Loans was 100%, indicating that the model correctly identified all healthy loans 100% of the time.

* Machine Learning Model 1 (High-Risk Loans Accuracy):
    * The model achieved a 99% accuracy, indicating that 99% of the predictions matched the actual loan statuses. The precision for predicting High-Risk loans stood at 87%, suggesting that when the model predicted a loan as high risk, it was accurate 87% of the time. The recall score for High-Risk Loans was 89%, indicating that the model correctly identified 89% of all high-risk loans.

## Summary
* The model with superior precision, recall, and accuracy is deemed the best, namely the Healthy Risk Loan model. This model had a precision of 100% which means it predicted loans that are of healthy risk 100% of the time and had a recall score of 100% which means that the model was able to recognize loans that are of healthy risk 100% of the time.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Given that all factors studied in the machine learning model are accurate, greater significance would be attributed to predicting instances of "1's (high risk loans)." This doesn't necessarily imply it's the optimal approach, but it's preferable to encounter false positives and delve deeper into understanding how to fix or intervene in such situations rather than solely focusing on "good" values like healthy loans. Relying solely on healthy loan assessments could lead to potential issues such as loan defaults, setting oneself up for failure.