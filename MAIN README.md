# Microsoft Fabric Data Engineering Project

## 📌 Overview

This repository documents my complete hands-on journey in Cloud Data Engineering using Microsoft Fabric.

The project follows a real-world Medallion Architecture approach and evolves from foundational ETL concepts to deployment, automation, enterprise data modeling, real-time API ingestion, and AI/ML integration.

The objective of this repository is not only to build dashboards, but to understand how modern enterprise data platforms are designed, orchestrated, optimized, and extended toward AI-driven systems.

---

## 🏗️ Project Architecture

```text
CSV / API Sources
        ↓
Fabric Pipelines (Scheduled)
        ↓
Bronze Layer
        ↓
Silver Layer
        ↓
Gold Layer
        ↓
Semantic Model
        ↓
Power BI Dashboard
```

---

## 🚀 Completed Phases

### 01️⃣ Incremental Load, MERGE & Partitioning

Focused on building the foundation of Medallion Architecture using Fabric and PySpark.

#### Features Implemented

✅ Bronze Layer (Raw Delta Tables)  
✅ Incremental Data Loading  
✅ MERGE (Upsert Logic)  
✅ Silver Layer Cleaning & Transformation  
✅ Data Standardization  
✅ Partitioning Optimization  
✅ Gold Layer Aggregation  
✅ Semantic Model Integration  
✅ Power BI Dashboard

#### Technologies Used

- Microsoft Fabric
- PySpark
- Delta Tables
- Power BI
- Semantic Models

---

### 02️⃣ Deployment & Automation

Focused on transforming manual ETL workflows into production-style pipelines.

#### Features Implemented

✅ Data Pipeline Orchestration  
✅ Notebook Automation  
✅ Scheduled Pipeline Execution  
✅ Semantic Model Refresh  
✅ Automated Dashboard Updates  
✅ Deployment Verification

#### Workflow

```text
Pipeline
   ↓
Bronze
   ↓
Silver
   ↓
Gold
   ↓
Refresh
   ↓
Dashboard
```

#### Technologies Used

- Microsoft Fabric Pipelines
- PySpark
- Semantic Models
- Power BI

---

### 03️⃣ Enterprise Data Modeling & BI

Focused on designing enterprise analytics structures using dimensional modeling.

#### Features Implemented

✅ Star Schema Design  
✅ Fact Table Creation  
✅ Dimension Table Creation  
✅ One-to-Many Relationships  
✅ Single Direction Filtering  
✅ DAX Measures  
✅ Time Intelligence Concepts  
✅ Power BI Semantic Relationships

#### Workflow

```text
Silver Layer
      ↓
Fact Table
      ↓
Dimension Tables
      ↓
Star Schema
      ↓
Semantic Model
      ↓
Power BI Analytics
```

#### Technologies Used

- PySpark
- Delta Tables
- Semantic Models
- Power BI
- DAX

---

### 04️⃣ Weather API Analytics Pipeline

Focused on real-time API ingestion and automated historical analytics.

#### Features Implemented

✅ OpenWeather API Integration  
✅ Raw JSON Bronze Storage  
✅ Silver Layer Data Flattening  
✅ Gold Layer Business Transformations  
✅ Historical Tracking (Append Mode)  
✅ Partitioning by Year & Month  
✅ Pipeline Automation  
✅ Power BI Dashboard

#### Workflow

```text
OpenWeather API
        ↓
API Bronze
        ↓
Silver History
        ↓
Gold History
        ↓
Partitioning
        ↓
Power BI Dashboard
```

#### Technologies Used

- OpenWeather API
- Microsoft Fabric
- PySpark
- Delta Tables
- Data Pipelines
- Power BI

---

## 🔮 Upcoming Phase

### 05️⃣ AI/ML Integration

Planned implementation:

- Feature Engineering
- Predictive Analytics
- Machine Learning Models
- AI-powered Insights
- End-to-End Data + AI Workflow

---

## 🎯 Key Concepts Covered

- Medallion Architecture
- ETL Pipelines
- Incremental Processing
- MERGE (Upsert Logic)
- Delta Lake Concepts
- Data Modeling
- Star Schema
- Semantic Modeling
- API Integration
- Historical Data Tracking
- Partitioning & Optimization
- Pipeline Automation
- Power BI Analytics
- Enterprise BI Design

---

## 📊 Tools & Technologies

- Microsoft Fabric
- PySpark
- Delta Lake
- Power BI
- Semantic Models
- Data Pipelines
- SQL
- Python
- OpenWeather API

---

## 📌 Repository Goal

This repository is designed as a progressive enterprise-style portfolio project demonstrating practical implementation of modern cloud data engineering concepts using Microsoft Fabric.

The goal is to simulate how real-world enterprise data platforms ingest, transform, optimize, automate, and analyze data at scale.
