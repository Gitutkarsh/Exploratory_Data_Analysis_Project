# Exploratory_Data_Analysis_Project
# SQL Explorational Data Analysis & Business Performance Analytics

## 📌 Project Overview
This repository contains a modular, production-grade Exploratory Data Analysis (EDA) pipeline executed inside SQL Server Management Studio (SSMS). The pipeline processes transactional operational records across data warehouse layers to extract key business metrics, benchmark performances, and prepare structured datasets for executive reporting.

## 🛠️ Tech Stack & Tools
* **Database Engine:** Microsoft SQL Server
* **Interface IDE:** SQL Server Management Studio (SSMS)
* **Language Layer:** T-SQL (Subqueries, Joins, Window Functions, Set Operators)

## 📂 Repository Structure & Workflow Pipeline
All database operations are divided into structural modules located inside the `/scripts` directory:

* **`00_init_database.sql`**: Database instantiation, schema building (`gold` schema), and bulk data loading protocols.
* **`02_dimensions_exploration.sql`**: Initial profile mapping and unique country/category data audits.
* **`03_date_range_exploration.sql`**: Temporal boundary tracking and age demographic evaluations.
* **`04_measures_exploration.sql`**: Consolidated KPI metrics ledger mapping total revenue, order count, and product densities using `UNION ALL`.
* **`05_magnitude_analysis.sql`**: Multi-dimensional aggregations evaluating revenue distribution across product catalogs and customer segments.
* **`06_ranking_analysis.sql`**: Advanced performance benchmarking utilizing analytical window functions (`RANK() OVER`) to capture high-value assets and customer churn indicators.

## 🚀 Key Database Engineering Practices Applied
* **Relational Accuracy:** Implemented explicit `LEFT JOIN` structures to safely link Fact data (`gold.fact_sales`) with Dimensional attributes (`gold.dim_products`, `gold.dim_customers`) without data leakage.
* **Analytical Isolation:** Leveraged inline subqueries paired with ranking window configurations to execute complex business rule filters.
* **Data Aggregation:** Handled extensive group-by operations and multi-line datasets using unified reporting sets (`UNION ALL`).
