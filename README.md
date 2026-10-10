# 📦 Supply Chain & Logistics Analytics

### End-to-End Data Analytics Project using SQL Server, Power BI & Excel

An end-to-end Supply Chain Analytics project that combines SQL Server data architecture, Excel dashboards, and interactive Power BI reports to analyze business operations and logistics performance.

**Project Workflow**

Raw Data → ETL → Data Warehouse → Data Modeling → SQL Analytics → Power BI & Excel → Business Insights

---

## 📌 Project Overview

Supply chain operations generate data across orders, customers, products, sales, shipping, and delivery processes. Analyzing this data helps organizations understand performance, identify operational inefficiencies, and make informed business decisions.

This project brings together data engineering, data analysis, and business intelligence in a single analytical solution.

The project focuses on:

- 📈 Sales and profitability analysis
- 👥 Customer performance
- 📦 Product performance
- 🚚 Order fulfillment
- 🚛 Shipping and delivery performance
- 🌎 Regional and market analysis
- ⏱️ Delivery delays and logistics efficiency

Rather than relying only on dashboards, the project also includes SQL Server data architecture and scripts to organize data for analytical reporting.

## 🎯 Project Objectives

- Build a structured SQL Server data warehouse.
- Implement a Bronze → Silver → Gold data architecture.
- Clean and transform raw data using SQL.
- Develop business-ready analytical tables and views.
- Create Excel dashboards for performance analysis.
- Develop interactive Power BI dashboards.
- Analyze supply chain and logistics KPIs.
- Translate operational data into actionable business insights.

## 📐 Project Documentation

The `Docs` folder contains supporting project documentation and architecture diagrams.

The documentation section covers:

- **Data Architecture:** Overall structure of the data warehouse.
- **Data Lineage:** Movement of data through the processing workflow.
- **Data Model:** Relationships between analytical tables, where available.

## 🗄️ SQL Server Data Architecture

The SQL Server component follows a layered data processing approach.

### 🥉 Bronze Layer — Raw Data

The Bronze layer is the initial landing layer for source data.

**Purpose**
- Load and preserve source data.
- Maintain a raw-data foundation for transformation.
- Separate source ingestion from downstream processing.

### 🥈 Silver Layer — Cleaned & Standardized Data

The Silver layer is used to prepare data for downstream analytical processing.

**Typical transformation activities**
- Data cleaning and standardization
- Handling missing or invalid values
- Data type conversion
- Data validation
- Duplicate identification and handling

### 🥇 Gold Layer — Business-Ready Data

The Gold layer contains the analytical structures used to support reporting and business analysis.

The Gold layer supports the preparation of reporting-oriented datasets for business intelligence.

### Database Initialization

The database initialization script is:

`init_database_RE.sql`

Review the SQL scripts and database configuration before executing them in your own environment.

## 🔄 ETL Pipeline

The project workflow can be summarized in three main stages.

**1. Extract**
- Load data from the source dataset into the SQL Server environment.

**2. Transform**
- Clean and standardize the data.
- Validate fields and data types.
- Prepare data for analytical use.

**3. Load**
- Organize the processed data into the Gold layer.
- Prepare reporting datasets for Excel and Power BI.

**Overall Workflow**

Source Data → Bronze → Silver → Gold → Reporting & Analysis

## 📊 Power BI Dashboard

The Power BI report provides interactive visual analysis of supply chain and logistics performance.

### Dashboard Preview
Supply Chain Analytics
<img width="1733" height="927" alt="Screenshot 2026-10-10 140923" src="https://github.com/user-attachments/assets/19c68dc0-4fd5-48d3-8447-ff231c7ee3ea" />

Customer Analytics
<img width="1735" height="922" alt="Screenshot 2026-10-10 141015" src="https://github.com/user-attachments/assets/a20b4191-789c-487d-8f3b-730909823c00" />

Sales & Product Analytics
<img width="1732" height="925" alt="Screenshot 2026-10-10 141053" src="https://github.com/user-attachments/assets/757b264a-c88d-4866-a472-cfb5ee83f86c" />

Logistics Analytics
<img width="1731" height="925" alt="Screenshot 2026-10-10 141123" src="https://github.com/user-attachments/assets/d9ba1398-08cf-49e3-8545-eaf0b8d79e87" />


