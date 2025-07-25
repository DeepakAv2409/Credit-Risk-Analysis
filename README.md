# Credit-Risk-Analysis
# 🧾 Credit Risk Analysis

A machine learning project aimed at identifying high-risk credit card users (Revolvers) and classifying them from low-risk users (Transactors) using behavioral, demographic, and financial features. Built using real-world customer data from a banking context, the project leverages advanced modeling and explainable AI techniques to guide credit decisions and minimize financial exposure.

---

## 📊 Dataset Overview

- 8,448 customer profiles with 28 features
- Includes demographics, card activity (30/60/90 days), income, credit limit, and customer vintage
- Target variable: `Transactor` vs. `Revolver` classification

---

## 🔍 Key Insights from EDA

- Most customers fall into the middle-income bracket (₹6L–₹20L)
- Recent card activity and spend-to-limit ratio are strong indicators of risk
- Income, credit limit, and card tenure heavily influence repayment behavior
- Revolvers show higher utilization and risk despite lower income levels

---

## ⚙️ Feature Engineering

- **Engagement Score** (activity over time)
- **Spend-to-Limit Ratio** (credit utilization)
- **Income Bracket Tagging**
- **Card Tenure Calculation**
- Label encoding for categorical variables
- Standardization of numerical financial features

---

## 🤖 Models Implemented

| Model                  | Accuracy | F1 Score | AUC Score | Best For                            |
|------------------------|----------|----------|-----------|-------------------------------------|
| Logistic Regression    | 81%      | 0.88 (R) | ~0.80     | Baseline performance                |
| Random Forest          | 91%      | 0.92     | ~0.95     | Balanced and interpretable model    |
| XGBoost                | 98%      | 0.96     | ~1.00     | Industry-grade classification       |
| LightGBM               | Similar to XGBoost | — | — | Comparable in accuracy and speed    |

---

## 📈 Model Explainability (SHAP)

- Top predictors: `avg_spends_l3m`, `annual_income`, `high_networth`, `spend_to_limit_ratio`
- SHAP values used to visualize individual and global feature contributions
- Identified high-risk Revolvers with mismatched income and credit limits for targeted interventions

---

## 💡 Business Outcomes

- Enabled **early detection** of credit risk for Revolvers
- Supported **risk-based credit limit assignment**
- Flagged overleveraged profiles for manual review
- Offered clear **recommendations for portfolio optimization**

---

## 🧠 Tools & Tech

`Python`, `Pandas`, `Scikit-learn`, `XGBoost`, `LightGBM`, `SHAP`, `Matplotlib`, `Seaborn`

---

## 📄 Full Report

[📥 Download the Credit Risk Analysis Report (PDF)](./Credit%20Risk%20Analysis.pdf)

---

## 👨‍💻 Author

**Deepak Arumugam Vivekanandan**  
📧 deep199907@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/deepakv1e7d6/)
