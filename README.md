
# Amazon E-Commerce Sales & Inventory Analysis

![Python](https://img.shields.io/badge/Python-Data%20Analysis-blue?logo=python)
![SQL](https://img.shields.io/badge/SQL-MySQL-orange?logo=mysql)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![Excel](https://img.shields.io/badge/Excel-Advanced-green?logo=microsoftexcel)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

**Project Duration:** July 2026 – September 2026  
**Project Domain:** E-Commerce | Sales Analytics | Inventory Analytics  
**Role:** Data Analyst  
**Author:** Pavan Kumar N

---

## 📌 Project Overview

The **Amazon E-Commerce Sales & Inventory Analysis** project is an end-to-end data analytics project designed to analyze e-commerce sales performance, customer purchasing patterns, product category performance, regional revenue distribution, and inventory levels.

The project demonstrates the complete data analytics workflow, starting with data cleaning and exploratory data analysis using Python, followed by database creation and SQL-based analysis in MySQL, and concluding with interactive dashboards and business insights using Power BI.

The primary objective is to transform raw sales and inventory data into meaningful insights that support business reporting, performance monitoring, and data-driven decision-making.

---

## 🎯 Project Objectives

- Analyze overall sales performance and revenue trends.
- Identify top-performing product categories and SKUs.
- Evaluate regional sales and revenue distribution.
- Understand customer purchasing behavior and customer segments.
- Analyze sales performance across different days of the week.
- Examine inventory levels and stock availability.
- Identify low-stock and out-of-stock products.
- Develop interactive dashboards to monitor key business KPIs.
- Generate actionable insights to support business decisions.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Data cleaning, transformation, and analysis |
| Pandas | Data manipulation and preparation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| MySQL | Database creation and data storage |
| SQL | Data querying and business analysis |
| Excel | Data inspection and reporting |
| Power BI | Interactive dashboards and reporting |
| DAX | KPI calculations and measures |
| Power Query | Data transformation and preparation |

---

## 📂 Dataset Description

The project uses two primary datasets:

### 1. Amazon Sales Dataset

Contains e-commerce sales transaction information, including fields such as:

- Order ID
- Date
- SKU
- Product category
- Quantity
- Sales amount
- Customer type
- Sales channel
- Shipping information
- Promotion details
- Order status

### 2. Inventory Dataset

Contains product inventory information, including fields such as:

- SKU
- Product details
- Category
- Stock quantity
- Inventory status

**Note:** Column names and available fields may vary according to the original dataset and its cleaned version.

---

## 🔄 Project Workflow

```text
Raw Sales & Inventory Data
            |
            v
    Python Data Cleaning
            |
            v
 Exploratory Data Analysis
            |
            v
    MySQL Database
            |
            v
       SQL Analysis
            |
            v
    Power BI Modeling
            |
            v
 Interactive Dashboards
            |
            v
 Business Insights & Reporting
```

---

## 🐍 1. Python – Data Cleaning & Exploratory Data Analysis

Python was used to prepare the raw datasets for analysis and improve data quality.

### Data Cleaning

- Inspected the datasets and reviewed their structure.
- Standardized column names.
- Removed unnecessary whitespace and corrected formatting inconsistencies.
- Examined missing and duplicate records.
- Handled missing values where appropriate.
- Checked data types and converted fields where required.
- Identified zero-quantity and zero-amount records.
- Prepared cleaned datasets for SQL analysis.

### Exploratory Data Analysis (EDA)

Performed analysis to understand:

- Sales and revenue distribution.
- Product category performance.
- Customer segment contribution.
- Regional sales patterns.
- Order and quantity trends.
- Inventory availability and stock status.
- Sales patterns by day of the week.

### Python Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

---

## 🗄️ 2. MySQL – Database & SQL Analysis

MySQL was used to store the cleaned datasets and perform structured business analysis.

### Database

```sql
CREATE DATABASE fashion_retail_analytics;

USE fashion_retail_analytics;
```

### Tables

- `amazon_sales_cleaned`
- `inventory_cleaned`

### SQL Concepts Applied

- SELECT
- WHERE
- DISTINCT
- ORDER BY
- GROUP BY
- HAVING
- Aggregate functions
- INNER JOIN
- LEFT JOIN
- RIGHT JOIN
- CASE statements
- Subqueries
- Common Table Expressions (CTEs), where applicable
- Date-based analysis
- Revenue and inventory calculations

### Business Analysis Using SQL

SQL queries were used to investigate:

- Total revenue and units sold.
- Total orders.
- Category-wise revenue and quantity.
- State-wise sales performance.
- Customer segment analysis.
- Sales trends by day of the week.
- SKU-level performance.
- Inventory stock status.
- Sales and inventory comparisons.

---

## 📊 3. Power BI – Dashboard Development

Power BI was used to create an interactive dashboard for monitoring sales performance and inventory metrics.

### Dashboard KPIs

| KPI | Description |
|---|---|
| Total Revenue | Overall sales revenue |
| Total Units Sold | Total quantity sold |
| Total Orders | Distinct order count |
| Total Stock | Available inventory quantity |
| Category Sales | Revenue and units by product category |
| Regional Revenue | Revenue by shipping state |
| Customer Analysis | B2B and B2C performance |
| Inventory Status | In-stock, low-stock, and out-of-stock products |

### Dashboard Visualizations

- KPI cards
- Category-wise sales charts
- State-wise revenue charts
- Customer segment analysis
- Day-of-week sales analysis
- Inventory status visuals
- SKU performance charts
- Interactive slicers and filters

### Power BI Features

- Data modeling
- Table relationships
- Power Query transformations
- DAX measures
- Interactive filtering
- KPI cards
- Business-focused dashboard design

### Sample DAX Measures

**Total Revenue**

```dax
Total Revenue =
SUM(amazon_sales_cleaned[amount])
```

**Total Units Sold**

```dax
Total Units Sold =
SUM(amazon_sales_cleaned[qty])
```

**Total Orders**

```dax
Total Orders =
DISTINCTCOUNT(amazon_sales_cleaned[order_id])
```

**Total Stock**

```dax
Total Stock =
SUM(inventory_cleaned[stock])
```

**Note:** These measures assume the column names and table structure match the cleaned dataset. Adjust them if your Power BI model uses different names.

---

## 📈 4. Key Performance Indicators

The following figures are based on the analysis results recorded during the project. Verify them against the final cleaned datasets and dashboard before publishing.

| KPI | Result |
|---|---:|
| Total Revenue | ₹17.38 Million |
| Total Units Sold | 26,706 |
| Total Orders | 26,145 |
| Total Inventory Stock | 242,386 |

---

## 🔍 5. Key Business Insights

### Category-Wise Performance

| Category | Revenue | Units Sold |
|---|---:|---:|
| Set | ₹9,229,991.27 | 10,792 |
| Kurta | ₹4,989,452.51 | 10,958 |
| Western Dress | ₹1,732,455.19 | 2,248 |
| Top | ₹1,068,326.76 | 2,118 |

**Insight:** Sets and kurtas account for substantial sales revenue and volume in the analyzed dataset. Category-level monitoring can help businesses evaluate product demand and plan inventory.

### Regional Sales Performance

| State | Revenue | Units Sold |
|---|---:|---:|
| Maharashtra | ₹2,927,366.60 | 4,606 |
| Karnataka | ₹2,234,830.05 | 3,550 |
| Uttar Pradesh | ₹1,547,161.22 | 2,235 |
| Telangana | ₹1,436,801.13 | 2,232 |
| Tamil Nadu | ₹1,274,316.81 | 2,215 |
| Delhi | ₹1,002,127.54 | 1,482 |
| Kerala | ₹822,821.93 | 1,308 |

**Insight:** Maharashtra and Karnataka contribute significant revenue in the analyzed data. Regional performance analysis can help businesses understand geographical demand and support regional planning.

### Customer Segment Analysis

| Customer Type | Revenue | Units Sold | Orders |
|---|---:|---:|---:|
| B2C | ₹17,212,479.01 | 26,457 | 25,933 |
| B2B | ₹165,551.19 | 249 | 212 |

**Insight:** B2C transactions account for the majority of recorded revenue, units, and orders in this dataset. Segment analysis helps businesses understand the composition of sales.

### Sales by Day of the Week

| Day | Units Sold |
|---|---:|
| Saturday | 4,528 |
| Thursday | 4,520 |
| Wednesday | 4,428 |
| Friday | 4,414 |
| Sunday | 3,073 |
| Tuesday | 2,877 |
| Monday | 2,866 |

**Insight:** Saturday, Thursday, Wednesday, and Friday have higher recorded unit sales than the other days in this dataset. Day-level analysis can support sales planning and promotional scheduling.

### Inventory Status

| Inventory Status | SKU Count |
|---|---:|
| In Stock | 5,278 |
| Low Stock | 3,359 |
| Out of Stock | 538 |

**Insight:** Inventory status analysis helps identify products that may need replenishment and supports stock monitoring.

---

## 💡 6. Business Recommendations

Based on the analysis, the following actions can be considered:

- Monitor category-level sales to understand changing product demand.
- Review inventory for low-stock and out-of-stock SKUs.
- Use regional sales trends to inform distribution and planning.
- Track B2C and B2B performance separately.
- Monitor sales patterns across weekdays to inform promotional planning.
- Use dashboards to support regular business reviews and KPI monitoring.
- Validate sales and inventory records regularly to maintain reporting accuracy.

These are analytical recommendations derived from the dataset; actual business decisions should also consider costs, margins, supply constraints, and operational context.

---

## 📁 Project Files

The project includes the following cleaned data files:

```text
Amazon_Sales_Cleaned.csv
Inventory_Cleaned.csv
Sales_Inventory_Analysis.csv
```

### Suggested Repository Structure

```text
Amazon-E-Commerce-Sales-Inventory-Analysis/
│
├── data/
│   ├── Amazon_Sales_Cleaned.csv
│   ├── Inventory_Cleaned.csv
│   └── Sales_Inventory_Analysis.csv
│
├── notebooks/
│   └── Python_Data_Cleaning_and_EDA.ipynb
│
├── sql/
│   └── Sales_Inventory_Analysis.sql
│
├── powerbi/
│   └── Sales_Inventory_Dashboard.pbix
│
├── images/
│   └── dashboard_screenshot.png
│
└── README.md
```

*This is a suggested structure. Keep only files and folders that actually exist in your repository.*

---

## 🧠 Skills Demonstrated

- Data Cleaning and Preparation
- Exploratory Data Analysis (EDA)
- Python Data Analysis
- Pandas and NumPy
- SQL Querying and Data Analysis
- MySQL Database Management
- Data Visualization
- Power BI Dashboard Development
- DAX Measures
- Data Modeling
- KPI Reporting
- Sales and Inventory Analysis
- Business Insights and Reporting

---

## 🎓 Project Outcome

This project demonstrates an end-to-end data analytics workflow using Python, MySQL, SQL, Excel, and Power BI. It showcases the ability to prepare and analyze datasets, query structured data, develop interactive dashboards, monitor business KPIs, and communicate findings through business-focused insights.

---

## 👨‍💻 About the Author

**Pavan Kumar N**  
Data Analyst | SQL | Python | Power BI | Excel

I have over three years of professional experience in operations, helpdesk coordination, reporting, and stakeholder communication, along with completed Data Analytics training and a six-month Data Analyst internship at B Dreams Global Solutions.

My technical skills include SQL, Python, Power BI, Excel, data cleaning, data analysis, visualization, and dashboard development. I have worked on analytics projects involving sales, inventory, and customer shopping behavior.

I am interested in Data Analyst, Junior Data Analyst, BI Analyst, and MIS Analyst opportunities where I can apply my analytical and reporting skills.

### Connect With Me

- **GitHub:** https://github.com/pavankumarn136-pixel
- **Portfolio:** https://pavankumarn136-pixel.github.io/
- **LinkedIn:** https://www.linkedin.com/in/pavan-kumar-n-3677b1238/

---

## ⭐ Thank You

Thank you for visiting my project!

If you find this project useful, feel free to explore the repository and connect with me.
