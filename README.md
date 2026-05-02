# 🚀 End-to-End Data Engineering Pipeline using Microsoft Fabric  
### (Incremental Load • MERGE • Partitioning • Power BI)

---

## 📌 Overview

This project demonstrates a complete end-to-end data engineering pipeline built on Microsoft Fabric.  
It follows the Medallion Architecture (Bronze → Silver → Gold) and implements real-world concepts such as incremental data loading, MERGE (upsert), and partitioning for performance optimization.

The pipeline processes raw sales data and transforms it into business-ready insights visualized through an interactive Power BI dashboard.

---

## 🏗️ Architecture

This pipeline consists of:

- **Bronze Layer** → Raw data ingestion with incremental load and MERGE  
- **Silver Layer** → Data cleaning, transformation, and partitioning  
- **Gold Layer** → Aggregated business metrics  
- **Semantic Model** → Direct Lake connection  
- **Power BI Dashboard** → Visualization and insights  

---

## ⚙️ Tech Stack

- Microsoft Fabric  
- PySpark  
- Delta Lake  
- Power BI  
- OneLake  

---

## 🔄 Pipeline Flow
CSV Dataset → Bronze → Silver → Gold → Semantic Model → Power BI Dashboard

---

## 🔥 Key Features

### ✅ Incremental Load
- Simulated real-world ingestion using date-based slicing  
- Avoids full dataset reloads  

### ✅ MERGE (Upsert Logic)
- Prevents duplicate records  
- Handles both updates and inserts efficiently  

### ✅ Partitioning (Optimization)
- Implemented in Silver Layer  
- Improves query performance by reducing data scan  

### ✅ Data Cleaning
- Removed null values  
- Eliminated duplicates  
- Standardized inconsistent categories  

### ✅ Live Dashboard
- Connected using semantic model  
- Reflects real-time data updates  

---

## 📊 Dashboard

The Power BI dashboard provides:

- 📈 KPI → Total Revenue  
- 📊 Bar Chart → Revenue by Category  
- 🍩 Donut Chart → Revenue Distribution  
- 🎯 Slicer → Category Filtering  

---

## 🧪 Data Validation (Live Testing)

To confirm live data connection:

- Modified revenue values in Silver layer  
- Rebuilt Gold layer  
- Refreshed semantic model and dashboard  
- Verified updated results in visuals  

---

---

## 📄 Documentation

A detailed explanation of each step, including incremental logic, MERGE operations, and partitioning, is available in the documentation (Checkout Brief Explanation)


---

## 🚀 Key Learnings

- Built scalable pipelines using incremental processing  
- Implemented MERGE (upsert) using Delta Tables  
- Optimized performance using partitioning  
- Understood real-world data engineering workflows  
- Integrated data pipeline with BI reporting  

---

## 🎯 Future Improvements

- Add real-time data ingestion using APIs  
- Implement pipeline scheduling and automation  
- Integrate AI/ML layer for predictive analytics  

---

## 👨‍💻 Author

Ahmed Irshad Hussain  

---

## ⭐ If you found this useful

Give this repo a ⭐ and feel free to connect!
