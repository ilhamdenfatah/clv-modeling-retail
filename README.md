# Customer Lifetime Value (CLV) Modeling & Analysis

## Executive Summary

### **Problem Framing**

Many companies know who their high-value customers were, but struggle to answer a more critical question:

`Who should we prioritize going forward, and what should we actually do for each customer?`

Traditional CLV approaches tend to be:
- backward-looking,
- static,
- and disconnected from churn risk.

As a result, retention budgets are often misallocated — over-investing in low-risk customers while missing high-value customers who are quietly drifting away.

### **Business Objective**

The goal of this project is to build a decision-oriented CLV system that:
1. Estimates customers’ future economic value,
2. Quantifies their risk of becoming inactive, and
3. Translates both into clear, differentiated business actions.

The objective is not prediction accuracy for its own sake, but better prioritization and smarter decisions.

### **Approach**

The solution is built in three layers:

##### 1. Probabilistic CLV Baseline

A probabilistic model captures repeat-purchase behavior to estimate:
- likelihood a customer is still active,
- expected number of future transactions,
- expected value per transaction.

This provides a stable, interpretable CLV foundation grounded in customer behavior.

##### 2. Risk-Aware Segmentation

CLV is combined with probability of being alive to separate customers who may look similar in value but differ meaningfully in risk:
- high-value / low-risk,
- high-value / high-risk,
- low-value customers where investment should be limited.

This prevents treating all “high CLV” customers the same.

##### 3. ML-Based CLV Uplift (Strategic Layer)

A machine learning model is layered on top — not to replace probabilistic CLV, but to:
- refine customer ranking,
- capture non-linear behavioral signals,
- and improve revenue concentration in the top segments.

### **Key Insights**

- Customer value and churn risk are not the same thing. A VIP customer can be either stable or close to churn — and the required action is very different.
- A small fraction of customers accounts for a disproportionate share of future revenue, but not all of them deserve equal investment.
- The ML-enhanced ranking consistently surfaces customers with higher realized revenue in the top deciles compared to probabilistic CLV alone.

### **Actionable Decision**

Instead of a single CLV score, the output is a strategy-ready segmentation, for example:
- VIP / High Risk → immediate win-back with personalized incentives.
- VIP / Low Risk → protect and delight with exclusive benefits.
- High CLV / Low Risk → upsell and cross-sell opportunities.
- Low CLV / High Risk → minimize spend or automate engagement.
- Each customer receives not just a score, but a recommended action.

### **Why This Is Better Than Naive CLV**

This approach is stronger because it:
- connects CLV directly to risk and action, not just ranking,
- combines the stability and interpretability of probabilistic models with the flexibility of ML,
- aligns modeling choices with real-world constraints like budget efficiency and diminishing returns.

---

## Project Overview

This project builds a decision-oriented Customer Lifetime Value (CLV) system using transactional data to support customer prioritization, retention planning, and long-term revenue growth.

Instead of treating CLV as a static metric, the system is designed to translate customer behavior into actionable insights for marketing, CRM, and growth teams.


---

## Dataset Overview

The analysis uses the Online Retail II dataset from the UCI Machine Learning Repository, which contains real transactional data from a UK-based non-store online retailer.
- Time period: December 2009 – December 2011
- Industry: E-commerce / Retail
- Granularity: Transaction-level purchase history
- Primary use cases: Customer behavior analysis, retention strategy, CLV modeling

This dataset is widely used in industry and academia to study repeat purchasing behavior and long-term customer value.

---

## Data Source

- Repository: UCI Machine Learning Repository
- Dataset name: Online Retail II
- Link: https://archive.ics.uci.edu/dataset/502/online+retail+ii
- Creator: Daqing Chen
- License: Creative Commons Attribution 4.0 International (CC BY 4.0)

---

## Business Problem

Many businesses still rely on short-term revenue metrics when making marketing and retention decisions.
This often leads to:
- Over-investing in low-value customers
- Under-investing in high-potential customers
- Reactive decision-making instead of forward-looking strategy

This project addresses the following questions:
- How can we estimate future customer value, not just historical spend?
- How do purchase frequency, recency, and monetary value jointly shape long-term value?
- How can CLV be used to guide concrete retention and engagement actions?

---

## Approach

This project follows an end-to-end analytical workflow:

1. **Data Preparation**
   - Transaction-level cleaning and validation
   - Handling missing values and irregular records
   - Customer-level aggregation

2. **Exploratory Data Analysis (EDA)**
   - Purchase frequency patterns
   - Monetary value distribution
   - Customer behavior insights

3. **Feature Engineering**
   - Recency, Frequency, and Monetary (RFM-style) features
   - Aggregation at customer level
   - Calibration and observation window alignment

4. **CLV Modeling**
   - Probabilistic modeling to estimate future purchase behavior and spend
   - Forward-looking CLV estimation over a fixed horizon
   - Interpretation focused on decision quality, not just model accuracy

5. **ML-Enhanced CLV**
   - Machine-learning layer built on top of probabilistic CLV
   - Predicts realized future revenue using CLV as a strong prior
   - Improves ranking and prioritization in high-value segments

---

## Key Insights

- Customers with similar historical revenue can have very different future value profiles
- High CLV does not always imply low churn risk — value and risk must be assessed jointly
- Probabilistic CLV provides stability, while ML adds flexibility in capturing non-linear behavior
- CLV-based segmentation enables smarter retention spend allocation

---

## Business Impact and Use Cases

This framework can support:
- Retention and win-back prioritization
- High-value customer protection strategies
- Targeted upsell and cross-sell initiatives
- Budget allocation based on expected future return, not past revenue

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Lifetimes (BG/NBD, Gamma-Gamma models)

---

## Author
Ilham Den Fatah  
Aspiring Data Scientist with a background in business & operations and decision-driven analytics