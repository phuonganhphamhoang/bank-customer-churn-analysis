# 🏦 Bank Customer Churn Analysis

This project focuses on analyzing and predicting customer churn in the banking sector using a dataset of 10,000 clients. By leveraging Python and machine learning models, the goal is to identify patterns and key drivers of churn and recommend actionable strategies for customer retention.

---

## 🎯 Objectives

- Understand customer profiles based on demographics and behavior.
- Identify key factors contributing to churn.
- Build a predictive model to classify churned vs. retained customers.
- Provide strategic recommendations to reduce churn rate.

---

## 📊 Dataset Overview

- **Source:** [Kaggle - Bank Customer Churn](https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn?fbclid=IwAR2EiBzhQphi0kE4NuPVzRx68HGTsAcvNeq_sncH1joh7Iq3M6XufXfrmX4)
- **Rows:** 10,000
- **Features:** 18 (including age, geography, balance, credit score, tenure, etc.)
- **Target Variable:** `Exited` (1 if the customer churned, 0 otherwise)

---

## 🛠 Tools & Technologies

- Python (pandas, matplotlib, seaborn, scikit-learn)
- SMOTE (for class imbalance)
- Tableau (for dashboarding)
- Jupyter Notebook
- Git & GitHub

---

## 🧼 Data Preprocessing

- Dropped irrelevant columns (`RowNumber`, `CustomerID`, etc.)
- Label encoding for categorical features (`Gender`, `Geography`, `CardType`)
- Feature normalization for numerical values (e.g., `Balance`, `EstimatedSalary`)
- Handled class imbalance using **SMOTE** to upsample minority class

---

## 📈 Modeling & Evaluation

- **Model used:** Random Forest Classifier
- **Train/Test Split:** 80/20
- **Accuracy:** 91.18%
- **Precision/Recall (Exited):** 91% / 91%
- **ROC-AUC Score:** 0.9686

---

## 🧠 Feature Importance

Top contributing features to customer churn:
- `Age` (20%)
- `Number of Products`
- `IsActiveMember`
- `Balance`

Less important: `HasCrCard`, `Tenure`, `Satisfaction Score`, `Card Type`

---

## 📊 Dashboard (Tableau)

Interactive churn insights available here:  
🔗 [View Tableau Dashboard](https://public.tableau.com/app/profile/anh.ph.m.ho.ng.ph.ng/viz/PROJECTCHURNANALYSISFINAL/Story1?publish=yes)

---

## 💡 Key Insights

- Customers in **Germany** have the highest churn rate (~32%)
- **Female customers** churn more than males
- Churn is higher in **inactive customers**, customers aged **40+**, and those using **3+ products**
- Complaint handling has a huge impact: nearly **100% of customers who filed a complaint churned**
- High earners and high card tier holders still churned — indicating service issues beyond benefits

---

## ✅ Recommendations

- Improve onboarding and retention for new customers (especially within the first year)
- Redesign benefits structure for higher-tier cards
- Address female customer pain points
- Create loyalty programs tied to complaint resolution and satisfaction scores
- Launch targeted campaigns for high-risk segments (e.g., inactive, older clients in Germany)

---
