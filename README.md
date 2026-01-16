# databricks_automated_lakeflow_pipeline_medallion_project
This repository contains an end-to-end Databricks Lakehouse analytics implementation, built using Delta Lake, Unity Catalog, SQL, and Python notebooks, following a Bronze → Silver → Gold architecture.

The project focuses on transforming raw transactional data into analytics-ready datasets, including aggregated revenue metrics and ranked customer insights by region, optimized for downstream BI and reporting use cases.

🏗️ Architecture Overview

The project follows a modern Lakehouse design pattern:

Source Data
   ↓
Bronze Layer (Raw ingestion)
   ↓
Silver Layer (Cleaned & transformed)
   ↓
Gold Layer (Aggregated & business-ready)


Bronze: Raw ingestion from source systems

Silver: Cleansed, standardized, and enriched datasets

Gold: Curated analytical tables and materialized views

🧱 Technology Stack

Databricks

Delta Lake

Unity Catalog

SQL (Window functions, Aggregations)

Python (Databricks notebooks)

GitHub (Version control)

📈 Key Features
🔹 Revenue Analytics by Region

Aggregates customer-level revenue

Ranks customers within each region

Identifies Top-N revenue contributors

Uses window functions (RANK() OVER) for analytical ranking

🔹 Materialized Views

Pre-computed and stored for fast querying

Optimized for BI dashboards and ad-hoc analysis

Designed for repeatable, production-grade analytics

🔹 Clean Separation of Concerns

Business logic lives in Silver

Aggregations and KPIs live in Gold

All transformations are code-driven and reproducible

🧠 Example Use Case

One of the core outputs is a Gold-layer materialized view that provides:

Top 5 revenue-generating customers in each region, ranked by total revenue.

This enables:

Regional performance analysis

Customer contribution insights

Executive-level reporting

Dashboard:

<img width="1723" height="612" alt="image" src="https://github.com/user-attachments/assets/9f0000f4-d1f4-425b-b6cd-837ebadfd72c" />

