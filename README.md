# SQL DAtawarehouse project

Welcome to the **Intelligent Supply Chain & Customer Analytics Platform**! This project demonstrates an end-to-end data warehousing and analytics solution built using **SQL Server, SQL, and Medallion Architecture**.

The platform integrates supply chain and retail datasets into a centralized analytical warehouse, transforming raw operational data into structured, analysis-ready information. It is designed to support data-driven decision-making across inventory management, sales, procurement, logistics, supplier performance, and customer analytics.

## 🏗️ Data Architecture

The project follows the **Medallion Architecture**, organized into three layers: Bronze, Silver, and Gold.

- **Bronze Layer:** Stores raw data ingested from CSV source files into SQL Server tables, preserving the original data for traceability and subsequent processing.
- **Silver Layer:** Cleans, standardizes, validates, and transforms raw data. This layer addresses data quality issues, corrects data types, handles missing or inconsistent values, and prepares reliable datasets for analytical modeling.
- **Gold Layer:** Organizes validated data into business-oriented analytical tables designed to support reporting, KPI calculations, and advanced SQL analytics.

📊 **Data Architecture Diagram:** [ADD LINK HERE]

## 📖 Project Overview

This project focuses on building a modern SQL-based data warehouse for supply chain and customer analytics.

The major components include:

- **Data Architecture:** Designing a scalable, layered data warehouse using Bronze, Silver, and Gold schemas.
- **Data Ingestion:** Loading multiple CSV datasets into SQL Server using appropriate data-loading techniques.
- **ETL Pipelines:** Extracting, cleaning, transforming, and integrating data across different processing layers.
- **Data Quality:** Identifying and resolving data type mismatches, inconsistent values, missing data, and data-loading errors.
- **Data Modeling:** Structuring operational data into analytical tables that support efficient queries and reporting.
- **Supply Chain Analytics:** Analyzing orders, inventory, procurement, shipments, warehouse operations, suppliers, and retail sales.
- **Customer & Sales Analytics:** Exploring sales performance, order patterns, and customer-related business metrics.
- **Documentation & Testing:** Maintaining technical documentation and validating data quality throughout the pipeline.

## 🎯 Project Objectives

The primary objective is to transform fragmented operational datasets into a unified analytical platform that enables better business decisions.

Key objectives include:

- Consolidate supply chain and retail data into a centralized warehouse.
- Establish a repeatable process for data ingestion and transformation.
- Improve data consistency, reliability, and usability.
- Enable analysis of inventory movement, shipment performance, supplier activity, and sales trends.
- Develop analytical SQL queries to identify business patterns, operational inefficiencies, and potential improvement opportunities.
- Build a foundation for future interactive dashboards and advanced analytics.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| SQL Server | Database and data warehouse |
| SQL / T-SQL | Data ingestion, transformation, validation, and analytics |
| CSV | Source data format |
| Medallion Architecture | Bronze, Silver, and Gold data processing layers |
| Dimensional Modeling | Organizing data for analytical queries |
| Git & GitHub | Version control and project documentation |
| Power BI | Visualization and dashboarding, where implemented |
| Draw.io | Data architecture and workflow diagrams |

## 📊 Supply Chain Dataset

The project uses multiple datasets representing different stages of supply chain operations.

The source tables include:

- `customer_orders` — Customer order information.
- `inventory_daily_snapshot` — Daily inventory levels and stock positions.
- `purchase_order` — Procurement and purchase order records.
- `retailsales` — Retail sales transactions.
- `routes_carrier` — Carrier and route information.
- `shipment` — Shipment records and logistics information.
- `shipment_to_store` — Shipment movements to stores.
- `sku_master` — Product and SKU master data.
- `store_master` — Store information.
- `suppliers` — Supplier details.
- `warehouse` — Warehouse master data.
- `warehouse_inbound` — Inbound warehouse movements.
- `warehouse_outbound` — Outbound warehouse movements.

**Dataset Source:** [ADD DATASET LINK HERE]

*Note: The final analytical model and the specific KPIs depend on the transformations and reporting features implemented in the repository.*

## 🚀 Project Requirements

### 1. Data Engineering — Building the Data Warehouse

