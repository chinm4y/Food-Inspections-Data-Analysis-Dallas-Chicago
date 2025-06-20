# Food Inspections Data Analysis – Dallas & Chicago

This project showcases a robust, end-to-end data pipeline to clean, transform, and analyze large public datasets from Dallas and Chicago food inspection systems. The pipeline integrates modern data engineering tools like **Talend**, **Alteryx**, and **Power BI**, and stores data in **Azure Data Lake Storage (ADLS)** for scalability and performance.

## Objective

To standardize and analyze food inspection records across cities, identify critical violations and trends, and build visual insights that can support public health decision-making and regulatory enforcement.

## Key Outcomes

- Built a unified data model across two distinct city datasets
- Detected data quality issues, outliers, and missing values
- Automated ETL workflows for ingestion, cleansing, and transformation
- Enabled dashboard-driven insights for business stakeholders

## Enterprise Tech Stack

- **Talend** – Data ingestion and schema mapping from city portals
- **Alteryx** – Data wrangling, transformation logic, and output formatting
- **Power BI** – Visualization of key KPIs, violation trends, and inspection outcomes
- **Azure Data Lake Storage (ADLS)** – Centralized data lake for raw and curated zones
- **Python + pandas** – Supplemental cleaning and profiling in Jupyter
- **YData Profiling / pandas-profiling** – For automated EDA
- **SQL** – For rule-based data validation and tabular aggregation

## Pipeline Overview

1. **Ingestion**  
   - Downloaded city-specific CSV datasets from public portals
   - Talend jobs extract files and map attributes to a unified schema
   - Uploaded data to ADLS raw zone

2. **Transformation**  
   - Alteryx workflows handle:
     - Date normalization, null handling
     - Violation flagging and deduplication
     - City-wise scoring and outcome standardization
   - Output written to ADLS curated zone and SQL staging layer

3. **Profiling & QA**  
   - Used Python (`pandas`, `ydata-profiling`) to:
     - Validate schema conformance
     - Profile high-cardinality fields
     - Identify outliers and common inspection violations

4. **Visualization**  
   - Power BI dashboard to show:
     - Pass/Fail rates by city and year
     - Top recurring violation categories
     - Inspection heatmaps (optional with coordinates)
     - Monthly inspection volume trends

## Skills Demonstrated

- ETL pipeline orchestration with Talend and Alteryx
- Data modeling across multi-source schemas
- Azure Data Lake architecture for raw → curated layers
- Python-based data validation and profiling
- BI dashboarding with drill-down and filters (Power BI)
- Data quality analysis and rule-based transformations
