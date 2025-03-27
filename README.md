# Credit Risk Classification

This project leverages machine learning techniques to analyze historical lending data and evaluate loan risk. Using a logistic regression model, we aim to predict borrowers' creditworthiness to assist peer-to-peer lending services in decision-making.

---

## Solution:
  - [`credit_risk_classification.ipynb`](https://github.com/Saurabh-Lakhanpal/credit-risk-classification/blob/main/credit_risk_classification.ipynb)
  - [`Overview of the Analysis`](#overview-of-the-analysis)
  - [`lending_data.csv`](https://github.com/Saurabh-Lakhanpal/credit-risk-classification/blob/main/Resources/lending_data.csv)

---

## Instructions

### Step 1: Split the Data into Training and Testing Sets
1. Load the `lending_data.csv` file into a Pandas DataFrame.
2. Create:
   - Labels set (`y`) from the `loan_status` column:
     - **0** = Healthy loan
     - **1** = High-risk loan
   - Features DataFrame (`X`) using the remaining columns.
3. Split the data into training and testing datasets using `train_test_split`.

### Step 2: Create a Logistic Regression Model
1. Train the logistic regression model using the training data (`X_train` and `y_train`).
2. Save predictions for the testing data labels using the testing feature data (`X_test`) and the trained model.

### Step 3: Evaluate Model Performance
1. Generate a confusion matrix.
2. Print the classification report.
3. Assess the model's performance in predicting:
   - **0 (healthy loan)**
   - **1 (high-risk loan)**

Answer this question: 
- How well does the logistic regression model predict each loan status label?

### Step 4: Write a Credit Risk Analysis Report
1. Provide an overview of the analysis in the **README.md** file.
2. Report model performance:
   - Accuracy score
   - Precision score
   - Recall score
3. Summarize the results and justify whether this model is recommended for identifying loan risks. If not, provide reasoning.

---

## Overview of the Analysis

The purpose of this analysis was to use machine learning to predict credit risk based on borrowers' financial data. The dataset included information such as:
- Loan size
- Interest rate
- Borrower income
- Debt-to-income ratio
- Number of credit accounts
- Derogatory credit marks
- Total outstanding debt

The target variable, `loan_status`, classified loans as either:
- **0** = Healthy loan
- **1** = High-risk loan.

Despite an imbalanced dataset (approximately 97% healthy loans and 3% high-risk loans), we successfully developed a logistic regression model to predict loan risk.

Key stages of the machine learning process included:
1. Preprocessing and feature selection.
2. Splitting data into training and testing sets.
3. Training and testing a logistic regression model.
4. Evaluating model performance through accuracy, precision, recall, and F1 scores.

---

## Results

Using a logistic regression model, we achieved the following performance metrics:

- **Accuracy Score:** 0.99 (99% of predictions were correct overall).
- **Precision:** 
  - **Healthy loan (`0`)**: 1.00 (no false positives for healthy loans).
  - **High-risk loan (`1`)**: 0.84 (some false positives for high-risk loans).
- **Recall:**
  - **Healthy loan (`0`)**: 0.99 (almost all healthy loans were correctly identified).
  - **High-risk loan (`1`)**: 0.94 (most high-risk loans were correctly identified).
- **F1 Score:**
  - **Healthy loan (`0`)**: 1.00
  - **High-risk loan (`1`)**: 0.89

---

## Summary

The logistic regression model performed exceptionally well in identifying healthy loans and reasonably well in detecting high-risk loans. It is recommended for credit risk prediction due to:
- High performance in accuracy and precision.
- Simplicity and interpretability.

However, if accurately identifying high-risk loans is critical, additional techniques (e.g., using SMOTE to handle class imbalance or exploring more complex models like Random Forest or XGBoost) could be considered for further improvements.

---

## Resources
- [scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Python Official Documentation](https://www.python.org/doc/)
- [Seaborn for Data Visualization](https://seaborn.pydata.org/)  
