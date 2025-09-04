# csv-to-azure-datalake-etl

# CSV to Azure Data Lake ETL (Bronze → Silver)

## 🎯 Goal
Load raw CSV files into Azure Data Lake (Bronze), transform with Azure Data Factory, and store optimized Parquet files in Silver zone.

## 🏗 Architecture
- Azure Data Lake Gen2
  - Bronze (raw CSVs)
  - Silver (curated Parquet)
- Azure Data Factory
  - Pipeline: Copy activity from Bronze CSV → Silver Parquet

## ⚙️ Steps
1. Created Storage Account with Bronze & Silver containers.
2. Uploaded raw CSV into Bronze.
3. Built ADF pipeline:
   - Source: Bronze CSV
   - Sink: Silver Parquet
4. Deployed pipeline → CSV converted to Parquet.

## 📂 Repo Structure
/pipeline/pipeline.json # ADF pipeline export
/screenshots/ # Setup & pipeline images
/data/ # Sample CSV



## ✅ Outcome
- CSV successfully transformed into Parquet.
- Data ready for analytics (Power BI, Spark, ML).