**Objective:** Develop a SQL Server data warehouse that integrates operational supply chain and retail data to support reliable analytical reporting.

**Specifications**

- **Data Sources:** Import multiple CSV datasets representing customers, orders, inventory, procurement, sales, suppliers, shipments, stores, and warehouse operations.
- **Data Ingestion:** Load source data into the Bronze layer using SQL Server.
- **Data Quality:** Identify and resolve inconsistencies, missing values, incorrect data types, and other data quality issues during transformation.
- **Data Transformation:** Clean, standardize, validate, and convert data in the Silver layer.
- **Data Integration:** Combine related datasets into a consistent analytical structure.
- **Data Modeling:** Design business-oriented Gold-layer tables suitable for reporting and analysis.
- **Documentation:** Document the architecture, data flow, transformation logic, table structures, and analytical definitions.

### 2. Data Analytics — Extracting Business Insights

**Objective:** Use SQL-based analytics to evaluate operational performance and uncover actionable business insights.

The intended analytical areas include:

- **Sales Analytics:** Sales trends, order volumes, product performance, and revenue patterns.
- **Inventory Analytics:** Stock availability, inventory movement, and potential stock imbalances.
- **Procurement Analytics:** Purchase orders, supplier activity, and purchasing patterns.
- **Logistics Analytics:** Shipment volumes, carrier performance, and shipment-to-store movements.
- **Warehouse Analytics:** Inbound and outbound operations and warehouse activity.
- **Customer Analytics:** Customer purchasing patterns and order behavior.

The insights generated from these analyses can help identify operational bottlenecks, improve visibility across the supply chain, and support evidence-based decision-making.

## 📂 Repository Structure

```text
intelligent-supply-chain-analytics/
│
├── datasets/
│   ├── customer_orders.csv
│   ├── inventory_daily_snapshot.csv
│   ├── purchase_order.csv
│   ├── retailsales.csv
│   ├── routes_carrier.csv
│   ├── shipment.csv
│   ├── shipment_to_store.csv
│   ├── sku_master.csv
│   ├── store_master.csv
│   ├── suppliers.csv
│   ├── warehouse.csv
│   ├── warehouse_inbound.csv
│   └── warehouse_outbound.csv
│
├── docs/
│   ├── data_architecture.png
│   ├── data_flow.png
│   ├── data_model.png
│   ├── data_catalog.md
│   └── project_requirements.md
│
├── scripts/
│   ├── init_database.sql
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── tests/
│   └── data_quality_checks.sql
│
├── reports/
│   └── analytical_queries.sql
│
├── README.md
└── .gitignore
```

*The structure above is a proposed documentation layout. Adjust the filenames and folders to match the scripts and files actually present in your repository.*

## 📈 Expected Deliverables

- SQL Server database with Bronze, Silver, and Gold processing layers.
- SQL scripts for data ingestion and transformation.
- Cleaned and standardized datasets.
- Analytical tables and data models.
- SQL queries for supply chain and customer analytics.
- Data quality validation checks.
- Architecture and data flow documentation.
- Business dashboards, if implemented.

## 📚 Project Resources

- **GitHub Repository:** [[ADD GITHUB REPOSITORY LINK](https://github.com/Nandu-yadav/SQL_DataWareHouse_Project_1/edit/main/README.md)]
- **Dataset:** [ADD DATASET LINK]
- **Data Architecture Diagram:** [ADD DIAGRAM LINK]
- **Data Model:** [ADD DATA MODEL LINK]
- **Project Documentation:** [[ADD DOCUMENTATION LINK](https://app.notion.com/p/SQL-Data-Warehouse-Project-Plan-3bfb8974d3b582f6bd570166dbc25ab4?source=copy_link)]


## 👨‍💻 About This Project

This project demonstrates practical skills in SQL development, data engineering, ETL processes, data quality management, data modeling, and business analytics.

It also provides a foundation for extending traditional data warehousing workflows with business intelligence tools and, in future iterations, predictive analytics and AI-driven supply chain optimization.

**Built with:** SQL Server | T-SQL | Medallion Architecture | Supply Chain Analytics

**Author:** [YOUR NAME]

- LinkedIn: [ADD LINK]
- GitHub: [ADD LINK]
