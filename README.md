# Fraud_Detection_Credit_Card

## Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. Fraudulent transactions constitute a very small percentage of overall transactions, making this a highly imbalanced dataset. By analyzing transaction patterns and building robust models, we aim to detect 100% of fraudulent transactions while minimizing false positives. This project not only helps reduce financial losses but also protects businesses from reputational damage caused by unauthorized card usage.

## Problem Statement
The goal is to develop a machine learning model that identifies fraudulent transactions with high accuracy. The main challenges include:
- Handling a highly imbalanced dataset, where only 0.172% of transactions are fraudulent.
- Developing a model that balances sensitivity (detecting all fraudulent cases) and specificity (reducing false positives).

## Dataset
The dataset consists of 284,807 credit card transactions, with 492 labeled as fraudulent. It includes the following features:
- **V1 to V28**: Principal Component Analysis (PCA)-transformed features, which are anonymized to protect sensitive information.
- **Time**: The elapsed time between each transaction and the first transaction in the dataset.
- **Amount**: The transaction amount in monetary units.
- **Class**: The target variable, where 1 indicates fraud and 0 indicates a legitimate transaction.

### Key Observations:
- The dataset is highly skewed, with less than 1% of transactions being fraudulent.
- The `Time` and `Amount` features are not PCA-transformed, making them crucial for initial exploratory analysis.
- There are no missing values, ensuring a clean dataset for analysis.

## Business Questions
1. How does the transaction amount differ between fraudulent and non-fraudulent transactions?
2. Do fraudulent transactions occur more frequently during specific time frames?

## Methodology

### Data Preprocessing
- Standardized the `Amount` and `Time` features for consistency in scale.
- Applied resampling techniques (Oversampling, SMOTE) to address the class imbalance.

### Exploratory Data Analysis (EDA)
- Analyzed `Amount` and `Time` distributions for both classes (fraudulent and non-fraudulent transactions).
- Visualized patterns in transaction amounts and temporal trends to identify anomalies.

### Machine Learning Models
- Evaluated multiple classification models, including:
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - Gradient

