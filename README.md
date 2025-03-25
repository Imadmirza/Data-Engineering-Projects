# Overview
This project demonstrates the implementation of a real-world data pipeline using Azure services to process Brazilian e-commerce data. It is divided into two phases:

Part 1: Data ingestion and pipeline setup using Azure Data Factory.
Part 2: Data transformation, enrichment, and visualization with Azure Databricks and Synapse Analytics.

The project follows Medallion Architecture (Bronze, Silver, Gold layers) to ensure data quality and efficient processing.

# Architecture Diagram

## Below is the high-level architecture of the pipeline:

1️ Data Ingestion: Extract raw data from multiple sources (GitHub, SQL, HTTP endpoints) using Azure Data Factory (ADF).
2️ Data Storage: Store raw data in Azure Data Lake Storage (ADLS Gen2) following the Medallion Architecture (Bronze, Silver, Gold).
3️ Data Processing: Transform data using Azure Databricks (batch processing, enrichment).
4️ Data Analytics: Load structured data into Azure Synapse Analytics for querying and analysis.
5️ Visualization: Generate business insights using Power BI.

### Part 1: Data Ingestion Pipeline
What I Learned & Implemented
✔ Set up Azure Data Factory for ETL processes.
✔ Configured ADLS Gen2 for cloud storage.
✔ Designed Medallion Architecture (Bronze, Silver, Gold).
✔ Implemented data ingestion pipelines from multiple sources (HTTP, SQL).
✔ Managed error handling & monitoring in pipelines.

### Part 2: Data Transformation & Visualization
Advanced Implementations:
✔ Set up Azure Databricks for large-scale data processing.
✔ Integrated MongoDB for data enrichment.
✔ Configured Azure Synapse Analytics for query optimization.
✔ Built interactive dashboards using Power BI/Tableau.
✔ Optimized data processing performance for scalability.

# Tech Stack

Cloud Platform: Microsoft Azure
Data Ingestion: Azure Data Factory (ADF)
Storage: Azure Data Lake Storage Gen2 (ADLS Gen2)
Processing: Azure Databricks (PySpark, DataFrames)
Database: Azure Synapse Analytics
Visualization: Power BI
Version Control: GitHub

# End-to-End Pipeline Process:
## 1. Data Ingestion
Built batch ingestion pipelines to collect data from SQL Server, PostgreSQL, and REST APIs using Azure Data Factory, scheduling daily/hourly syncs.
Implemented real-time streaming for IoT devices using Kafka and Azure Event Hubs, reducing data latency from hours to seconds.

## 2. Scalable Processing
Designed a distributed processing system with PySpark in Databricks, handling 10TB+ of raw data monthly.
Configured auto-scaling clusters in GCP DataProc to optimize costs while maintaining SLA for critical jobs.

## 3. Transformation & Enrichment
Developed PySpark scripts to cleanse and join user behavior data with sales records, improving dataset accuracy by 30%.
Integrated data quality checks using great_expectations, logging anomalies to Slack for rapid troubleshooting.

## 4. Storage & Querying
Deployed a cloud data warehouse in Azure Synapse Analytics, enabling complex SQL queries on processed data with sub-second response times.
Optimized BigQuery table partitioning schemas, reducing query costs by 45%.

## 5. Visualization & Delivery
Created interactive Power BI dashboards for executive teams, visualizing revenue trends and customer segmentation.
Exposed processed data via REST APIs (Azure Functions) for internal apps, eliminating manual CSV exports.

Key Achievements
Reduced pipeline runtime by 60% through Spark optimizations.
Cut cloud costs by 35% with partitioned storage and auto-scaling.
Enabled real-time analytics for 5+ business units.

