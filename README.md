# 🏦 Bank Customer Churn Analysis

## 📘 Project Overview

This project analyzes a customer churn dataset provided by Maven Analytics, containing 9,997 rows of historical customer data from a fictional bank. The primary objective is to **identify key patterns behind customer churn (Exited = 1)** and offer **actionable recommendations** to improve retention and customer experience across departments.

---

## 📊 Dataset Summary

- **Total rows**: 9,997   
- **Target metric**: `Exited` (1 = churned, 0 = retained)
- **Key segmentation variables**:
  - `Geography` (Country)
  - `CreditScore`
  - `Balance`
  - `Tenure` (months)
  - `NumberOfProducts`
  - `IsActiveMember`
  - `EstimatedSalary`
  - `Age`

---

## 📌 Analytical Approach

- Exploratory Data Analysis in Power BI
- Segmentation by geography, credit score group, balance group, product usage, and age groups
- Churn percentage and volume analysis
- Cross-dimensional comparisons (e.g., Germany vs France/Spain)
- Business-focused insights and team-specific recommendations

---

## 📈 Key Findings

### 📍 Overall Churn
- **20.38%** of customers have churned (2,037 out of 9,997).
- **Germany** shows the highest churn rate at **32.46%**, with more **non-active users than active** ones.
- **France and Spain** are more stable with **churn rates at 16%**.

### 🌍 Geography-Based Insights
- Germany's churn is consistent across credit score and product groups, with no stabilizing segment except **2-product users (12% churn)**.
- France and Spain follow the same pattern: churn is lowest for 2-product customers, but  4-product customers show **100% churn**.

### 💰 Balance-Based Insights
- **High Balance** group has the **most churned customers overall (1,192)**.
- **Very High Balance**  only have **19 churned customers** overall due to small group size.
- **Germany** has **no customers in the Very High or Zero balance groups** that churned — only Medium and High.
  - Among Germans:
    - **High Balance**: **36%** churn
    - **Medium Balance**: **21%** churn
- In **France and Spain**, **Very High Balance customers** have the **highest churn rates**, unlike Germany.

### 📉 Credit Score Insights
- **Low credit score group** has the highest churn rate at **23%**, but small size.
- **Medium credit score group (500–650)** has the **most churned customers** — making it the highest-impact segment.
- Credit score alone does not explain churn in Germany, where rates are high across all bands.

### ⏳ Tenure Insights
- **No strong churn pattern based on tenure**.
  - Churn counts are fairly even across 1–9 months.
  - **1-month tenure** has the most churn (232), but differences are minor.
  - **Lowest churn** is at 0-month (95) and 10-month (101) tenure groups.

### 👥 Product Usage Patterns
- In all three countries, customers with **2 products** have the **lowest churn rate**:
  - **Germany**: 2-product customers churn at just **12%**
  - Other product counts show steep churn:
    - **1 product**: 43%
    - **3 products**: 90%
    - **4 products**: **100%**
- **France and Spain** follow the same trend:
  - Lowest churn at 2 products, highest at 3, then followed by 4 products (100%).

### 🧓 Age Group Insight
- The **age group 41–50** has the **highest number of churned customers (788)** across all three countries.
- This pattern is consistent in **Germany, France, and Spain**.

---

## 🧠 Business Insight

Churn is **not driven by tenure**, but rather by **customer profile and behavior**:
- Geography (especially Germany)
- Balance group (High and Very High)
- Medium credit scores
- Product usage (1 or more than 2)
- Age group 41–50

---

## 🎯 Recommendations by Team

### 👨‍💼 Customer Retention
- Deploy churn-risk alerts for **medium credit score + high balance customers**, especially in Germany.
- Launch targeted campaigns for **3–4 product users**, simplifying their product experience.

### 📈 Marketing
- Localize engagement strategies for **German customers** with tailored messaging.
- Promote cross-sell strategies nudging 1-product users toward 2-product bundles.

### 🧑‍💻 Product
- Redesign product bundles with a focus on **2-product combinations**, which show lowest churn.
- Audit churn journeys for **3–4 product users** to identify friction or mismatch.

### 📊 Data & Analytics
- Build a churn prediction model using: geography, balance, product usage, credit score, and activity.

### 🌍 Country/Regional Teams
- Investigate churn causes in Germany through surveys or interviews.
- Customize support and onboarding flows for German users in High/Medium balance groups.

### 💼 Strategy & Finance
- Quantify **financial loss from churn in high-value segments**.
- Align LTV and churn-risk models to decide retention budget priorities.

---

## 🔚 Final Summary

> “This churn analysis shows that customer loss is **not random** — it follows distinct patterns by geography, product behavior, and value segment.  
> High churn is concentrated in Germany, among medium-credit and high-balance users, and among customers with 1 or more than 2 products.  
> By targeting these segments across departments, the business can **retain high-value customers**, reduce financial loss, and improve customer experience.”

---

## 📂 Tools Used

- Power BI (Data Modeling & Dashboard)
- Excel (initial review)
- DAX for churn calculation
- SQL (if applicable for preprocessing)

---

## 📌 Dataset Source

This dataset was provided by **[Maven Analytics](https://www.mavenanalytics.io/data-playground)** as part of a public data challenge.

---

## 📧 Contact

Built by **Daniel Siregar**  
Aspiring Data Analyst | SQL | Power BI | Python  
Connect on [LinkedIn](#)  
