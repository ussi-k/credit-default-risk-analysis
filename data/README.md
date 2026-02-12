# Credit Card Default Risk Analysis – Exploratory Data Analysis (EDA)

**Author:** Usaid Khan

---

## 📌 Project Overview

This project presents a comprehensive Exploratory Data Analysis (EDA) of a credit card default dataset to identify the key financial and behavioral drivers of default risk.

The objective is to analyze customer repayment patterns, credit utilization behavior, and demographic characteristics to understand what factors most strongly influence the probability of default in the following month.

This project follows an industry-aligned risk analytics approach, focusing on structured analysis, behavioral feature engineering, and business interpretation rather than predictive modeling.

---

## 📂 Dataset Information

- **Dataset Name:** Default of Credit Card Clients Dataset
- **Source:** UCI Machine Learning Repository
- **Original Study:** Yeh, I. C., & Lien, C. H. (2009)
- **Dataset Link:** https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients
- **Total Records:** 30,000 customers
- **Target Variable:** `default_next_month`

### Key Variables

- Credit limit (`LIMIT_BAL`)
- Billing amounts for the last 6 months (`BILL_AMT1 – BILL_AMT6`)
- Payment amounts for the last 6 months (`PAY_AMT1 – PAY_AMT6`)
- Repayment status history (`PAY_0 – PAY_6`)
- Demographic features (Age, Gender, Education, Marital Status)

---

## 🔎 Analytical Approach

The analysis was structured in a step-by-step risk evaluation framework:

### 1️⃣ Data Cleaning & Preparation

- Verified data types and structure
- Checked for missing values
- Handled edge cases (e.g., zero average bill amounts)
- Validated target distribution

### 2️⃣ Univariate Analysis

- Distribution of default vs non-default
- Credit limit distribution
- Age distribution
- Demographic breakdown

### 3️⃣ Bivariate Analysis

- Education vs Default Rate
- Marital Status vs Default Rate
- Credit Limit vs Default
- Repayment Status vs Default
- Payment Behavior vs Default

### 4️⃣ Multivariate Analysis

- Correlation analysis with default
- Heatmap visualization
- Multicollinearity assessment
- Comparative behavioral trend analysis

---

## ⚙️ Feature Engineering

To enhance behavioral risk interpretation, domain-driven features were engineered:

### • Utilization Ratio

Average billing amount divided by credit limit.
Measures how intensively a customer uses their available credit.

### • Average Payment

Mean of payment amounts across six months.
Captures overall repayment volume.

### • Average Bill

Mean of billing amounts across six months.
Represents typical financial exposure.

### • Average Payment Ratio

Average Payment divided by Average Bill.
Evaluates repayment discipline relative to outstanding balance.

### • Average Delinquency Score

Mean of repayment status variables (`PAY_0 – PAY_6`).
Quantifies overall payment delay behavior.

These engineered features provide consolidated behavioral indicators commonly used in credit risk analysis.

---

## 📊 Key Findings

- Repayment history variables (`PAY_0 – PAY_6`) show the strongest relationship with default probability.
- Customers with repeated or recent payment delays exhibit significantly higher default risk.
- High credit utilization combined with low payment ratio strongly correlates with elevated default probability.
- Behavioral metrics outperform demographic features in explaining default risk.
- Demographic attributes such as gender and marital status show comparatively weak influence.

---

## 💼 Business Implications

- Repayment discipline should be prioritized in credit risk monitoring systems.
- Customers with rising delinquency trends should be flagged for early intervention.
- Utilization-based segmentation can improve risk-based credit policy decisions.
- Behavioral features provide stronger predictive insight than demographic segmentation.

---

## 🛠 Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

---

## 🚀 How to Run the Project

1. Clone this repository
2. Navigate to the `notebooks/` folder
3. Open `01_credit_card_default_eda.ipynb`
4. Run all cells sequentially

---

## 🎯 Project Highlights

- Structured EDA framework aligned with industry practice
- Domain-driven feature engineering
- Behavioral risk interpretation
- Business-focused insights
- Clean project organization

---

## 🏁 Conclusion

This project demonstrates how structured exploratory analysis and behavioral feature engineering can uncover critical drivers of credit default risk.

The findings align with industry-level credit risk assessment practices, emphasizing repayment behavior, credit utilization, and delinquency trends as primary determinants of default probability.

This analysis provides a strong foundation for future predictive modeling and risk scoring systems.

---
