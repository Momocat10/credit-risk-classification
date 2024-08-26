##Credit Risk Analysis

This analysis aims to predict the creditworthiness of borrowers using a machine learning model. The dataset includes financial information such as:

- Loan size
- Interest rate
- Income
- Debt-to-income ratio
- Number of accounts
- Derogatory marks
- Total debt
- Loan status

The goal is to predict the `loan_status` of a borrower:

- 0: Loan repaid
- 1: High risk of default

## Machine Learning Process

### 1. Data Preparation
- Loaded data from `lending_data.csv`.

### 2. Creating Labels and Features
- `y` (labels) created from the `loan_status` column.
- `X` (features) created from the other columns.

### 3. Splitting Data
- Split data into training and testing sets using `train_test_split`.

### 4. Model Training
- Trained a Logistic Regression model with the training data (`X_train`, `y_train`).

### 5. Making Predictions
- Used the model to predict loan statuses on the test set (`X_test`).

### 6. Evaluating the Model
- Evaluated model performance with a confusion matrix and classification report.

## Results

- **Accuracy**: 99%  
- **Precision for Loan Repaid (0)**: 1.00  
- **Precision for High Risk (1)**: 0.87  
- **Recall for Loan Repaid (0)**: 1.00  
- **Recall for High Risk (1)**: 0.89  

## Summary

The logistic regression model showed high accuracy (99%) and performed very well in predicting loans that were repaid. However, it was less accurate for high-risk loans, with a precision of 87% and a recall of 89%. While these results are strong, further improvements, especially for high-risk predictions, could be beneficial.

## Recommendation

To enhance the model's accuracy, especially for high-risk loans, I recommend balancing the dataset. Slighlty exaggerating the majority or minority class can train the model to predict high-risk loans better. 
