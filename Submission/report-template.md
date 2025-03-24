#  Credit Risk Analysis Report

## Overview of the Analysis

The goal of this analysis was to build and test machine learning models to predict whether a loan applicant is a **healthy borrower (0)** or a **high-risk borrower (1)**. This is important for financial institutions because predicting high-risk loans can help reduce losses and make better lending decisions.

The data provided information about each loan applicant, such as their financial details, to predict whether they will pay back the loan or default. The target variable is the loan status, where:
- **0** means the borrower is healthy (low-risk).
- **1** means the borrower is high-risk.

The process of the analysis included:
1. **Data Cleaning and Preparation:** We cleaned the data, handled any missing values, and scaled the features for better model performance.
2. **Model Selection:** There are different machine learning model like **Logistic Regression**, **Support Vector Machine (SVM)**, **K-Nearest Neighbors (KNN)**, **XGBoost**, and **LightGBM** for supervised learning. We used **Logistic Regression** for this module to predict the loan status.
3. **Model Training:** We trained the models using the training data.
4. **Model Evaluation:** We evaluated the models using metrics such as **accuracy**, **precision**, **recall**, and **AUC-ROC score**.

## Result

#### **Logistic Regression (LR)**

- **Accuracy:** 99% (both on training and testing data)
- **Precision:** 
    - Healthy loans (0): 100%
    - High-risk loans (1): 87%
- **Recall:** 
    - Healthy loans (0): 99%
    - High-risk loans (1): 98%
- **F1-Score:**
    - Healthy loans (0): 100%
    - High-risk loans (1): 92%
- **AUC (Area Under the Curve):**
    - Training AUC: 99%
    - Test AUC: 99.6%

#### **Summary of Results:**
- **Logistic Regression** has a very high accuracy (99%) and is good at predicting healthy loans (0). It performs well in predicting high-risk loans (1), with a recall of 98%, meaning it correctly identifies most high-risk loans. However, its precision for high-risk loans is a bit lower (87%).
- Other models like **XGBoost** and **LightGBM** were not tested here, but **Logistic Regression** already gives good results.

## Summary

- **Best Performing Model:** **Logistic Regression** is the best model in this case. While it doesn't have perfect precision for high-risk loans, its high recall (98%) is very important because we don’t want to miss high-risk loans, even if it means misclassifying a few healthy loans.
- Logistic Regression works well because it's simple and effective for binary classification tasks like this. It is also less likely to overfit the data due to regularization.
- Based on the results, **Logistic Regression** is the recommended model. It strikes a good balance between performance and ease of understanding, making it a reliable option for real-world use, especially when trying to avoid missing high-risk loans.
