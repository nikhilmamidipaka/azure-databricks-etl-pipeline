# Azure Databricks ETL Project

## Project Overview
This project demonstrates an end-to-end ETL pipeline using **Azure Databricks**, designed for learning and interview preparation. The pipeline handles **incremental data ingestion**, **data transformation**, and **analytics-ready data modeling** using a medallion architecture (Bronze → Silver → Gold).  

Key objectives of this project:
- Learn **Spark Structured Streaming** for incremental data processing.
- Build **ETL pipelines** and workflows in Databricks.
- Implement **star schemas** and **slowly changing dimensions (SCD Types 1 & 2)**.
- Utilize **Delta Live Tables** for automated data management.
- Connect Databricks to **Power BI** for visualization.
- Apply **data governance** using Unity Catalog.

---

## Project Architecture

### Medallion Architecture
The data flows through three layers:
1. **Bronze Layer** – Raw data ingestion from GitHub and Azure using **Spark Structured Streaming**.
2. **Silver Layer** – Cleaned and processed data using **PySpark transformations**.
3. **Gold Layer** – Analytics-ready tables with **star schemas, dimension & fact tables**, and SCD implementation.

---

## Pipeline Overview

Below is the **visual representation of the Databricks job pipeline**:

[docs](End_To_End_Pipeline)

The above pipeline covers:
- Incremental data ingestion using **Autoloader**
- ETL workflows using **dynamic notebooks**
- Job scheduling and orchestration in **Databricks Jobs**
- Data storage in **Azure Data Lake** with Delta tables

---

## Job Configuration (JSON)
The Databricks job configuration is stored as a JSON file for version control:

`job_config/job_config.json`

This contains all the pipeline settings, cluster configuration, and notebook dependencies used in this project.

---

## Tech Stack
- **Azure Databricks** – Data processing and orchestration
- **PySpark** – ETL transformations
- **Delta Lake** – Transactional data storage
- **Azure Data Lake Storage** – Data storage
- **Power BI** – Visualization
- **Git & GitHub** – Version control

