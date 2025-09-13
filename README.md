
# Week-1 Cleaned Data (Data Engineering Internship)

This repository contains the **cleaned and partitioned outputs** for Week-1 of the StoryPoints Data Engineering Internship.

## 📂 Files

- `clickstream_ingest_2025-09-13.zip`  
  → Contains cleaned clickstream Parquet shards under  
  `clickstream/ingest_date=2025-09-13/part_*.parquet`

- `transactions_ingest_2025-09-13.zip`  
  → Contains cleaned transactions Parquet shards under  
  `transactions/ingest_date=2025-09-13/part_*.parquet`

## 🛠 Process Summary
- Source CSVs were cleaned:  
  - Normalized headers  
  - Converted timestamps to UTC  
  - Removed duplicates  
- Data written in **Parquet format**, partitioned by ingest date (`2025-09-13`).  
- Final row counts:  
  - **Clickstream:** 200,000 rows  
  - **Transactions:** 100,000 rows  

## 🚫 Notes
- Currency enrichment (USD conversion) was skipped — no rates JSON available.  
- Raw CSV files are excluded; only curated outputs are provided.  
