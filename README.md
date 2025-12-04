# CHURN_ANALYSIS
# Customer Churn Prediction & Financial Impact Analysis
**End-to-End Analytics Project | Machine Learning + Power BI Financial Dashboard**
**Overview**

This project develops a complete analytics pipeline to identify customers at risk of churning, predict churn probability using a machine learning model, and quantify the financial impact of churn using CLV (Customer Lifetime Value)–based revenue loss and retention ROI simulations.
A full Power BI dashboard is created to translate the insights into actionable business decisions.

**Data Overview**

**Customer Information**

- customerID – Unique customer identifier
- gender – Male/Female
- SeniorCitizen – 0 = Not senior, 1 = Senior citizen
- Partner – Whether the customer has a partner (Yes/No)
- Dependents – Whether the customer has dependents (Yes/No)

**Account Tenure**

- tenure – Number of months the customer has stayed
**Phone & Internet Services**

- PhoneService – Whether the customer has a phone service (Yes/No)
- MultipleLines – Multiple phone lines status (Yes/No/No phone service)
- InternetService – DSL / Fiber optic / No internet
- OnlineSecurity – Online security add-on (Yes/No)
- OnlineBackup – Online backup add-on
- DeviceProtection – Device protection add-on
- TechSupport – Tech support add-on
- StreamingTV – Streaming TV add-on
- StreamingMovies – Streaming Movies add-on

**Contract & Billing**

- Contract – Type of contract (Month-to-month / One year / Two year)
- PaperlessBilling – Whether billing is paperless (Yes/No)
- PaymentMethod – e.g., Electronic check, Mailed check, Bank transfer, Credit card

**Charges**

- MonthlyCharges – Current monthly bill
- TotalCharges – Total amount paid till date


**1.  Data Preprocessing**

Handling missing values
Encoding categorical variables
Feature scaling
Creating new features:
ContractMonths (1, 12, or 24)
CLV = Monthly Charges × Contract Months
Tenure Bands
Splitting train/test sets

**2. Exploratory Data Analysis (EDA)**
- Churn vs Non-Churn Customers
- Monthly Charges distribution
- Churn rate by Tenure group
- Churn rate by contact type
- Churn rate by Payment method
- Churn rate by internet service type
- Monthly charges vs Churn
- Correlation Heatmap
- Average monthly revenue: Churned vs Non churned

**Modelling**
Compare 3 models
- Logistic regression
- Random forest
- Xgboost

Went ahead with Logistic regression as it performed thebest in predicting the Churn

**4. Financial Impact Analysis**

Key components included:
A. Revenue Lost
Target Variable
CLV Lost
ROI Simulation for Retention Strategy

**5. Power BI Dashboard**

A complete interactive dashboard was built containing:

**KPIs**

- Total Customers
- Churned Customers
- Churn Rate
- High-Risk Customers
- Revenue Lost
- CLV Lost

**Visuals**

- Churn by Tenure Band

- Churn by Contract Type

- High-Risk High-Value Customer Table

- Churn Probability Histogram

- Revenue Loss by Customer Segment (Donut)


**Key Insights for Retention**
Targeting customers with high churn probability (≥ 0.6) The strategy focuses on customers who are likely to churn soon, making them the most important group for intervention.

Selecting financially valuable customers (top 40% CLV) By choosing customers with above-average Customer Lifetime Value, the company ensures retention efforts focus on customers who generate significant revenue.

Including customers with moderate Monthly Charges (top 60%) This avoids spending resources on very low-paying customers who wouldn't justify the retention cost.

Allowing moderate tenure (≥ 3 months) This expands the target group beyond long-tenure customers, increasing retention potential without lowering quality.

Offering a very low-cost retention incentive (Rs. 100 discount) The strategy keeps intervention expenses minimal, increasing the chances of achieving a positive ROI.

Assuming a realistic but effective success rate (60%) With more than half of targeted customers retained, the revenue saved becomes significantly higher than the retention cost.

Revenue saved from retained high-CLV customers outweighs cost Because high-value customers are retained at a good success rate, the total saved revenue exceeds the total discount cost—leading to a positive Net ROI.

 ## Dashboard Preview

Below is the Power BI dashboard created for this project:

![Churn Analysis Dashboard](https://github.com/SaurabhKumar-Singh/CHURN_ANALYSIS/blob/main/CHURN_ANAlYSIS/Dashboard_Picture.JPG?raw=true)
