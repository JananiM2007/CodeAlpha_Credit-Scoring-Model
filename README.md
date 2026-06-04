# CodeAlpha_Credit-Scoring-Model
Machine Learning-based Credit Scoring System that predicts customer creditworthiness using Logistic Regression and Random Forest, achieving 79% accuracy through feature engineering and financial risk analysis.
# Credit Scoring & Credit Risk Prediction using Machine Learning

## Project Overview

This project develops a Machine Learning-based Credit Scoring System to evaluate the creditworthiness of loan applicants. By analyzing customer financial and demographic information, the model predicts whether an applicant represents a good or bad credit risk.

The goal is to support data-driven lending decisions, reduce the likelihood of loan defaults, and improve overall risk assessment.

---

## Dataset Information

The dataset contains information related to loan applicants, including:

- Account status
- Credit history
- Loan purpose
- Credit amount
- Savings account status
- Employment duration
- Payment-to-income ratio
- Age
- Housing status
- Number of existing credits
- Guarantor information
- Collateral details

**Target Variable:**
- Good Credit Risk
- Bad Credit Risk

---

## Exploratory Data Analysis (EDA)

Performed exploratory analysis to:

- Understand feature distributions
- Identify class imbalance
- Analyze relationships between variables
- Detect potential outliers and trends

---

## Feature Engineering

To improve predictive performance, additional financial indicators were created:

### Credit Per Month
```python
credit_per_month = credit_amount / month_duration
```

### Credit-Age Ratio
```python
credit_age_ratio = credit_amount / age
```

### Burden Score
```python
burden_score = credit_amount * payment_to_income_ratio
```

These engineered features help capture an applicant's financial burden and repayment capability.

---

## Data Preprocessing

- Label Encoding for ordinal categorical features
- One-Hot Encoding for nominal categorical features
- Feature Scaling using StandardScaler
- Train-Test Split for model evaluation

---

## Machine Learning Models

The following classification algorithms were trained and evaluated:

### Logistic Regression
A baseline linear classification model used for credit risk prediction.

### Random Forest Classifier
An ensemble learning model that combines multiple decision trees to improve prediction accuracy and robustness.

---

## Model Performance

| Model | Accuracy |
|---------|---------|
| Logistic Regression | 77% |
| Random Forest Classifier | 78.5% |

The Random Forest model achieved the best overall performance and was selected as the final model.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## Project Workflow

1. Data Collection
2. Data Cleaning and Preprocessing
3. Exploratory Data Analysis
4. Feature Engineering
5. Model Training
6. Model Evaluation
7. Performance Comparison

---

## Key Outcomes

- Built a Credit Risk Prediction System
- Applied Feature Engineering to financial data
- Compared multiple Machine Learning models
- Evaluated model performance using classification metrics
- Automated creditworthiness assessment

---

## Future Improvements

- Hyperparameter Tuning using GridSearchCV
- Implementation of XGBoost and LightGBM
- Credit Score Generation (300–850 scale)
- Deployment using Streamlit or Flask
- Real-time Credit Risk Assessment Dashboard

---

## Author

Janani M

Machine Learning | Data Science | Python
