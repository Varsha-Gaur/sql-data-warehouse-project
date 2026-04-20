# 🏗️ Modern Data Warehouse using Medallion Architecture

## 📌 Overview
This project demonstrates the design and implementation of a **scalable modern data warehouse** using the **Medallion Architecture (Bronze, Silver, Gold layers)**.

The system ingests raw data from multiple sources, processes it through structured transformation layers, and delivers **analytics-ready datasets** for reporting and business intelligence.

---

## 🎯 Problem Statement
Organizations often deal with fragmented data from multiple systems such as ERP and CRM, leading to:
- Inconsistent data formats  
- Poor data quality  
- Inefficient reporting and analytics  

This project addresses these challenges by building a **centralized, clean, and optimized data warehouse**.

---

## 🧠 Architecture

### 🔹 Medallion Architecture Layers

#### 🟤 Bronze Layer (Raw Data)
- Ingests raw data from CSV files (ERP & CRM systems)
- Stores data in SQL Server without transformation
- Acts as a single source of truth

#### ⚪ Silver Layer (Cleaned Data)
- Handles data cleaning and transformation
- Removes duplicates and null values
- Standardizes formats and ensures consistency

#### 🟡 Gold Layer (Business Layer)
- Transforms data into **analytics-ready format**
- Implements **Star Schema (Fact & Dimension Tables)**
- Optimized for reporting and business queries

---

## 🏛️ Data Modeling

- Designed **Fact Tables** for transactional data  
- Created **Dimension Tables** for descriptive attributes  
- Implemented **Star Schema** for efficient querying  
- Optimized schema for:
  - Fast aggregations  
  - Query performance  
  - Scalability  

---

## ⚙️ ETL Pipeline

### 🔄 Pipeline Workflow

1. **Extract**
   - Load raw CSV files into SQL Server (Bronze layer)

2. **Transform**
   - Clean, validate, and standardize data (Silver layer)

3. **Load**
   - Insert processed data into analytical tables (Gold layer)

### ✨ Features
- Automated data processing  
- Data validation and error handling  
- Scalable pipeline design  

---

## 📊 Analytics & Insights

Built SQL-based analytics to derive insights on:
- 📈 Sales Trends  
- 🛍️ Product Performance  
- 👥 Customer Behavior  

---

## 🛠️ Tech Stack

| Category            | Tools / Technologies |
|--------------------|--------------------|
| Database           | SQL Server         |
| Language           | SQL                |
| Data Processing    | ETL Pipelines      |
| Tools              | SSMS, DrawIO, Git  |
| Data Modeling      | Star Schema        |

---

## 📂 Project Structure
│
├── datasets/ # Raw datasets (ERP & CRM)
│
├── docs/ # Documentation and diagrams
│ ├── data_architecture.drawio
│ ├── data_flow.drawio
│ ├── data_models.drawio
│ ├── data_catalog.md
│
├── scripts/
│ ├── bronze/ # Data ingestion scripts
│ ├── silver/ # Data transformation scripts
│ ├── gold/ # Analytical models
│
├── tests/ # Data validation scripts
│
├── README.md
