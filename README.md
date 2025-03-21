# Credit Risk Classification

This project leverages machine learning techniques to analyze historical lending data and evaluate loan risk. Using a logistic regression model, we aim to predict borrowers' creditworthiness to assist peer-to-peer lending services in decision-making.

---

## Solution:
  - [`credit_risk_classification.ipynb`]()
  - [`Report`]()
  - [`lending_data.csv`]()

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

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

---

## Resources
- [scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Python Official Documentation](https://www.python.org/doc/)
- [Seaborn for Data Visualization](https://seaborn.pydata.org/)

