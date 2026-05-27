# Retail Finance & Sales Analytics using Snowflake + BI

## Project Overview
This project demonstrates an end-to-end cloud data warehousing solution using Snowflake and BI for retail finance and sales analytics.

The solution covers:
- Snowflake database setup
- Data ingestion using Stages & File Formats
- Incremental loading using Streams
- Automated ETL using Tasks
- Star schema data modeling
- KPI reporting and analytical SQL queries
- BI reporting integration

## Architecture
CSV Files -> Snowflake Stage -> RAW Schema -> Streams -> Tasks (Automated ETL) -> MART Schema -> BI Dashboards/Reports

## Tech Stack
- Snowflake
- SnowSQL
- Snowflake Streams
- Snowflake Tasks
- CSV Data Files

## Database Structure

### RAW Schema
Contains raw ingested data from source CSV files.
#### Tables:
- RAW_SALES
- DIM_CUSTOMER
- DIM_PRODUCT
- DIM_REGION
- DIM_DATE
#### Objects:
- CSV_FORMAT
- RETAIL_STAGE
- SALES_STREAM

### MART Schema
Contains transformed and reporting-ready data.
#### Tables:
- FACT_SALES
- DIM_CUSTOMER
- DIM_PRODUCT
- DIM_REGION
- DIM_DATE
#### Objects:
- LOAD_SALES_TASK

## Key Features
### Automated Data Loading
Implemented Snowflake Tasks for scheduled automated loading from Streams into Fact tables.

### Incremental Data Processing
Used Snowflake Streams for CDC (Change Data Capture) based incremental processing.

### Star Schema Design
Built dimensional model with:
- Fact Table
- Dimension Tables

### Business KPI Queries
Developed analytical SQL queries for:
- Monthly Revenue
- Top Products
- Customer Retention

## Business KPIs
- Total Revenue
- Profit Analysis
- Product Performance
- Customer Retention
- Monthly Sales Trends

## Snowflake Concepts Used
- Database & Schema Management
- Warehouses
- Internal Stages
- File Formats
- COPY INTO
- Streams
- Tasks
- Incremental Loading
- Data Mart Design

## Sample Workflow
1. Upload CSV files to Snowflake Stage
2. Load raw data into RAW schema
3. Track incremental changes using Streams
4. Automate ETL using Tasks
5. Populate MART tables
6. Connect Power BI for reporting

## Project Highlights
- End-to-end Snowflake implementation
- Real-world retail analytics use case
- Production-style ELT pipeline
- Automated scheduled data processing
