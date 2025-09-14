# Customer Churn Analysis (Python)

Analysing customer churn to identify key drivers and build a simple predictive model.

---

## Objective
Explain the business question in one or two lines.  
**Example:** Identify which customers are most likely to churn and what factors drive churn so that retention actions can be prioritised.

---

## Dataset
- **Source:** [Telco Customer Churn (Kaggle)](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Shape:** **~7,000 rows**, **21+ columns** (demographics, services, account info, churn)
- **Notes:** Remove any personally identifiable information. Large files are not stored in the repo. A small sample may appear in `data/`.

---

## Method
1. **Data cleaning** — handle missing values, fix data types, tidy categorical fields.  
2. **Exploratory Data Analysis (EDA)** — churn rate by contract type, payment method, tenure, services.  
3. **Feature preparation** — encode categoricals, scale numeric features if needed.  
4. **Baseline model** — Logistic Regression and Random Forest.  
5. **Evaluation** — train/test split, accuracy, precision, recall, F1, ROC-AUC.  
6. **Interpretation** — feature importance and practical retention ideas.

**Notebook:** [01_customer_churn_analysis.ipynb](notebooks/01_customer_churn_analysis.ipynb)

---

## Results and Insights
- **Contract type** (month-to-month) is strongly associated with higher churn.  
- **Payment method** (electronic cheque) shows higher churn risk.  
- **Tenure** is protective. Longer-tenure customers churn less.  
- **Model performance:** **Random Forest ~80% accuracy** with balanced precision/recall.  
- Suggested actions: encourage longer contracts, reduce friction in payment methods, target new users with onboarding and support.

**Example charts:**  
![Churn by contract](visuals/churn_by_contract.png)  
![ROC curve](visuals/roc_curve.png)

---

## Files in this repository
