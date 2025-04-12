# Loan Default Prediction

## Project Overview

You work for a **Fintech** company specializing in lending various types of loans to urban customers. When a loan application is received, the company must decide whether to approve the loan based on the applicant’s profile. This decision involves a trade-off:

- **Risk of Business Loss**: Not approving a loan for a trustworthy customer results in lost revenue.
- **Risk of Financial Loss**: Approving a loan for a high-risk customer who defaults can lead to monetary loss.

The goal of this project is to **build a predictive model** using historical loan applicant data to estimate the likelihood of loan default. This will help inform decisions such as:
- Denying risky applications
- Adjusting the loan amount
- Applying a higher interest rate for high-risk applicants

---

## Problem Statement

The dataset provided includes information about past applicants and whether they defaulted. By identifying patterns in this data, we aim to predict the probability of default for new applicants.

### Loan Decision Outcomes:
- **Loan Accepted**:
  - **Fully Paid**: Loan has been fully repaid.
  - **Current**: Loan is still being repaid.
  - **Charged-off**: Loan has defaulted (our target label).
- **Loan Rejected**: No transactional history is available for these applicants.

---
## Objective

Build a machine learning model that can reliably **predict the risk of loan default** and assist the company in **making smarter lending decisions**.

---

## Dataset Information

### Sources:
- **Training Data**: [train.csv](train.csv)
- **Test Data**: [test.csv](test.csv)

### Target Variable:
- `loan_status`: We will treat `Charged-off` as a positive label (i.e., **defaulted**) and the rest as negative.

---

## Data Dictionary

| Column Name             | Description |
|-------------------------|-------------|
| `loan_amnt`             | Requested loan amount |
| `term`                  | Loan term (36 or 60 months) |
| `int_rate`              | Interest rate |
| `installment`           | Monthly installment amount |
| `grade`                 | Assigned loan grade |
| `sub_grade`             | Assigned sub-grade |
| `emp_title`             | Job title |
| `emp_length`            | Employment length in years (0–10+) |
| `home_ownership`        | Home ownership status (RENT, OWN, MORTGAGE, OTHER) |
| `annual_inc`            | Annual income |
| `verification_status`   | Income verification status |
| `issue_d`               | Loan issue date |
| `loan_status`           | Current status of the loan (target variable) |
| `purpose`               | Loan purpose category |
| `title`                 | Loan title |
| `zip_code`              | Zip code (first 3 digits) |
| `addr_state`            | State |
| `dti`                   | Debt-to-Income ratio |
| `earliest_cr_line`      | Date of earliest credit line |
| `open_acc`              | Number of open credit lines |
| `pub_rec`               | Number of derogatory public records |
| `revol_bal`             | Revolving credit balance |
| `revol_util`            | Revolving line utilization rate |
| `total_acc`             | Total number of credit lines |
| `initial_list_status`   | Initial listing status (W, F) |
| `application_type`      | Individual or joint application |
| `mort_acc`              | Number of mortgage accounts |
| `pub_rec_bankruptcies`  | Number of public record bankruptcies |

---

## Project Workflow

1. **Data Exploration (EDA)**:
   - Analyze class distribution
   - Visualize key trends and correlations

2. **Preprocessing**:
   - Handle missing values
   - Encode categorical variables
   - Feature scaling and transformation

3. **Model Building**:
   - Train multiple classification models (e.g., Logistic Regression, Random Forest, XGBoost)
   - Evaluate using metrics like Accuracy, Precision, Recall, F1 Score, and ROC-AUC

4. **Model Evaluation**:
   - Confusion Matrix
   - Feature Importance
   - Cross-validation

5. **Prediction**:
   - Generate predictions on the test dataset

---

## Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- SMOTE
- Logistic Regression,Decision Tree,Random Forest

---
## Directory Organization

- Code-loan_default_prediction.pdf - Code
- Slides - Slides-Loan_Default_Prediction.pdf
- Train Dataset - train.csv
- Test Dataset - test.csv

---


## License

This project is for educational and internal research use only.

