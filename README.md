# BootCamp_credit-risk-classification

## Overview of the Analysis

#### Purpose of the Analysis:

The purpose of this analysis is to assess credit risk for a lending company. The analysis aims to develop a machine learning model, specifically a logistic regression model, to predict the likelihood of loans being healthy or high-risk. The company needs to make informed decisions about loan approval based on the credit risk assessment to minimise potential losses and maintain a healthy loan portfolio.

#### Financial Information in the Data:

The data used for this analysis contains financial information related to loans. The key target variable is the "loan_status," which indicates whether a loan is classified as healthy (0) or high-risk (1). The financial information includes various features such as loan amount, interest rate, annual income of borrowers, debt-to-income ratio, and more. The goal is to predict the loan status based on these financial attributes.

#### Basic Information about Variables:

- "loan_status" is the target variable, and its value counts would typically show the distribution of healthy and high-risk loans.
- The features include various financial and personal attributes of borrowers, which are used to predict loan status.

#### Stages of the Machine Learning Process:

1. Data Preprocessing:
   - Reading the data from the CSV file and creating a Pandas DataFrame.
   - Creating labels (y) from the "loan_status" column and features (X) from the remaining columns.
   - Splitting the data into training and testing datasets to train and evaluate the model.

2. Model Development:
   - Utilising a Logistic Regression model to predict loan status.
   - Fitting the model using the training data (X_train and y_train).
   - Making predictions on the testing data (X_test) to evaluate the model's performance.

3. Model Evaluation:
   - Generating a confusion matrix to understand the model's ability to correctly classify healthy and high-risk loans.
   - Creating a classification report to provide detailed metrics such as accuracy, precision, recall, and F1-score, which assess the model's performance.

4. Credit Risk Analysis Report:
   - Providing an overview of the analysis and its purpose.
   - Describing the accuracy, precision, and recall scores of the machine learning model.
   - Summarising the results and justifying whether the model should be recommended for use by the company.

#### Methods Used:

The primary method employed in this analysis is Logistic Regression, a classification algorithm used to obtain an odds ratio based on individual characteristics. It is used to predict the loan status as either healthy or high-risk based on the financial and personal attributes of borrowers.

## Results

#### Balanced Accuracy Scores:
   
Balanced accuracy is the average recall for each class and are calculated as follows:
- Healthy Loan = 0.99
- High-Risk Loan = 0.91
- Balanced Accuracy = (0.99 + 0.91) / 2 = 0.95

#### Precision and Recall Scores:

Precision is a metric that indicates the accuracy of positive predictions, while recall measures the proportion of actual positives correctly identified by the model.

For the "healthy loan" class:
- Precision = 1.00: This means that when the model predicts a loan as a healthy loan, it is correct 100% of the time.
- Recall = 0.99: The model correctly identifies 99% of actual healthy loans.

For the "high-risk loan" class:
- Precision = 0.85: When the model predicts a loan as a high-risk loan, it is correct 85% of the time.
- Recall = 0.91: The model correctly identifies 91% of actual high-risk loans.

#### F1-Score:

The F1-score is the mean of precision and recall. 
- The F1-score for "healthy loan" is 1.00, indicating high accuracy and recall.
- The F1-score for "high-risk loan" is 0.88, indicating a trade-off between precision and recall for this class.

## Summary

These metrics collectively suggest that the machine learning model performs well in identifying healthy loans with high precision and recall. It also has a reasonably good balance between precision and recall for high-risk loans. The balanced accuracy of 0.95 indicates that the model is effective in accounting for class imbalance and provides a good overall assessment of its performance.
