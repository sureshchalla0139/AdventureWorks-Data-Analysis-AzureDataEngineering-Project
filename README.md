# Adventure Works | Azure Data Engineering Project

## Introduction
This project demonstrates the **end-to-end data pipeline** for processing and analyzing **AdventureWorks Sales data** using the **Azure Cloud** ecosystem. It follows the **Medallion Architecture (Bronze, Silver, Gold)** to ensure **data quality, governance, and performance**.

The project involves:
- Extracting data from **On-Prem SQL Server** using **Azure Data Factory**.
- Storing raw data in **Azure Data Lake Storage Gen2 (Bronze Layer)**.
- Performing **ETL transformations using PySpark in Azure Databricks**.
- Storing cleaned and aggregated data in **Silver and Gold Layers**.
- Loading data into **Azure Synapse Analytics (Serverless SQL Pool)**.
- Visualizing insights in **Power BI**.
- Implementing **Role-Based Access Control (RBAC) using Microsoft Entra ID**.
- Managing secrets securely with **Azure Key Vault**.
- Using **GitHub for version control**.

---

## Project Architecture
This project follows the **Medallion Architecture**:
1. **Bronze Layer**: Stores raw, unprocessed data as extracted from the source.
2. **Silver Layer**: Cleans and transforms data for business analysis.
3. **Gold Layer**: Provides aggregated and business-ready data for reporting.

The architecture ensures **scalability, data governance, and optimized query performance**.

### 🖼️ High-Level Architecture Diagram
Below is the **high-level architecture** of the project:

![Project Architecture](Project%files/AdventureWorksArchitecture.png)

### 🔑 Key Components
- **Data Ingestion**: Azure Data Factory extracts data from **On-Prem SQL Server**.
- **Storage**: Azure Data Lake Gen2 with **Bronze, Silver, and Gold layers**.
- **Processing & Transformation**: Azure Databricks (PySpark-based ETL).
- **Analytics**: Azure Synapse Serverless SQL Pool.
- **Visualization**: Power BI.
- **Security & Access Control**: Microsoft Entra ID for RBAC, Azure Key Vault for secrets.
- **Code Management**: GitHub repository.

---

## 🔄 Project Workflow
1. **Extract & Load (EL)**  
   - Azure Data Factory fetches **Sales schema** from **SQL Server**.  
   - Stores raw data in **Azure Data Lake (Bronze Layer)**.

2. **Transformation (ETL in Databricks)**  
   - PySpark transformations applied:
     - Schema enforcement, deduplication, standardization.
     - Handling missing data, type conversions.
     - Aggregations & business logic.
   - Processed data stored in **Silver Layer**.

3. **Aggregation & Business Insights (Gold Layer)**  
   - Joins, aggregations, and business rule applications.  
   - Optimized data stored in **Gold Layer**.

4. **Loading into Azure Synapse Analytics**  
   - Gold Layer data is **queried using Serverless SQL Pool**.

5. **Data Visualization in Power BI**  
   - Power BI connects to **Azure Synapse for interactive dashboards**.

6. **Security & Governance**  
   - **Azure Active Directory (Entra ID)** for **Role-Based Access Control (RBAC)**.  
   - **Azure Key Vault** for **secure credential storage**.  
   - **GitHub** for **code version control**.

---

## ⚙️ Technologies Used
| Component             | Technology Used                     |
|----------------------|----------------------------------|
| **Data Ingestion**   | Azure Data Factory (ADF)         |
| **Storage**         | Azure Data Lake Storage Gen2     |
| **Processing**      | Azure Databricks (PySpark)       |
| **Analytics**       | Azure Synapse Analytics (SQL)   |
| **Visualization**   | Power BI                         |
| **Security**       | Azure Active Directory (RBAC)   |
| **Secret Management** | Azure Key Vault                 |
| **Code Repository** | GitHub                           |

---

## ✨ Key Features
✅ **End-to-End Cloud-Based Data Pipeline** using Azure.  
✅ **Multi-Hop Data Architecture** (Bronze, Silver, Gold).  
✅ **PySpark-Based Transformations** in Azure Databricks.  
✅ **Optimized Data Querying** with Azure Synapse Analytics.  
✅ **Interactive Dashboards** in Power BI.  
✅ **Enterprise-Grade Security** with Entra ID & Azure Key Vault.  
✅ **Scalable & Automated ETL Workflows** using Azure Data Factory.  

---

## 📂 Dataset Used
- **Source**: **AdventureWorks2019 (Sales Schema)**
- **Schema Includes**:
  - `Customer`
  - `SalesOrderHeader`
  - `SalesOrderDetail`
  - `CurrencyRate`
  - `SpecialOffer`
  - **And more...**
- **File Format**: Parquet  
- **Storage**: Azure Data Lake Gen2  

---

## 🛠️ Project Setup
### **Prerequisites**
1. Azure Subscription.
2. SQL Server with **AdventureWorks2019 database**.
3. Azure Data Lake Gen2, Databricks, Data Factory, Synapse, and Power BI.
4. GitHub for version control.

### **Deployment Steps**
1. **Set up Azure Data Factory** to ingest data into **Bronze Layer**.
2. **Mount Data Lake Gen2 in Azure Databricks**.
3. **Transform Bronze → Silver → Gold using PySpark** in Databricks.
4. **Load Gold Layer data into Azure Synapse Analytics**.
5. **Connect Power BI to Synapse SQL Pool** for reporting.
6. **Secure data using Azure Entra ID and Key Vault**.

---

## 📊 Project Insights
- **Total Sales Per Year**
- **Top Selling Products**
- **Customer Purchase Trends**
- **Sales Performance by Region**
- **Revenue Growth Over Time**
- **Discount Impact on Sales**
- **High-Value Customers Identification**

---

## 🚀 Key Takeaways
✅ **Azure Data Engineering Best Practices**: Implemented **Medallion Architecture** for scalable data processing.  
✅ **Optimized ETL Workflows**: Using **PySpark in Azure Databricks** for high-performance transformations.  
✅ **Serverless Analytics**: Leveraged **Azure Synapse SQL Pool** for querying structured data.  
✅ **Data-Driven Insights**: Created **Power BI Dashboards** for business intelligence.  
✅ **Enterprise Security**: Implemented **RBAC, Key Vault, and GitHub for governance**.  

---

## 📜 Conclusion
This project **showcases the power of Azure** in **building a scalable, secure, and high-performance data pipeline**. It **demonstrates best practices for data engineering** using the **Medallion Architecture**, enabling **efficient data transformation and analytics**.

---

## 🛠️ Future Enhancements
🔹 Implement **Delta Lake** for better versioning & ACID compliance.  
🔹 Use **Azure Machine Learning** to predict future sales trends.  
🔹 Automate end-to-end pipeline with **Azure Data Factory triggers**.  
🔹 Optimize Power BI dashboards with **incremental data refresh**.  

---

## 📌 Author
**[Your Name]**  
📧 Contact: [Your Email]  
🔗 LinkedIn: [Your LinkedIn Profile]  
🚀 GitHub: [Your GitHub Profile]  
