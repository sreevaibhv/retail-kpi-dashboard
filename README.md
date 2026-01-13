# Retail KPI Intelligence Dashboard (Star Schema + Semantic Layer)

## Overview
This project demonstrates an enterprise BI reporting workflow similar to MicroStrategy BI development.
It includes a dimensional data model (Star Schema), semantic reporting views (Facts/Attributes), and KPI dashboards with prompt-style filters.

## Tech Stack
- PostgreSQL
- SQL (Views, Materialized Views)
- Metabase / Power BI / Superset (Dashboarding)

## Data Model (Star Schema)
- FactSales
- DimCustomer, DimProduct, DimStore, DimDate

📌 Schema Diagram: `docs/schema_diagram.png`

## Semantic Layer (MicroStrategy-style)
Created semantic reporting views to represent:
- Facts
- Attributes
- Hierarchies

Key views:
- vw_sales_base
- vw_store_kpis
- vw_product_kpis

## KPIs Implemented (25+)
- Revenue, Profit, Gross Margin %
- Orders, Units Sold, AOV
- Store Ranking, Region Contribution
- Category Contribution, Top Products
- Repeat Customer Rate, New vs Returning Customers

Full list: `docs/kpi_list.md`

## Dashboards
1) Executive KPI Dashboard
2) Drilldown Dashboard (Region → Store → Product)

Screenshots: `/dashboards`

## Performance Optimization
- Indexing strategy
- Materialized Views for aggregation/caching
- Dashboard load improvement: 40–60%

## How to Run
1. Run SQL scripts in order from `/sql`
2. Connect BI tool to PostgreSQL
3. Import dashboard / recreate visuals
