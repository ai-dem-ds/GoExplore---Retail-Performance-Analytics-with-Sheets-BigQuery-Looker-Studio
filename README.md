###  📊 GoExplore – Retail Analytics Project

####  **End-to-End Data Analysis: Google Sheets → BigQuery → Looker Studio**

**🌐 Summary**

This project demonstrates a complete data analytics pipeline built for GoExplore, a fictional outdoor retail company.
The goal was to collect raw sales and product data, prepare and store it in BigQuery, calculate core business KPIs using SQL, and visualize insights in an interactive dashboard created with Looker Studio.

The project highlights practical skills in data cleaning, data modeling, querying, and business-oriented analytics—similar to real-world workflows in data analytics and BI teams.

**🛠️ Languages, Tools & Libraries Used**

* Google Sheets – data collection, cleaning, formatting, and source tables
* BigQuery (Google Cloud) – data warehouse, SQL queries, KPI calculations
* SQL – data transformation and analysis
* Looker Studio (Google Data Studio) – dashboard creation and data visualization
* Google Cloud Connector – linking Sheets ↔ BigQuery & BigQuery ↔ Looker Studio

**📚 Key Learnings**
**Technical Skills**

* Understanding how a data warehouse works and why BigQuery is optimized for analytics.
* Learning how to upload data from Google Sheets to BigQuery and define schemas correctly.

**Writing clean SQL queries using:**
* CTEs (WITH statements)
* Aggregations (SUM, AVG, COUNT)
* GROUP BY for monthly/yearly KPIs
* JOINs to combine sales, products, and retailers
* Designing core business KPIs, such as:
* Total Revenue
* Total Profit
* Revenue by Month / Year / Country
* Top 10 Products by Revenue
* Active Retailers
* Creating a Star-Schema-like structure across tables (Daily Sales, Products, Retailers, Methods).
* Analytics & Visualization
* Building an interactive Looker Studio Dashboard with:
* Trendlines
* Maps (Geo Revenue)
* KPI scorecards
* Top-N tables
* Filters for Region, Retailer Type, and Dates
* Understanding how dashboards help non-technical users interpret results instantly.
* Communication
* Explaining SQL results in clear business language.
* Structuring insights for presentations and stakeholder consumption.

**🧠 Challenges Overcome**

**1. Date Format Errors in BigQuery**

Uploading Google Sheets CSVs often resulted in errors (“Cannot find matched format element at…”) due to inconsistent DD/MM/YYYY vs MM/DD/YYYY formatting.
Solution: Cleaned and standardized dates inside Google Sheets before upload.

**2. Schema Mismatch & Data Type Issues**

Some columns (e.g., product_number, unit_sale_price) were recognized incorrectly.
Solution: Manually adjusted schema in BigQuery to match the correct data types.

**3. Differences Between Retailer Counts**

Daily Sales contained only active retailers; the Retailers table stored all.
Solution: Understood the difference between full dimension tables and fact-level activity.

**4. Understanding CTEs (WITH statements)**

Originally unclear; later became essential for writing clear, reusable SQL.
Solution: Practiced by rewriting KPIs with clear CTE naming.

**5. Dashboard Filtering Logic**

Ensuring KPIs updated dynamically with date/region filters.
Solution: Carefully linked KPIs to correct BigQuery tables and aggregated views.

#### **🎯 Additional Reflections**

This project significantly improved my confidence in SQL, BigQuery, and dashboard design. It helped me understand a realistic workflow of data collection → storage → transformation → visualization.
It also strengthened my ability to explain technical concepts clearly and break down complex tasks into logical steps.

I now feel more prepared for roles that involve data analysis, BI, dashboard development, and communication with non-technical stakeholders.
