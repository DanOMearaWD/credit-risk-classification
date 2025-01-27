# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to evaluate the performance of machine learning models in predicting high-risk loans. The dataset contained financial information such as:

- **loan_size**
- **interest_rate**
- **borrower_income**
- **debt_to_income**
- **num_of_accounts**
- **derogatory_marks**
- **total_debt**

The goal was to predict whether a loan would be classified as "healthy" (0) or "high-risk" (1). The target variable, **loan_status**, showed significant class imbalance with:

- 75,036 loans labeled as "healthy" (0)
- 2,500 loans labeled as "high-risk" (1)

The machine learning process involved:
1. Splitting the data into training and testing sets.
2. Training the model.
3. Evaluating model performance using metrics like precision, recall, F1-score, and a confusion matrix, with a focus on predicting the minority class of "high-risk" loans.

## Results

### Machine Learning Model Performance

- **Accuracy:** 99%
  - The model correctly predicted 99% of all samples, indicating strong overall performance.
- **Precision (Class 0 - Healthy Loans):** 1.00
  - Perfect precision for healthy loans, with no false positives.
- **Recall (Class 0 - Healthy Loans):** 0.99
  - Identified 99% of actual healthy loans.
- **Precision (Class 1 - High-Risk Loans):** 0.84
  - Precision measures the proportion of predicted high-risk loans that are actually high-risk loans. A precision of 0.84 means that:
    - 84% of loans classified as high-risk were actually high-risk.
    - 16% (1 - 0.84) were false positives (healthy loans misclassified as high-risk).
- **Recall (Class 1 - High-Risk Loans):** 0.94
  - Correctly identified 94% of actual high-risk loans.

## Summary

### Key Insights
- **Strengths:**
  - Highly effective at identifying healthy loans (perfect precision and high recall).
  - High recall for high-risk loans ensures most actual high-risk loans are correctly identified.
- **Limitations:**
  - Lower precision for high-risk loans indicates a notable proportion of false positives.

The model is suitable if identifying healthy loans is the priority. However, further improvements in high-risk loan precision may be required.
