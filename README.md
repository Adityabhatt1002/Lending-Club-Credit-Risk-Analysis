# Lending Club Credit Risk Analysis & Default Prediction

## Project Overview

This project analyzes loan data from Lending Club to identify factors that influence loan default and build machine learning models capable of predicting borrower risk.

The objective is to help financial institutions identify potentially risky borrowers before issuing loans.

---

## Business Problem

Loan defaults result in significant financial losses for lending institutions.

The goal of this project is to:

* Analyze borrower behavior
* Identify key default indicators
* Build predictive models for credit risk assessment

---

## Dataset

Source:

https://www.kaggle.com/datasets/jeandedieunyandwi/lending-club-dataset

Dataset Size:

* ~396,000 loan records
* Multiple borrower and loan-related attributes

Target Variable:

* 0 = Fully Paid
* 1 = Charged Off (Default)

---

## Project Workflow

### 1. Data Cleaning

* Missing value handling
* Outlier treatment
* Data type conversion

### 2. Exploratory Data Analysis

Analyzed relationships between:

* Loan Grade
* Sub Grade
* Debt-to-Income Ratio (DTI)
* Revolving Utilization
* Interest Rate
* Loan Term
* Home Ownership
* Loan Purpose

### 3. Feature Engineering

Created additional features:

* Payment-to-Income Ratio
* Loan-to-Income Ratio

### 4. Model Development

Models Trained:

* Logistic Regression
* Random Forest
* Tuned XGBoost

---

## Key Findings

### Strong Predictors of Default

* Loan Grade
* Sub Grade
* Interest Rate
* Debt-to-Income Ratio
* Revolving Credit Utilization
* Loan Term

### Business Insights

* 60-month loans default significantly more than 36-month loans.
* Higher debt burden increases default risk.
* Higher credit utilization is associated with increased financial stress.
* Lower credit grades show dramatically higher default rates.
* Extracting the `zip_code` from the applicant addresses revealed highly specific regional clusters with disproportionately high default rates.

---

## Best Model Performance

### Tuned XGBoost

Accuracy: 81%

Default Class Metrics:

* Precision: 0.51
* Recall: 0.78
* F1 Score: 0.62

The model successfully identifies approximately 78% of defaulting borrowers while maintaining overall accuracy above 80%.

---

## Repository Structure

```text
notebooks/
├── 01_EDA_and_Feature_Engineering.ipynb
└── 02_Model_Training_and_Evaluation.ipynb
```

---

## Future Improvements

* Probability-based risk scoring
* Explainability using SHAP
* Deployment using Streamlit
* Automated retraining pipeline

---

## Contact
Email: [iamadityabhatt1002@gmail.com](mailto:iamadityabhatt1002@gmail.com)
