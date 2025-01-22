# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to evaluate the performance of machine learning models in predicting high-risk loans. The dataset contained financial information such as loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt. The goal was to predict whether a loan would be classified as "healthy" (0) or "high-risk" (1). The target variable, loan_status, showed significant class imbalance with 75,036 loans labeled as "healthy" (0) and only 2,500 labeled as "high-risk" (1).

The machine learning process involved splitting the data into training and testing sets, followed by training the model. The model's performance was evaluated using precision, recall, F1-score, and a confusion matrix to assess its ability to predict both classes, especially the minority class of "high-risk" loans.

## Results

Machine Learning Model:
- Accuracy: 99%
The model correctly predicted 99% of all samples, indicating strong overall performance.

- Precision (for 0 class): 1.00
The model had perfect precision for healthy loans (class 0), with no false positives.

- Recall (for 0 class): 0.99
The model identified 99% of the actual healthy loans.

- Precision (for 1 class): 0.84
For high-risk loans (class 1), 84% of the predictions were correct, with some false positives.

- Recall (for 1 class): 0.94
The model correctly identified 94% of actual high-risk loans.

## Summary

The model performs well overall with 99% accuracy, excelling at predicting healthy loans (0) with perfect precision and high recall. However, for high-risk loans (1), the precision is lower (0.84), meaning some healthy loans are misclassified as high-risk. The model’s performance is suitable if identifying healthy loans is the priority, but improvements in high-risk loan precision could be needed if that is more critical. If reducing false positives for high-risk loans is essential, further adjustments or another model may be needed.
