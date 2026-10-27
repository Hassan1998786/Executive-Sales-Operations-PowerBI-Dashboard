#  Executive Sales & Operational Performance Dashboard

##  Project Overview
An end-to-end Business Intelligence (BI) project designed to monitor commercial and operational performance for executive-level decision-makers. This dashboard aggregates multi-source tabular data into actionable visual insights, tracking cross-regional sales, profitability margins, and supply chain KPIs.

---

##  Tech Stack & Tools
* **Power BI Desktop:** Dashboard design, visual modeling, and UI/UX implementation.
* **Power Query & DAX:** Data transformation (ETL workflows) and advanced metric formulation.
* **Python (Pandas & NumPy):** Synthetic data generation and realistic dataset simulation.
* **GitHub:** Version control, project documentation, and portfolio showcasing.

---

##  Data Architecture & Modeling (Star Schema)
The data model follows a robust **Star Schema** architecture to ensure optimal query performance and accurate cross-filtering:
* **Dimension Tables:**
  * `Dim_Calendar`: Custom date table created via DAX covering full-year analytics.
  * `dim_regions`: Administrative regions and managerial hierarchy.
* **Fact Tables:**
  * `fact_sales`: Transactional sales data, quantities, unit prices, and revenue/cost metrics.
  * `fact_operations`: Daily operational KPIs including inventory levels, fulfillment rates, and delivery lead times.

---

##  Advanced DAX Analytics
Developed a comprehensive suite of calculated measures to drive executive insights:
* **Financial Metrics:** 
  * `Total Revenue = SUM(fact_sales[Total_Revenue])`
  * `Gross Profit = [Total Revenue] - SUM(fact_sales[Total_Cost])`
  * `Gross Margin % = DIVIDE([Gross Profit], [Total Revenue], 0)`
* **Time Intelligence:** 
  * `YoY Revenue Growth %` (Comparing performance against the same period last year).
  * `Revenue 3M Moving Avg` (Smoothing out monthly revenue fluctuations for trend analysis).
* **Operational KPIs:** 
  * Average Fulfillment Rate % and Average Delivery Days.

---

##  UI/UX Executive Design Principles
* **Layout Structure:** Implemented an **F-Pattern** layout, placing high-priority KPI cards at the top for immediate executive visibility.
* **Color Palette:** Utilized a professional Executive Theme (`#1E293B` dark navy, `#2563EB` accent blue, and `#F4F6F8` neutral light background).
* **Clarity:** Reduced visual clutter by streamlining gridlines, applying consistent card borders with subtle drop shadows, and organizing regional breakdowns logically.

---

##  Repository Contents
* `fact_sales.csv`: Processed sales transactional dataset.
* `fact_operations.csv`: Operational and supply chain KPI dataset.
* `dim_regions.csv`: Regional dimension mapping table.
* `executive_theme.json`: Custom Power BI executive color and styling theme.
* `Dashboard_Previews/`: High-resolution screenshots of the Power BI report pages.

---

## 👤 Author
**Hassan Mohammed Ali Al-Hasani**  
*Department of Computing | Umm Al-Qura University*  
[GitHub Profile](https://github.com/YOUR_USERNAME) | [LinkedIn Profile](YOUR_LINKEDIN_URL)