## 📈 Excel Dashboard
Excel is used as an additional analysis and reporting tool in this project.

The dashboards provide visual summaries of the analyzed business areas and complement the Power BI reporting solution.

## 📊 Excel Dashboard
Retail Supply Chain Analytics
<img width="1855" height="902" alt="Screenshot 2026-10-10 140224" src="https://github.com/user-attachments/assets/41fafc9c-24a1-427f-9feb-007b5fdc70d4" />

Customer Analytics
<img width="1858" height="902" alt="Screenshot 2026-10-10 140300" src="https://github.com/user-attachments/assets/f7eff1b2-2328-41d5-b2ef-3c6b0b815d6c" />

Product Analytics
<img width="1865" height="890" alt="Screenshot 2026-10-10 140350" src="https://github.com/user-attachments/assets/29bbca71-23af-4775-8501-90b82d674cc7" />

Logistics Performance
<img width="1857" height="895" alt="Screenshot 2026-10-10 140417" src="https://github.com/user-attachments/assets/9ae99382-534c-412a-bc63-af99d8a5935b" />

## 💼 Business Questions

The project supports analysis of practical business questions, including:

### 📈 Sales & Product Analysis
- How does sales performance change over time?
- Which products and business segments perform best?
- Which areas require further profitability analysis?

### 👥 Customer Analysis
- Which customers and customer segments contribute most to sales?
- How does customer performance vary across business segments?

### 📦 Product Analysis
- Which products and categories perform best?
- Which products require additional performance investigation?

### 🚚 Supply Chain & Logistics
- How does delivery performance vary across shipping modes?
- Where are shipping delays concentrated?
- How does actual shipping performance compare with planned performance?
- Which logistics areas require operational attention?


## 📂 Project Structure

```text
supply-chain-analytics/
│
├── README.md
│
├── docs/
│   └── Project documentation and diagrams
│
├── Excel_Dashboard-screenshot/
│   └── Excel dashboard screenshots
│
├── PowerBI_Dashboard/
│   ├── Scm_project.pbix
│   └── Dashboard screenshots
│
└── Sql_Server/
    ├── init_database_RE.sql
    │
    ├── bronze/
    │   ├── ddl_bronzeRE.sql
    │   └── proc_load_bronzeRE.sql
    │
    ├── silver/
    │   ├── ddl_silverRE.sql
    │   └── proc_load_silverRE.sql
    │
    └── gold/
        ├── ddl_goldRE.sql
        └── view_goldRE.sql1.sql
```

## ▶️ How to Explore the Project

### Excel Dashboards
Open the `Excel_Dashboard-screenshot/` folder to explore the Excel dashboard previews.

### Power BI Dashboard
1. Install Microsoft Power BI Desktop.
2. Open `PowerBI_Dashboard/Scm_project.pbix`.
3. Refresh the data source if required by your local configuration.
4. Explore the available report pages and interactive filters.

### SQL Server Architecture
1. Review the scripts in `Sql_Server/`.
2. Check the database initialization and source-data configuration.
3. Execute the scripts in the appropriate order for your database environment.
4. Verify the resulting tables, views, and reporting structures.

Always review initialization scripts before running them, particularly if they drop or recreate databases or tables.

## 🔎 Project Workflow

```text
          SOURCE DATA
               |
               v
        BRONZE LAYER
          Raw Data
               |
               v
        SILVER LAYER
    Clean & Transform
               |
               v
         GOLD LAYER
    Analytical Structures
               |
               v
       BUSINESS REPORTING
          /        \
         v          v
     POWER BI      EXCEL
          \        /
           v      v
        BUSINESS INSIGHTS
```

## 📌 Key Takeaway

This project demonstrates an integrated approach to analytics by combining SQL Server data processing, Excel analysis, and Power BI visualization.

The objective is to transform operational data into structured information that supports supply chain performance monitoring and business decision-making.

## 👨‍💻 About Me

I'm a BBA graduate from Shivaji University building my career in Data Analytics, with a particular interest in Supply Chain & Logistics Analytics.

My technical interests include SQL, Power BI, Excel, data modeling, and business intelligence.

I'm interested in Data Analyst and Business Analyst opportunities where I can use data to solve business and operational problems.

## 🔗 Connect

- GitHub: 
- LinkedIn: www.linkedin.com/in/ravikiranpatole01

⭐ Thank you for exploring my project!
