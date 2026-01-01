# Retail Analysis using Microsoft Fabric & Power BI

## 📊 Project Overview
This project demonstrates an **end-to-end retail analytics solution** built using **Microsoft Fabric**, **Fabric Data Pipelines**, and **Power BI**.  
The solution follows **modern data warehousing best practices**, including a **staging layer**, **dimension tables**, **fact tables**, and a **star schema model**, with data stored in **Parquet file format** for optimized performance.

---

## 🏗 Overall Architecture
1. Raw data ingested using **Microsoft Fabric Data Pipelines**
2. Data stored in **Parquet format** within Fabric Lakehouse
3. Data organized into **staging tables**
4. Transformed into **dimension and fact tables**
5. Star schema model created for analytics
6. Interactive dashboards built in **Power BI**

---

## 🔄 Data Ingestion – Microsoft Fabric Data Pipeline
- Automated ingestion of retail data using Fabric Data Pipelines
- Raw data landed as **Parquet files** in the Lakehouse
- Parquet format chosen for:
  - Columnar storage
  - Faster query performance
  - Reduced storage size
  - Optimized analytics workloads

---

## 🧩 Data Modeling Approach

This project uses a **dimensional data model (Star Schema)** optimized for analytical reporting and Power BI performance.

### 🔹 Staging Tables
Staging tables store raw, untransformed data ingested from source systems and saved in **Parquet format**.

- `stg_orders`
- `stg_products`
- `stg_users`
- `stg_reviews`

---

### 🔹 Dimension Tables
Dimension tables provide descriptive attributes used for slicing and filtering analysis.

- `dim_products`
  - Product information
  - Category
  - Vendor details

- `dim_users`
  - Customer details
  - City and state
  - Customer channel (Google, Facebook, Twitter, Organic, Affiliate)

---

### 🔹 Fact Tables
Fact tables store measurable transactional and event-based data.

- `fact_orders`
  - Order amount
  - Quantity
  - Order date
  - Foreign keys to product and user dimensions

- `fact_reviews`
  - Product ratings
  - Review timestamps
  - User and product references

---

### 🔹 Schema Design
- Implemented as a **Star Schema**
- Stored in **Parquet format** for efficient analytics
- Optimized for aggregations, joins, and drill-down analysis in Power BI

---

## 📈 Power BI Dashboard Highlights

### 🔹 Key KPIs
- **Total Revenue:** €388.3K  
- **Total Orders:** 1.86K  
- **Average Basket Amount:** €208.29  
- **Average Product Rating:** 3.99  

---

### 🔹 Business Insights
- Monthly revenue trends (2017–2020)
- Revenue by customer channel:
  - Google
  - Facebook
  - Twitter
  - Organic
  - Affiliate
- Geographic revenue distribution by state
- Product, vendor, and category performance
- Quantity sold vs average product rating analysis

---

## 🛠 Tools & Technologies Used
- Microsoft Fabric
- Fabric Data Pipelines
- Fabric Lakehouse / OneLake
- **Parquet file format**
- Power BI
- GitHub
