# Retail Analysis using Microsoft Fabric & Power BI

## 📊 Project Overview
This project demonstrates an **end-to-end retail analytics solution** built using **Microsoft Fabric**, **Fabric Data Pipelines**, and **Power BI**.  
The solution follows **modern data warehousing best practices**, including a **staging layer**, **dimension tables**, **fact tables**, and a **star schema model**, to deliver meaningful business insights.

---

## 🏗 Overall Architecture
1. Raw data ingested using **Microsoft Fabric Data Pipelines**
2. Data stored in **staging tables** in Fabric Lakehouse
3. Transformed into **dimension and fact tables**
4. Star schema model created for analytics
5. Interactive dashboards built in **Power BI**

---

## 🔄 Data Ingestion – Microsoft Fabric Data Pipeline
- Automated ingestion of retail data
- Raw data loaded into staging tables
- Pipelines used to prepare data for analytical modeling

---

## 🧩 Data Modeling Approach

This project uses a **dimensional data model (Star Schema)** optimized for analytical reporting and Power BI performance.

### 🔹 Staging Tables
Staging tables store raw, untransformed data ingested from source systems.

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
  - City, state
  - Customer channel (Google, Facebook, Twitter, Organic, Affiliate)

---

### 🔹 Fact Tables
Fact tables store measurable transactional and event data.

- `fact_orders`
  - Order amount
  - Quantity
  - Order date
  - Product and user foreign keys

- `fact_reviews`
  - Product ratings
  - Review timestamps
  - User and product references

---

### 🔹 Schema Design
- Implemented as a **Star Schema**
- Optimized for reporting, aggregations, and drill-down analysis
- Improves query performance and dashboard responsiveness

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
- Revenue by customer channel
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
- Power BI
- GitHub
