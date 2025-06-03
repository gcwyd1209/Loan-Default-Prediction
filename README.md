# Loan-Default-Prediction

## Introduction

Credit risk management is essential for the sustainability and profitability of banking institutions. In response to rising consumer loan delinquencies post-COVID-19, this project addresses the limitations of traditional credit scoring systems by leveraging machine learning techniques. Group 1 Data Science Consultants partnered with Evergreen National Bank to build an advanced predictive model for loan default using the Berka Dataset—an anonymized financial dataset containing account, transaction, loan, and demographic data.

## Objectives

Identify behavioral, demographic, and financial factors contributing to loan default.
Develop machine learning models to predict borrower risk.
Recommend strategies to improve risk assessment, operational efficiency, and fairness.

## Dataset: The Berka Dataset

Sourced from the PKDD'99 Discovery Challenge, the dataset contains:
1. account.asc: Account information
2. client.asc: Client demographics
3. loan.asc: Loan records
4. trans.asc: Transactions
5. card.asc, disp.asc, order.asc, district.asc: Supplementary data

## Data Integration

Key integration steps:
Merged loans with account and client data
Aggregated transactions to create behavioral features (e.g., balance trends, overdraft frequency)
Incorporated demographic data (e.g., salary, unemployment rate by district)
Created binary features for credit card ownership and permanent orders
Imputed missing values and standardized formats for modeling

## Feature Engineering

Created balance statistics (mean, max, min) over recent months
ncoded categorical variables (e.g., transaction type)
Derived frequency of overdrafts and monthly payment patterns

## Methodology

### Models Developed

1. Generalized Linear Model (GLM)
2. GLM with ROSE (for balancing class distribution)
3. Naïve Bayes with ROSE
4. Random Forest with ROSE
5. Gradient Boosting Machine (GBM)

### Evaluation Metrics
1. Accuracy
2. AUC (Area Under the ROC Curve)
3. Confusion Matrix


### Key Findings

Top-performing model: GBM

Most predictive features:
balance_min_last_month
loan_duration
loan_payments
monthly_payment_trans_count
account_balance_trends

## Conclusion

By using machine learning to assess loan default risk, Evergreen National Bank can improve prediction accuracy, enhance operational efficiency, and adopt ethical, data-driven lending practices. The Berka Dataset offers a strong foundation for building scalable credit risk models that combine behavioral, demographic, and financial insights.


## Authors

Group 1 Data Science Consultants
