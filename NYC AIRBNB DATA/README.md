 🏙️ Sprint 1: Spreadsheet Data Analysis – NYC Airbnb Market

Welcome to my second business intelligence project from the TripleTen Data Analytics Bootcamp. This project showcases my ability to clean spreadsheet data, create pivot tables, and generate actionable insights for a client in the vacation rental market.

---

## 📌 Project Summary

**Client:** Anonymous Real Estate Investor  
**Objective:** Recommend ideal neighborhoods and property sizes in Manhattan for vacation rental investment based on Airbnb data  
**Tools:** Google Sheets, Pivot Tables, Data Cleaning, Basic Excel Functions  
**Duration:** ~2 hrs 20 min

---

## 🗽 Project Background

The client is exploring investment opportunities in New York City’s vacation rental market. They want data-driven recommendations on:

1. Which **neighborhoods** and **property sizes** (number of bedrooms) are most attractive.
2. Which listings generated the most **revenue** based on Airbnb activity.

---

## 📊 Analysis Overview

### 🔍 1. Attractiveness by Neighborhood & Property Size

- **Metric Used:** Number of reviews in the last 12 months (proxy for demand)
- **Top Neighborhoods:**  
  - Lower East Side  
  - Hell’s Kitchen  
  - Harlem  
  - Midtown  
  - Upper West Side  
  - Chelsea  
  - East Village  
  - East Harlem  
  - West Village  
  - Upper East Side

- **Most Popular Property Size:**  
  - 1-Bedroom listings were the most popular in nearly every neighborhood  
  - Midtown had a preference for **studio** apartments

---

### 💰 2. Revenue Analysis

To estimate earnings:
- Cleaned calendar data and calculated nightly revenue (only when “available” = false)
- Summed 30-day revenue and projected **annual revenue** by multiplying by 12

> 📈 **Top Listing ID:** `49946551`  
> 💵 **30-Day Revenue:** `$29,940`  
> 📆 **Estimated Annual Revenue:** `$359,280`

---

## ✅ Key Recommendations

- Focus investments on 1-bedroom units in high-demand neighborhoods (e.g., Hell’s Kitchen, East Village)
- Target studio units only in Midtown, where they outperform
- Prioritize listings that align with top revenue-generating profiles
- Use review data as a leading indicator of demand when analyzing other regions

---

## 🧹 Data Cleaning Steps

- Created `neighborhood_clean` column to fix inconsistent naming
- Replaced blank `bedrooms` with `0` to represent studios → stored in `bedrooms_clean`
- Added `top_listing`, `revenue_earned`, and `annual_revenue` columns using formula logic and `SUMIF()`

---

## 📄 Final Report

📎 **[Download Full PDF Report](./nyc%20airbnb%20data%20analysis.pdf)**  
_(Make sure to upload this PDF to your GitHub repo.)_

---

## 🛠️ Skills Demonstrated

- Spreadsheet cleaning & transformation
- Pivot table analysis
- Revenue modeling using spreadsheet formulas
- Business recommendation development
- Analytical thinking with minimal code

---

## 👩🏽‍💼 About Me

**Author:** Chiamaka Obieli  
**Role:** Aspiring Business Intelligence Analyst  
**Bootcamp:** TripleTen Data Analytics Program  
**LinkedIn:** [Your LinkedIn Profile URL]  
**Email:** [your.email@example.com]

---

## 🚀 What’s Next?

Future projects will explore hands-on data analysis with SQL, Python, and Power BI. This project built the foundation for transforming raw spreadsheet data into powerful business insights.
