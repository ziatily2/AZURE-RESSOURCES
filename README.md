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

## 📂 Repository Structure
```
📦 AZURE-RESSOURCES
 ┣ 📂 notebooks
 ┃ ┣ 📜 silver_notebook.ipynb  # Data transformation logic
 ┃ ┣ 📜 gold_dim_date.ipynb    # Dimensional modeling (Date dimension)
 ┃ ┣ 📜 gold_fact_sales.ipynb  # Fact table processing (Sales data)
 ┣ 📂 pipelines
 ┃ ┣ 📜 incremental_data_pipeline.json  # ADF Pipeline Configuration
 ┣ 📜 README.md  # Project Documentation
```

## 📷 Project Screenshots
✅ **Azure Data Factory Pipeline** - Incremental Data Loading & Orchestration
✅ **Databricks Job Execution** - ETL Pipeline Execution & Dimensional Modeling

## 🚀 Getting Started
### 1️⃣ Clone Repository
```bash
git clone https://github.com/ziatily2/AZURE-RESSOURCES.git
```
### 2️⃣ Deploy Azure Data Factory Pipeline
- Import **incremental_data_pipeline.json** into Azure Data Factory.
- Configure **SQL Database** and **Data Lake Gen2** connections.

### 3️⃣ Deploy Databricks Notebooks
- Upload notebooks to **Databricks Workspace**.
- Schedule jobs using **Databricks Workflows**.

## 💡 Future Enhancements
- **Integrate Advanced Unity Catalog Features** for enhanced data governance and access control.
- **Optimize Databricks Workflows** for better performance and cost efficiency.
- **Implement CI/CD Pipelines** using GitHub Actions for automation.

## 🔗 Connect with Me
I’d love to collaborate and hear your feedback! 🚀
