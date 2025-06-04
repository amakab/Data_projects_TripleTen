# Shopify App Analysis — Power BI Project

## Project Overview

**Objective**: To analyze the landscape of Shopify apps and identify key factors that contribute to app success on the platform.

This Power BI project provides a comprehensive review of publicly available data scraped from the Shopify App Store. The analysis explores app statistics, user reviews, developer responsiveness, and performance indicators to reveal insights that can guide app developers and platform strategists.

## Dataset

- **File**: `shopify.xlsx`
- **Tables Included**:
  - `apps`: Metadata on apps
  - `apps_categories`: Mapping table between apps and categories
  - `categories`: App categories
  - `reviews`: User reviews and developer responses

---

## Power BI Report Structure

The report is organized into **three main sections**, each on its own Power BI page:

### App Landscape

Exploring the overall ecosystem of Shopify apps.

- **KPI Card**: Total unique number of apps
- **Line Chart**: Review count trend over time (`lastmod` date vs. sum of `review_count`)
- **Scatterplot**: Review count vs. average rating
  - Annotated insights highlight which apps achieve high ratings despite fewer reviews.

---

### Reviews

Diving deeper into user feedback and developer engagement.

- **DAX Column**: `helpful_reviews = rating * (1 + helpful_count)`
  - KPI Card showing the average of `helpful_reviews`
- **DAX Column**: `developer_answered = IF(ISBLANK(developer_reply), 0, 1)`
  - Scatterplot: Average rating by whether the developer responded

---

### App Reviews

Joining reviews with app data for developer-specific insights.

- **Relationship**: `reviews.app_id` → `apps.id` (many-to-one)
- **Bar Chart 1**: Developers ranked by total review ratings
- **Bar Chart 2**: Developers ranked by average of `helpful_reviews`
- **Bar Chart 3**: Developer responsiveness (with filter: `reviews_count > 500`)

---

## Key Findings

- Apps with more reviews tend to have varied rating distributions, but high average ratings aren't always tied to high volume.
- Developer responsiveness correlates positively with higher average ratings.
- Some developers achieve high helpful review scores, suggesting quality engagement rather than quantity.
- Visual trends help isolate top-performing categories and identify improvement opportunities for lower-rated developers.

---

## Tools & Techniques

- **Platform**: Microsoft Power BI
- **Modeling**: Relationships, calculated columns using DAX
- **Visuals**: KPI Cards, Scatterplots, Bar Charts, Line Charts
- **Data Insights**: Temporal analysis, sentiment weighting, developer accountability

---

## Screenshots

All visuals and transformations were captured with full-screen screenshots for documentation and validation.

> See the attached Power BI `.pbix` file and project PDF for detailed dashboards and screenshots of each visualization step.

---

## Conclusion

This project demonstrates how Power BI can be used not just for visualization, but for driving strategic product insights in eCommerce. By combining modeling, DAX transformations, and storytelling techniques, we derived actionable insights on the app ecosystem and developer behavior on Shopify.

---

**Author**: *Chiamaka Obieli*  
**LinkedIn**: [Chiamaka Obieli](www.linkedin.com/in/chiamaka-obieli-939b5284)
**Tags**: `Power BI`, `Shopify`, `App Analysis`, `DAX`, `Business Intelligence`
