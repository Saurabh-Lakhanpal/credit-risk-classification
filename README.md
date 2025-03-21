# Credit Risk Classification

This project leverages machine learning techniques to analyze historical lending data and evaluate loan risk. Using a logistic regression model, we aim to predict borrowers' creditworthiness to assist peer-to-peer lending services in decision-making.

---

## Solution:
  - [`credit_risk_classification.ipynb`]()
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

## Results

### Model Evaluation Metrics:
- **Accuracy Score**: Add your score here.
- **Precision Score**: Add your score here.
- **Recall Score**: Add your score here.

### Summary:
Summarize key takeaways from the analysis, including:
- Strengths of the model.
- Any limitations.
- Recommendation (or not) for the company to adopt the model.

---

## Resources
- [scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Python Official Documentation](https://www.python.org/doc/)
- [Seaborn for Data Visualization](https://seaborn.pydata.org/)

