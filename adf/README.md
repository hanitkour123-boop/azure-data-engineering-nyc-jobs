# Azure Data Factory

Azure Data Factory (ADF) was used as the data ingestion and orchestration layer of the project.

ADF was configured to retrieve the source dataset from GitHub using HTTPS and copy the raw data into Azure Data Lake Storage Gen2 for further processing.

## Responsibilities

- Configured the source connection to GitHub.
- Used HTTPS-based data ingestion.
- Configured the destination in ADLS Gen2.
- Created and executed the data ingestion pipeline.
- Validated successful data movement into the data lake.

## Data Flow

**GitHub → Azure Data Factory → ADLS Gen2**
