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

**Scripts**
- ddl_bronzeRE.sql
- proc_load_bronzeRE.sql

### 🥈 Silver Layer — Cleaned & Standardized Data

The Silver layer is used to prepare data for downstream analytical processing.

**Typical transformation activities**
- Data cleaning and standardization
- Handling missing or invalid values
- Data type conversion
- Data validation
- Duplicate identification and handling

**Scripts**
- `Sql_Server/silver/ddl_silverRE.sql`
- `Sql_Server/silver/proc_load_silverRE.sql`

### 🥇 Gold Layer — Business-Ready Data

The Gold layer contains the analytical structures used to support reporting and business analysis.

**Scripts**
- `Sql_Server/gold/ddl_goldRE.sql`
- `Sql_Server/gold/view_goldRE.sql1.sql`

The Gold layer supports the preparation of reporting-oriented datasets for business intelligence.

### Database Initialization

The database initialization script is:

`Sql_Server/init_database_RE.sql`

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

**Report file:** `PowerBI_Dashboard/Scm_project.pbix`

### Dashboard Preview

The `PowerBI_Dashboard/` folder contains the Power BI report and its dashboard screenshots.

The report can be opened using Microsoft Power BI Desktop.

## 📈 Excel Dashboard

Excel is used as an additional analysis and reporting tool in this project.

The Excel dashboard screenshots are available in the `Excel_Dashboard-screenshot/` folder.

The dashboards provide visual summaries of the analyzed business areas and complement the Power BI reporting solution.

## 💼 Business Questions

The project supports analysis of practical business questions, including:

### 📈 Sales & Profitability
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

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| SQL Server | Database and data architecture |
| T-SQL | Data processing and transformation |
| Microsoft Power BI | Interactive dashboards |
| DAX | Analytical calculations in Power BI |
| Power Query | Data preparation |
| Microsoft Excel | Dashboarding and supporting analysis |
| Draw.io | Architecture documentation, where applicable |
| GitHub | Project hosting and documentation |

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

## 🧠 Skills Demonstrated

**SQL & Data Engineering**
- SQL Server and T-SQL
- Database scripting
- Data transformation
- ETL workflow
- Layered data architecture

**Business Intelligence**
- Power BI dashboards
- Excel dashboard development
- Data visualization
- KPI reporting
- Business-oriented analysis

**Supply Chain Analytics**
- Sales and product analysis
- Customer performance
- Order fulfillment
- Shipping and delivery analysis
- Logistics performance

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

- GitHub: [Add your GitHub profile URL]
- LinkedIn: [Add your LinkedIn profile URL]

⭐ Thank you for exploring my project!
