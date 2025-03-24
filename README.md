# Credit Risk Analysis - Logistic Regression Model

## Overview

This module focuses on building and evaluating a **Logistic Regression** model to predict credit risk for loan applicants. The goal is to classify loan applicants as either **healthy borrowers (0)** or **high-risk borrowers (1)** based on their financial and demographic information. This is crucial for financial institutions to reduce losses and make informed lending decisions.

## Purpose

The purpose of this analysis is to:
- Build a machine learning model that predicts whether a loan applicant is a high-risk borrower.
- Evaluate the model's performance using metrics such as **accuracy**, **precision**, **recall**, and **AUC-ROC**.
- Provide recommendations for using the model in a real-world credit risk assessment scenario.

## Requirements

To run this module, we will need the following libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

## Data

The dataset includes various features about loan applicants, such as:
- Applicant’s age
- Income
- Loan amount
- Previous loan history
- Other financial and demographic details

The **target variable** is **loan status**, which can take two values:
- **0**: Healthy loan (low-risk borrower)
- **1**: High-risk loan (high-risk borrower)

## Steps

### 1. Data Preprocessing
- Cleaned the data by handling missing values.
- Scaled the features to ensure better model performance.
  
### 2. Model Training
- The **Logistic Regression (LR)** model was trained on the prepared dataset using **X_train** and **y_train**.

### 3. Model Evaluation
- Evaluated the model’s performance using the following metrics:
  - **Accuracy**: Percentage of correct predictions.
  - **Precision**: The proportion of positive predictions that were correct.
  - **Recall**: The proportion of actual positives that were correctly identified.
  - **F1-Score**: A balance between precision and recall.
  - **AUC-ROC**: Measures how well the model distinguishes between the two classes.

## Results

### Logistic Regression Model
- **Accuracy:** 99%
- **Precision for Class 1 (high-risk):** 87%
- **Recall for Class 1 (high-risk):** 98%
- **F1-Score for Class 1 (high-risk):** 92%
- **AUC (Test):** 99.6%

#### Key Insights:
- **Accuracy**: The model performs very well with an accuracy of 99%, indicating it classifies most applicants correctly.
- **Precision & Recall**: The model has a good balance, with high recall (98%) for high-risk loans, ensuring that most high-risk borrowers are identified. However, precision is slightly lower at 87%, meaning some healthy loans (0) may be misclassified as high-risk.
- **AUC**: The model's AUC of 99.6% shows it does a great job distinguishing between healthy and high-risk loans.

## Summary

- **Logistic Regression** is the most effective model in this analysis, providing an excellent balance of performance, interpretability, and simplicity.
- Logistic Regression works well for binary classification tasks like this one, especially when classifying data with an imbalance between the classes (as in this case with healthy vs. high-risk loans).
- **Logistic Regression** is recommended for use in predicting credit risk. While there is a slight trade-off between precision and recall for high-risk loans, the high recall rate is more important for financial institutions to avoid missing high-risk applicants.


