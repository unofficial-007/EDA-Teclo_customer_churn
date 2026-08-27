# Telco Customer Churn - Exploratory Data Analysis

## Overview

This project performs Exploratory Data Analysis (EDA) on the IBM Telco Customer Churn dataset.

The purpose of this analysis is to investigate customer characteristics, service usage, billing information, and factors associated with customer churn.

## Dataset

The dataset contains 7,043 customer records and 21 original variables.

The dataset includes:

- Customer demographic information
- Account information
- Services subscribed to
- Billing information
- Customer churn status

## Objectives

The main objectives of this EDA are:

1. Understand the structure of the dataset
2. Assess data quality
3. Identify missing values and duplicate records
4. Analyze numerical variable distributions
5. Analyze categorical variables
6. Investigate relationships between features and churn
7. Identify important patterns associated with customer churn

## Data Preprocessing

The following preprocessing steps were performed:

- Converted `SeniorCitizen` from numerical values to categorical labels
- Converted `TotalCharges` to a numerical data type
- Created a `tenure_group` feature
- Removed the `customerID` identifier
- Separated numerical and categorical variables

## Exploratory Data Analysis

The analysis includes:

### Univariate Analysis

- Histograms
- Kernel density estimates
- Categorical count plots
- Distribution analysis

### Bivariate Analysis

- Numerical variables vs Churn
- Box plots
- Categorical variables vs Churn
- Churn rate comparisons

### Correlation Analysis

A correlation heatmap was used to examine relationships between numerical variables and identify potential multicollinearity.

## Key Findings

The analysis identified several factors associated with customer churn:

- Customer tenure
- Monthly charges
- Contract type
- Internet service
- Payment method

Month-to-month customers showed higher churn compared with customers on longer-term contracts.

The Churn target variable is also imbalanced, which should be considered during machine learning model development.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

```text
telco-customer-churn-eda/
│
├── README.md
├── EDA_Report.pdf
├── EDA_Telco_Customer_Churn.ipynb
├── requirements.txt
│
├── data/
│   └── Telco-Customer-Churn.csv
│
└── eda_charts/
