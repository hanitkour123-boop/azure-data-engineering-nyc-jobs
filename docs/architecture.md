# Azure Data Engineering Pipeline Architecture

## Overview

This project implements an end-to-end data engineering pipeline using Microsoft Azure services. The solution covers data ingestion, storage, transformation, analytics, and visualization.

## Architecture Flow

**GitHub → Azure Data Factory → ADLS Gen2 → Azure Databricks → ADLS Gen2 → Azure Synapse Analytics → Power BI**

## Components

### 1. GitHub

GitHub was used as the external source of the raw dataset.

### 2. Azure Data Factory

Azure Data Factory was used to ingest the source data from GitHub using HTTPS and transfer the raw data to Azure Data Lake Storage Gen2.

### 3. Azure Data Lake Storage Gen2

ADLS Gen2 was used as the central storage layer for the pipeline. It stored both the raw data received from the source and the processed data generated after transformation.

### 4. Azure Databricks

Azure Databricks was used as the data processing layer. PySpark was used to clean, transform, and enrich the raw dataset.

### 5. Azure Synapse Analytics

Azure Synapse Analytics was used to query and analyze the transformed data and provide an analytical layer for downstream consumption.

### 6. Power BI

Power BI was used as the visualization layer to present insights from the processed data.

## Data Flow

1. Raw data is obtained from GitHub.
2. Azure Data Factory ingests the data.
3. Raw data is stored in ADLS Gen2.
4. Azure Databricks reads the raw data.
5. PySpark transformations are applied.
6. Processed data is stored back in ADLS Gen2.
7. Azure Synapse Analytics is used for analytical querying.
8. Power BI consumes the analytical data for visualization.

## Technologies

* Microsoft Azure
* Azure Data Factory
* Azure Data Lake Storage Gen2
* Azure Databricks
* Apache Spark
* PySpark
* Azure Synapse Analytics
* Power BI
* GitHub

