# Loan-Default-Prediction
Introduction

Credit risk management is essential for the sustainability and profitability of banking institutions. In response to rising consumer loan delinquencies post-COVID-19, this project addresses the limitations of traditional credit scoring systems by leveraging machine learning techniques. Group 1 Data Science Consultants partnered with Evergreen National Bank to build an advanced predictive model for loan default using the Berka Dataset—an anonymized financial dataset containing account, transaction, loan, and demographic data.

Objectives

Identify behavioral, demographic, and financial factors contributing to loan default.

Develop machine learning models to predict borrower risk.

Recommend strategies to improve risk assessment, operational efficiency, and fairness.

Research Questions

Are larger loan amounts and longer durations associated with higher default risk?

How does a client’s account balance influence repayment behavior?

Does frequent overdraft activity predict loan default?

Dataset: The Berka Dataset

Sourced from the PKDD'99 Discovery Challenge, the dataset contains:

account.asc: Account information

client.asc: Client demographics

loan.asc: Loan records

trans.asc: Transactions

card.asc, disp.asc, order.asc, district.asc: Supplementary data

Data Integration

Key integration steps:

Merged loans with account and client data

Aggregated transactions to create behavioral features (e.g., balance trends, overdraft frequency)

Incorporated demographic data (e.g., salary, unemployment rate by district)

Created binary features for credit card ownership and permanent orders

Imputed missing values and standardized formats for modeling

Feature Engineering

Created balance statistics (mean, max, min) over recent months

Encoded categorical variables (e.g., transaction type)

Derived frequency of overdrafts and monthly payment patterns

Methodology

Models Developed

Generalized Linear Model (GLM)

GLM with ROSE (for balancing class distribution)

Naïve Bayes with ROSE

Random Forest with ROSE

Gradient Boosting Machine (GBM)

Evaluation Metrics

Accuracy

AUC (Area Under the ROC Curve)

Confusion Matrix

Key Findings

Top-performing model: GBM

Most predictive features:

balance_min_last_month

loan_duration

loan_payments

monthly_payment_trans_count

account_balance_trends

Recommendations

Adopt Predictive Modeling: Integrate GBM and Random Forest into credit approval processes.

Enhance Feature Engineering: Focus on transaction history and behavioral trends.

Improve Operational Efficiency: Automate workflows to flag high-risk accounts.

Mitigate Bias: Monitor model fairness using explainable AI and periodic retraining.

Conclusion

By using machine learning to assess loan default risk, Evergreen National Bank can improve prediction accuracy, enhance operational efficiency, and adopt ethical, data-driven lending practices. The Berka Dataset offers a strong foundation for building scalable credit risk models that combine behavioral, demographic, and financial insights.

References

A full list of academic references can be found in the final report (Final paper.docx.pdf).

File Structure

├── Final_Loan-Default-Prediction-for-Evergreen.pdf
├── Final paper.docx.pdf
├── data/
│   ├── account.asc
│   ├── client.asc
│   ├── card.asc
│   ├── disp.asc
│   ├── district.asc
│   ├── loan.asc
│   ├── order.asc
│   ├── df.csv
├── data_manipulation.html
├── README.md

Authors

Group 1 Data Science Consultants
