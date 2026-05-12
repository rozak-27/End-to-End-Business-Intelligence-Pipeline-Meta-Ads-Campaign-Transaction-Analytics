# End-to-End-Business-Intelligence-Pipeline-Meta-Ads-Campaign-Transaction-Analytics

 # Project Description
This project demonstrates a complete Business Intelligence pipeline built to analyze Meta (Facebook & Instagram) ad campaign performance and sales transactions. Starting from raw CSV data, the pipeline covers database design, ETL processing, multidimensional OLAP modeling, and interactive dashboard visualization — simulating a real-world enterprise data engineering workflow.
The dataset includes 379,954 ad events and 2,031 transactions across a 3-month campaign period (May–August 2025), covering user demographics, ad formats, platforms, products, and payment behavior.

What Was Built
Database Architecture — Designed a Galaxy Schema data warehouse in SQL Server with 2 fact tables (fact_transactions, ad_events) and 6 dimension tables (dim_date, dim_user, dim_product, dim_payment, ads, campaigns). Defined all primary keys, foreign keys, and relationships to support analytical queries.
ETL Pipeline
— Built a fully automated ETL package in SSIS with 6 Data Flow Tasks, each handling extraction from CSV files, data type conversion, surrogate key generation via C# Script Component, and loading into SQL Server. Implemented Precedence Constraints to ensure dimensions load before fact tables.
OLAP Cube
— Developed a Multidimensional OLAP cube in SSAS with 2 Measure Groups and 5 dimensions. Wrote MDX calculated measures including CTR, CVR, Revenue per Campaign, Conversion Value, Total Users, Peak Day, and Best CTR Format. Configured Dimension Usage following Galaxy Schema logic where shared dimensions connect to both fact tables.
Interactive Dashboard
— Connected Power BI via Live Connection to the SSAS cube and built a 3-page interactive dashboard covering ad performance KPIs, OLAP drill-down analysis, and user demographic profiling. All pages support cross-filtering, slicers, and conditional formatting heatmaps.

Key Findings

CTR of 11.76% with Video ads achieving the highest CTR at 11.9%
Friday afternoons identified as peak engagement time across all platforms
Facebook outperformed Instagram in total purchases (1,264 vs 673)
Dominant user demographic: Female, age 25–34, from United States
Total revenue of $8.59M with an average cost per purchase of $2.01K
Top interest category: Fitness, top sales channel: Mobile App


Skills Demonstrated
Data Warehousing ETL Pipeline OLAP Cube Design MDX SQL C# Data Modeling Galaxy Schema Business Intelligence KPI Development Dashboard Design SSIS SSAS Power BI SQL Server
