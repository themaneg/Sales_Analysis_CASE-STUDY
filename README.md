# Sales_Analysis_CASE-STUDY
# Sales Performance Analysis — Databricks SQL Case Study

### Overview
This project analyzes a retail product’s daily sales performance using **Databricks SQL**, based on the provided `Sales Case Study (2).csv` dataset.  
The goal is to calculate key metrics, detect promotional periods, evaluate price elasticity, and generate performance classifications using SQL logic and visualization dashboards.

---

### Dataset Description
The dataset includes:
- **Date** – Day of sale  
- **Sales** – Total Rand value of sales  
- **Cost of Sales** – Total Rand value of product cost  
- **Quantity Sold** – Units sold  

---

### Key Objectives
1. Compute daily and average **unit price**, **gross profit**, and **gross profit %**  
2. Detect **promotion periods** where prices drop significantly  
3. Calculate **price elasticity of demand** to measure customer sensitivity  
4. Use **CASE logic** for performance classification: Excellent, Good, Average, Poor  
5. Build a **Databricks SQL dashboard** with KPIs and visuals  

---

### KPIs & Metrics
| Metric | Description |
|--------|--------------|
| **Average Unit Price** | Mean price per unit sold |
| **Average GP%** | Average gross profit percentage |
| **Total Sales** | Total Rand value of sales |
| **Elasticity** | % Change in Quantity / % Change in Price |
| **Performance Rating** | CASE-based classification by GP% and sales |

---

### Insights & Visuals
- **Promotion Detection:** 10% price drop below 7-day rolling average  
- **Elasticity Analysis:** Evaluates demand reaction during promotions  
- **Performance Dashboard:** Databricks SQL visuals for trends and KPIs  
- **Excel Export:** `Sales_Performance_KPI.xlsx` summarizing daily results  

---

### Project Workflow
1. **Data Ingestion:** Load CSV into Databricks table `sales_raw`  
2. **Transformation:** Compute metrics (`sales_enriched`)  
3. **KPI Computation:** Average sales, margin %, total units  
4. **Promotion Detection:** Using rolling averages and CASE  
5. **Elasticity Analysis:** Compare promo vs baseline periods  
6. **Classification:** CASE-based profit and sales performance  
7. **Visualization:** Create SQL dashboards and charts  
8. **Reporting:** Export to Excel and summarize insights  

---

### Visualization Plan
A Miro-style flowchart illustrates the end-to-end process from data ingestion to reporting, ensuring clarity before execution.  
*(Refer to the included `Sales_Performance_Analysis_Flow.png` for the visual process.)*

---

### Technologies Used
- **Databricks SQL**
- **Spark SQL Window Functions**
- **Excel Export (KPI Summary)**
- **Miro Flow Plan (Visualization of Workflow)**

---

### Outputs
- `sales_enriched` table (cleaned & derived metrics)  
- `promo_periods` and `elasticity_results` tables  
- `Sales_Performance_KPI.xlsx` Excel summary  
- Databricks SQL Dashboard for visualization  

---

### Example KPIs
- **Avg Unit Price:** R XX.XX  
- **Avg GP%:** XX%  
- **Top Performance Days:** Dates with >45% GP% and high sales volume  
- **Elasticity:** Indicates whether demand is elastic (>-1) or inelastic (<-1)

---

### 🧩 Author
**Gary Themane** — Sales Analytics | Databricks SQL | Data-Driven Insights  
