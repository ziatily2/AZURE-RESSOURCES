# 🚀 Azure Data Engineering Pipeline

## 📌 Project Overview
This project demonstrates an **end-to-end data pipeline** leveraging **Azure** services for data ingestion, transformation, and storage. It follows best practices for **incremental data processing** and **dimensional modeling** to build a scalable data architecture.

## 🔰 Tech Stack
✅ **Azure Data Factory (ADF)** - Orchestration & Data Ingestion  
✅ **Databricks with Unity Catalog** - Data Transformation & Governance  
✅ **Apache Spark** - Distributed Data Processing  
✅ **Delta Lake** - Optimized Data Storage & Versioning  
✅ **Azure Data Lake** - Scalable Storage Layer  
✅ **Azure SQL Database** - Source System  
✅ **GitHub** - Version Control & Collaboration  

## 🔰 Architecture
✅ **Medallion Architecture** - Implementing **Bronze, Silver, Gold layers** for better data management  

## 🔰 Complex Real-Time Scenarios
✅ **Incremental Data Loading** - Handling new data efficiently  
✅ **Dimensional Data Modeling** - Structuring data for analytics  
✅ **STAR Schema Design** - Optimizing for performance  
✅ **Slowly Changing Dimensions (SCDs)** - Managing historical data changes  

## 🔄 Pipeline Workflow
1️⃣ **Data Ingestion**: Extracting data from **Azure SQL Database** using **ADF Copy Activity**
2️⃣ **Bronze Layer (Raw Storage)**: Storing extracted data in **Azure Data Lake Gen2**
3️⃣ **Incremental Processing**: Applying a **Watermark Strategy** to load only new data
4️⃣ **Silver Layer (Cleansed Data)**: Processing and cleaning data with **Databricks Notebooks**
5️⃣ **Gold Layer (Analytics Ready Data)**: Creating structured tables such as **Dim_branch, Dim_date, Dim_model, Fact_sales**
6️⃣ **Serving Layer**: Storing transformed data in **Delta Lake** for optimized querying


