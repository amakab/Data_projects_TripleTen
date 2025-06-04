# 📊 Storytelling with Data: Superstore Return Analysis

## 🧠 Project Overview

**Goal**: To analyze customer return behavior at the Superstore and provide actionable insights for executive decision-making.

This business intelligence project investigates the root causes behind returned orders at a fictional Superstore. Through data analysis and visual storytelling using Tableau, we uncovered patterns in customer returns across products, regions, time, and customer demographics. The findings are synthesized in an interactive dashboard and a clear narrative for business stakeholders.

## 📂 Files

- `Superstore.xls` – Raw dataset including orders and returns
- Tableau Workbook – Visual analyses and dashboard (not included in repo)
- Mockups – Dashboard sketches for design planning
- Final PDF Report – Full summary of findings and dashboard screenshots (`Storytelling with data - Project.pdf`)

## ❓ Key Business Question

**What is causing the high number of returned orders at the Superstore?**

---

## 📈 Data Analysis Highlights

To identify drivers of returns, we conducted the following visual analyses:

- 🔹 **Sales vs. Returns Scatterplot**: Correlation of total sales and total returns by sub-category  
- 📊 **Return Rate by Product Category**: Identified highest return categories  
- 👤 **Customer-Level Return Rates**: Filtered for repeat customers to isolate high-return behavior  
- 🗺️ **Geographic Return Rates**: Mapped return rates by state to discover regional trends  
- 📅 **Seasonal Return Trends**: Monthly analysis to identify seasonality in returns  
- ⚙️ **Composite Visuals**: Two multi-factor charts combining geography, product, and time

Each analysis used a `Returned` calculated field (1 for "Yes", 0 for null) to compute return rates.

---

## 📐 Dashboard Design

A dashboard was created to allow executives to monitor return patterns interactively.

### 📌 Key Components

- Return rate trends over time
- Geographical heatmap of return rates
- Return rate by product category and sub-category
- Filterable views by region, product, and customer

### 🖌️ Design Process

- 📝 Sketched 3 low-fidelity mockups
- ✅ Chose and built the most intuitive version using Tableau
- 🧱 Built layout with empty containers to mirror the wireframe
- 🧩 Populated dashboard with interactive charts and filters

---

## 🧾 Narrative Summary

### 📋 Measuring Returns

- **Preferred Metric**: *Return rate* (not just total returns) provides normalized comparison across categories.
- **Alternative Metrics**: Total return count and cost of returns may be useful for financial perspectives.

### 💡 Key Insights

- High return rates were concentrated in specific product subcategories such as **Tables** and **Chairs**.
- Certain **states and regions**, particularly **California and the West**, had elevated return rates.
- Some **customers** showed disproportionately high return behavior, especially those with frequent purchases.
- **Seasonality**: Return rates spiked around certain months, suggesting possible effects from holiday or promotion periods.

### 🧭 Dashboard Interpretation

Users can:
- **Drill down** into return trends by subcategory and state
- **Filter** by customer segments, products, or time periods
- **Compare** high-performing versus high-returning areas to strategize interventions

---

## ✅ Recommended Next Steps

1. **Investigate high-return subcategories** for potential quality or fulfillment issues.
2. **Target regions and customers** with high return rates with tailored messaging or support.
3. **Deploy dashboard organization-wide** to monitor return trends continuously.
4. **Evaluate policy** on returns and customer education to reduce friction.

---

## 📌 Tools & Techniques

- **Data**: Superstore Orders & Returns Dataset (Excel)
- **Visualization**: Tableau (interactive dashboards)
- **Techniques**: Return rate normalization, LEFT JOIN, filtering, geographic & temporal aggregation
- **Design**: Wireframing, UX-first dashboard composition

---

## 🧠 Reflections

This project demonstrates the power of visual analytics and storytelling to inform executive strategy. By focusing on the *"why"* behind return behaviors rather than just the *"what"*, we enable data-driven improvements in operations, customer service, and product management.

---

> 📁 For full visual output, refer to the accompanying Tableau dashboard and PDF summary.

