
Zuber Ride-Share Analysis – SQL & Data Exploration

This project was completed as part of the TripleTen Data Analytics Bootcamp. I took on the role of a business analyst for **Zuber**, a new ride-sharing company launching in **Chicago**. The goal was to analyze competitor taxi data, explore ride patterns, and test a hypothesis about the effect of **weather on ride durations**.

---

Project Summary

**Client:** Zuber Ride-Sharing (Startup)  
**Toolset:** SQL (PostgreSQL), Relational Databases  
**Dataset:** Public taxi and weather data for Chicago  
**Goal:**  
- Understand taxi company performance  
- Identify ride patterns by time and location  
- Test how **weather impacts ride duration** from the Loop to O’Hare Airport

---

Database Structure

Tables Used:

1. **neighborhoods**
   - `neighborhood_id`, `name`
2. **cabs**
   - `cab_id`, `vehicle_id`, `company_name`
3. **trips**
   - `trip_id`, `cab_id`, `start_ts`, `end_ts`, `duration_seconds`, `distance_miles`, `pickup_location_id`, `dropoff_location_id`
4. **weather_records**
   - `record_id`, `ts`, `temperature`, `description`

 *Note:* `trips.start_ts` and `weather_records.ts` were joined using **rounded hour timestamps**.

---

Step 1: Exploratory Data Analysis (EDA)

Questions Answered:

1. **Top Taxi Companies by Ride Volume (Nov 15–16, 2017)**  
   - Field: `trips_amount` (count of rides per company)  
   - Result: Flash Cab and Taxi Affiliation Services had the highest volume.

2. **Performance of 'Yellow' and 'Blue' Taxis (Nov 1–7, 2017)**  
   - Used a `LIKE` filter on `company_name`  
   - Focused only on taxi companies with "Yellow" or "Blue" in the name

3. **Flash Cab vs Taxi Affiliation Services vs Others**  
   - Grouped all other companies into an "Other" category  
   - Sorted results by total rides taken

*Insight:* Flash Cab and Taxi Affiliation Services dominate Chicago’s taxi market.

---

Step 2: Hypothesis Test – Rainy Saturday Rides

**Objective:**  
Analyze if ride **duration from Loop (ID 50) to O’Hare (ID 63)** increases on **rainy Saturdays**.

Steps Performed:

1. **Tagged Weather Conditions:**
   - Used `CASE` to label each hour as:
     - `"Bad"` → if `description` included "rain" or "storm"
     - `"Good"` → all other conditions

2. **Filtered Ride Data:**
   - From **Loop to O’Hare only**
   - Day: **Saturday only**
   - Joined to weather data using `start_ts = ts`

3. **Calculated Ride Durations:**
   - Focused only on records with valid weather info

*Result:* The average ride duration **increased significantly during “Bad” weather** on Saturdays compared to “Good” weather.

---

Key Takeaways

- Zuber can expect **longer ride durations** in bad weather, especially on weekends.
- This insight is critical for:
  - Pricing algorithms
  - Driver dispatch planning
  - Customer wait time estimations

---

Final Report

📎 [Download Full SQL Project Report (PDF)](./Your_Zuber_Project_File.pdf)  
_(Replace with your actual PDF file name and ensure it's uploaded to your repo.)_

---

Skills Demonstrated

- Advanced SQL Querying
- Time-based Data Joins
- Data Cleaning & Filtering
- CASE Logic & Aggregation
- Exploratory Data Analysis
- Hypothesis Testing using Real-World Data

---

About Me

**Author:** Chiamaka Obieli  
**Role:** Aspiring Business Intelligence Analyst  
**Bootcamp:** TripleTen Data Analytics Program  
**LinkedIn:** [Chiamaka Obieli](www.linkedin.com/in/chiamaka-obieli-939b5284) 
**Email:** [somaksy@gmail.com]

---

What’s Next?

Next steps in my analytics journey include:
- Predictive modeling with Python
- Building interactive dashboards with Power BI & Tableau
- Automating ETL pipelines for real-time insights

_Thank you for visiting this project. Feel free to connect with me on LinkedIn or explore my other case studies._
Data_projects_TripleTen/Zuber README.md at main · amakab/Data_projects_TripleTen 
