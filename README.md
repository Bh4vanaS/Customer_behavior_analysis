# Customer_behavior_analysis
Data analytic project showcasing customer behavior analysis using Python,Sql,Power Bi
<<<<<<< HEAD
Here's your advanced GitHub README description in plain text:

---

# 🛒 Customer Shopping Behavior Analysis

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat&logo=python&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-SQL_Analysis-336791?style=flat&logo=postgresql&logoColor=white) ![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-F2C811?style=flat&logo=powerbi&logoColor=black) ![Pandas](https://img.shields.io/badge/Pandas-Data_Wrangling-150458?style=flat&logo=pandas&logoColor=white) ![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=flat)

> **End-to-end data analysis pipeline** uncovering actionable customer insights from 3,900 retail transactions — spanning Python-based EDA, relational SQL querying in PostgreSQL, and interactive Power BI visualization.

---

## 📌 Project Overview

This project delivers a full-stack analytics workflow on a retail transaction dataset. The objective was to move from raw, messy data to strategic business intelligence — identifying high-value customer segments, discount-dependent products, subscription behavior patterns, and revenue distribution across demographics.

The analysis answers real business questions: *Who are our most valuable customers? Which products rely on discounts to sell? Do subscribers actually spend more?*

---

## 🗂️ Dataset

The dataset contains **3,900 transaction records** across **18 feature columns** covering three core dimensions — customer demographics (Age, Gender, Location, Subscription Status), purchase details (Category, Item, Amount, Season, Size, Color), and behavioral signals (Discount Usage, Promo Codes, Purchase Frequency, Shipping Type, Review Ratings). One quality issue was addressed: 37 missing values existed in the `review_rating` column.

---

## ⚙️ Technical Pipeline

**Stage 1 — Data Preprocessing in Python**

Raw data was loaded using Pandas and profiled using `.info()` and `.describe()`. Missing values in `review_rating` were imputed using the **category-level median** rather than a global mean — preserving the distributional integrity of each product group. All column names were standardized to `snake_case` for cross-tool consistency. Two engineered features were created: `age_group` (binned from continuous age values) and `purchase_frequency_days` (derived from frequency labels). A redundancy check between `discount_applied` and `promo_code_used` confirmed overlap, and the latter was dropped. The cleaned DataFrame was exported directly to PostgreSQL via SQLAlchemy.

**Stage 2 — SQL Analysis in PostgreSQL**

Ten structured business queries were executed to answer stakeholder-level questions including revenue by gender, high-spending discount users, top-rated products, shipping type behavior, subscriber vs. non-subscriber spend comparison, discount-dependent products, customer segmentation (New / Returning / Loyal), category-level bestsellers, repeat buyer subscription likelihood, and revenue by age cohort.

**Stage 3 — Power BI Dashboard**

An interactive dashboard was built featuring KPI cards (3.9K customers, $59.76 average purchase, 3.75 average rating), a subscription status donut chart, revenue and sales bar charts by category and age group, and dynamic slicers for Gender, Category, Subscription Status, and Shipping Type.

---

## 📊 Key Findings

Male customers generated **2.1× more revenue** than female customers ($157,890 vs $75,191). **839 customers** used discounts yet spent above the average — representing a strong upsell segment. Express shipping users spent $2 more on average than Standard users. Interestingly, non-subscribers had a marginally higher average spend ($59.87) than subscribers ($59.49), suggesting the subscription program needs stronger value differentiation. Hat, Sneakers, and Coat showed nearly **50% discount dependency**, flagging a margin risk. The customer base skewed overwhelmingly loyal — **80% of customers (3,116)** had an extensive purchase history. Young Adults were the highest-revenue age cohort at $62,143.

---

## 🧠 Business Recommendations

**Subscription Conversion** — Non-subscribers form the majority and spend comparably; tiered exclusive benefits could convert a portion of the 2,847 non-subscribers. **Discount Optimization** — With Hat and Sneakers at ~50% discount rates, A/B price sensitivity testing could recover margin without hurting volume. **Loyalty Reinforcement** — An 80% loyal base is a strong foundation; a structured rewards program could deepen retention at low acquisition cost. **Age-Targeted Campaigns** — Young Adults lead revenue; personalized campaigns aligned to their seasonal and category preferences would maximize ROI. **Express Shipping Upsell** — Higher average spend among Express users suggests a natural bundling opportunity with high-AOV products.

---

## 🛠️ Tech Stack

Python (Pandas, NumPy) for data cleaning, EDA, and feature engineering — SQLAlchemy for the Python-to-PostgreSQL pipeline — PostgreSQL for relational querying and business analysis — Power BI for interactive dashboard and visual storytelling.

---


=======
>>>>>>> b5e2f43bc03db42136a1fabbdfc0a1cde6b63d1c
