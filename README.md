# Customer Lifetime Value (CLV) Modeling & Analysis

## Project Overview
This project focuses on estimating **Customer Lifetime Value (CLV)** using transactional data, with the goal of supporting data-driven decisions in customer segmentation, retention strategy, and revenue optimization.

Rather than treating CLV as a purely academic exercise, this project is designed from a **business-first perspective**, translating customer behavior into actionable insights that stakeholders can use.

---

## Dataset Overview
This project uses the Online Retail II dataset from the UCI Machine Learning Repository, which contains real transactional data from a UK-based non-store online retail company.
- Time period: December 2009 – December 2011
- Business domain: E-commerce / Retail
- Primary use case: Customer behavior analysis and Customer Lifetime Value (CLV) modeling

The dataset captures individual customer purchase transactions and is commonly used for customer segmentation, retention analysis, and CLV-related studies.

---

## Data Source
- Repository: UCI Machine Learning Repository
- Dataset name: Online Retail II
- Link: https://archive.ics.uci.edu/dataset/502/online+retail+ii
- Creator: Daqing Chen
- License: Creative Commons Attribution 4.0 International (CC BY 4.0)

---

## Business Problem
In many retail and subscription-based businesses, understanding **which customers are truly valuable over time** is more important than short-term revenue.

Key questions addressed in this project:
- How can we estimate long-term customer value using historical transaction data?
- How do purchasing frequency and monetary value affect customer lifetime value?
- How can CLV insights support prioritization in marketing and retention strategies?

---

## Approach
This project follows an end-to-end analytical workflow:

1. **Data Preparation**
   - Cleaning transactional data
   - Handling missing values and outliers
   - Creating customer-level features

2. **Exploratory Data Analysis (EDA)**
   - Purchase frequency patterns
   - Monetary value distribution
   - Customer behavior insights

3. **Feature Engineering**
   - Recency, Frequency, and Monetary (RFM-style) features
   - Aggregation at customer level

4. **CLV Modeling**
   - Probabilistic modeling for customer lifetime value
   - Interpretation of model outputs in a business context

---

## Current Status
🚧 **Work in Progress**

The core analysis and modeling pipeline is implemented.  
Further refinements and extensions (e.g. validation, sensitivity analysis, and business scenario simulation) are currently in progress.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Lifetimes (BG/NBD, Gamma-Gamma models)

---

## Key Takeaways (Preliminary)
- CLV provides a more stable metric than short-term revenue for strategic decisions
- Customer purchasing behavior varies significantly and should not be treated uniformly
- Probabilistic models help bridge uncertainty in long-term customer value estimation

---

## Next Steps
- Model validation and performance evaluation
- CLV-based customer segmentation
- Business scenario analysis (e.g. retention uplift simulation)

---

## Author
Ilham Den Fatah  
Aspiring Data Scientist with a background in business & operations leadership