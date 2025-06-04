Business Analytics Project – E-commerce Funnel & Retention Analysis

Welcome to my Business Analytics project as part of the TripleTen Data Analytics Bootcamp. This project simulates a real-world scenario in which I was hired as a **Junior Analyst** at an e-commerce company to transform raw transaction logs into actionable business metrics, with a focus on **conversion funnel creation** and **customer retention analysis via cohorts**.

---

Project Overview

**Company Context:** E-commerce  
**Project Title:** Turning Event Logs into Business Metrics  
**Role:** Junior Business Analyst  
**Tools Used:** Google Sheets, Pivot Tables, Spreadsheet Functions  
**Dataset:** Raw user activity logs from the company’s website  
**Duration:** ~3 hours  

---

Objective

Analyze raw event logs and answer key business questions:

1. How well does the website convert product views into purchases?
2. What does user retention look like based on monthly acquisition cohorts?
3. How can these insights inform product and marketing strategies?

---

Project Deliverables

Conversion Funnel

- **Stages Analyzed:**  
  - `view` → `shopping_cart` → `purchase`
- **Conversion Rates:**  
  - View to Cart: **29%**  
  - Cart to Purchase: **36%**  
- **Key Insight:**  
  Users who add items to their cart show a high likelihood of completing a purchase, indicating an effective checkout process.

📄 Sheet: `conversion_funnel`

---

Cohort Analysis

- Created acquisition cohorts based on **first purchase month**
- Tracked each cohort’s engagement over a **5-month period**
- Metrics: **Unique user counts** per month since first purchase

📄 Sheet: `cohort_analysis`

---

Retention Rate Calculation

- Used `DATEDIF()` to calculate **cohort age**
- Calculated monthly **retention rates** for each cohort
- **Insight:**  
  Significant drop in engagement after month 1, with most cohorts losing over 90% of users by month 2

📄 Sheet: `retention_rates`

---

Data Preparation & Cleaning

- Filtered event types to isolate purchases
- Created `first_purchase_date`, `event_month`, `first_purchase_month`, and `cohort_age` columns
- Used `VLOOKUP()`, `TEXT()`, and `DATEDIF()` functions to enrich and prepare data

📄 Sheet: `purchase_activity`, `first_purchase`

---

## Executive Summary (from project report)

- **Conversion Funnel:**  
  The website has a solid cart-to-purchase conversion rate (36%), but could improve initial engagement from product views.
  
- **Retention Analysis:**  
  Retention rates fall sharply after the first month. This indicates a need for improved post-purchase engagement strategies.

📄 Sheet: `executive_summary`

---

Skills Demonstrated

- Conversion Funnel Design
- Retention & Cohort Analysis
- Pivot Table Construction
- Spreadsheet Functions (`VLOOKUP`, `DATEDIF`, `TEXT`)
- Data Cleaning & Restructuring
- Business Insight Communication

---

View Full Report

📎 [Download PDF Report](./Copy%20of%20Business%20Analytics%20Project.pdf)  

---

About Me

**Author:** Chiamaka Obieli  
**Role:** Aspiring Business Intelligence Analyst  
**Bootcamp:** TripleTen Data Analytics Program  
**LinkedIn:** [Chiamaka Obieli](www.linkedin.com/in/chiamaka-obieli-939b5284)  
**Email:** [somaksy@gmail.com]

---

What’s Next?

In future projects, I will transition from spreadsheet-based analysis to using SQL, Python, and BI tools like Power BI and Tableau to perform more advanced analytics and build dynamic dashboards.

