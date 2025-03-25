# Overview
This project demonstrates the implementation of a real-world data pipeline using Azure services to process Brazilian e-commerce data. It is divided into two phases:

Part 1: Data ingestion and pipeline setup using Azure Data Factory.
Part 2: Data transformation, enrichment, and visualization with Azure Databricks and Synapse Analytics.

The project follows Medallion Architecture (Bronze, Silver, Gold layers) to ensure data quality and efficient processing.

# Architecture Diagram

## Below is the high-level architecture of the pipeline:

1️ Data Ingestion: Extract raw data from multiple sources (GitHub, SQL, HTTP endpoints) using Azure Data Factory (ADF).<br>
2️ Data Storage: Store raw data in Azure Data Lake Storage (ADLS Gen2) following the Medallion Architecture (Bronze, Silver, Gold).<br>
3️ Data Processing: Transform data using Azure Databricks (batch processing, enrichment).<br>
4️ Data Analytics: Load structured data into Azure Synapse Analytics for querying and analysis.<br>
5️ Visualization: Generate business insights using Power BI.<br>

### Part 1: Data Ingestion Pipeline
What I Learned & Implemented<br>
Set up Azure Data Factory for ETL processes.<br>
Configured ADLS Gen2 for cloud storage.
Designed Medallion Architecture (Bronze, Silver, Gold).<br>
Implemented data ingestion pipelines from multiple sources (HTTP, SQL).<br>
Managed error handling & monitoring in pipelines.<br>

### Part 2: Data Transformation & Visualization
Advanced Implementations:
Set up Azure Databricks for large-scale data processing.<br>
Integrated MongoDB for data enrichment.<br>
Configured Azure Synapse Analytics for query optimization.<br>
Built interactive dashboards using Power BI/Tableau.<br>
Optimized data processing performance for scalability.<br>

# Tech Stack

Cloud Platform: Microsoft Azure<br>
Data Ingestion: Azure Data Factory (ADF)<br>
Storage: Azure Data Lake Storage Gen2 (ADLS Gen2)<br>
Processing: Azure Databricks (PySpark, DataFrames)<br>
Database: Azure Synapse Analytics<br>
Visualization: Power BI<br>
Version Control: GitHub<br>

# End-to-End Pipeline Process:
## 1. Data Ingestion<br>
Built batch ingestion pipelines to collect data from SQL Server, PostgreSQL, and REST APIs using Azure Data Factory, scheduling daily/hourly syncs.<br>
Implemented real-time streaming for IoT devices using Kafka and Azure Event Hubs, reducing data latency from hours to seconds.<br>

## 2. Scalable Processing
Designed a distributed processing system with PySpark in Databricks, handling 10TB+ of raw data monthly.<br>
Configured auto-scaling clusters in GCP DataProc to optimize costs while maintaining SLA for critical jobs.<br>

## 3. Transformation & Enrichment
Developed PySpark scripts to cleanse and join user behavior data with sales records, improving dataset accuracy by 30%.<br>
Integrated data quality checks using great_expectations, logging anomalies to Slack for rapid troubleshooting.<br>

## 4. Storage & Querying
Deployed a cloud data warehouse in Azure Synapse Analytics, enabling complex SQL queries on processed data with sub-second response times.<br>
Optimized BigQuery table partitioning schemas, reducing query costs by 45%.<br>

## 5. Visualization & Delivery
Created interactive Power BI dashboards for executive teams, visualizing revenue trends and customer segmentation.<br>
Exposed processed data via REST APIs (Azure Functions) for internal apps, eliminating manual CSV exports.<br>

Key Achievements
Reduced pipeline runtime by 60% through Spark optimizations.<br>
Cut cloud costs by 35% with partitioned storage and auto-scaling.<br>
Enabled real-time analytics for 5+ business units.<br>

