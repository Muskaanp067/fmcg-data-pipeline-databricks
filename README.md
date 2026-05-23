# FMCG Data Pipeline — Databricks

End-to-end Data Engineering project built on Databricks for an 
FMCG client with a parent-child company data model.

## What This Project Does
Ingests and processes sales, customer, product, and pricing data 
from two companies (parent + child) into a unified data warehouse 
using full load and incremental load strategies.

## Architecture
![Project Architecture](resources/project_architecture.png)

## Tech Stack
- **Platform:** Databricks (PySpark)
- **Language:** Python, SQL
- **Data:** CSV ingestion → Delta tables
- **Load Strategy:** Full load + Incremental load
- **Dashboarding:** PDF dashboard with denormalized query layer

## Project Structure
1_codes/
1_setup/          → Catalog setup, utilities, date table
2_dimension_data_processing/ → Customers, Products, Pricing
3_fact_data_processing/      → Full load & Incremental load
2_dashboarding/     → Final dashboard + SQL query
resources/          → Architecture diagram


## Key Concepts Covered
- Medallion-style data processing
- Incremental load with partition-based ingestion
- Dimension and fact table separation
- Multi-source data unification (parent + child company)
