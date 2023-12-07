# Fintech-Loan-Default-Prediction-Machine-Learning-Model

# Loan Default Prediction on Imbalanced Dataset Using Classification Machine Learning Model

## Table of Contents
1. [Problem](#problem)
2. [Aim](#aim)
3. [Exploratory Data Analysis](#exploratory-data-analysis)
4. [Data Pre-processing](#data-pre-processing)
5. [Feature Engineering](#feature-engineering)
6. [Feature Analysis](#feature-analysis)
7. [Machine Learning Model Part](#machine-learning-model-part)
8. [Conclusion](#conclusion)

## Problem
Exploratory data analysis reveals a significant issue: the payback rate for approved loans is just 31.1%, indicating a high risk of default.

## Aim
The primary goals of this project are:
- To reduce the financial losses incurred by Fintech company due to high-risk loan approvals.
- To build an efficient classification machine learning model that can predict loan defaults in approved loans.

## Exploratory Data Analysis
- Joining loan and payment data.
- Merging datasets and exploring the combined data.
- Focusing on approved and fully funded loans.
- Analyzing missing values.

## Data Pre-processing
- Removing features with over 80% missing values.
- Feature classification into numerical, categorical, and other types.
- Imputing missing values in each feature set.

## Feature Engineering
- Developing a new feature: "days_to_process".
- Defining the target variable.
- Standardizing numerical columns using RobustScaler.
- One-hot encoding of categorical features.

## Feature Analysis
- Standardizing numerical columns.
- Preparing the dataset for training.

## Machine Learning Model Part
### Performance Metrics
- Recall
- Precision
- F1-Score

### Model Analysis
- Random Forest model performance with and without 'loanAmount'.
- Analysis of the model's precision, recall, and F1-score.
- Impact of 'loanAmount' on Type-II errors (false negatives).

## Conclusion
The Random Forest model demonstrates high precision and good recall rates. It effectively identifies defaulted loans, which is crucial for minimizing financial losses in Fintech Company's loan approval process. The analysis shows that dropping 'loanAmount' increases the number of false negatives, suggesting its importance in the model. Thus, it is recommended to retain 'loanAmount' in the model to reduce Type-II errors.
