# 🌦 Weather API Analytics – End-to-End Microsoft Fabric Project

## Overview

This project demonstrates an end-to-end real-time weather analytics pipeline built using Microsoft Fabric and OpenWeather API.

The pipeline follows a Medallion Architecture approach:

OpenWeather API → Bronze → Silver → Gold → Partitioning → Pipeline Automation → Power BI Dashboard

The project simulates how enterprise data systems ingest, process, optimize, and visualize live data.

---

## Architecture Flow

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
Semantic Model
        ↓
Power BI Dashboard

---

## Technologies Used

- Microsoft Fabric
- PySpark
- Delta Tables
- Lakehouse
- Data Pipelines
- OpenWeather API
- Power BI
- DAX

---

## Project Features

### API Data Ingestion
- Connected to OpenWeather API
- Pulled real-time weather JSON response
- Stored raw API data in Bronze Layer

### Bronze Layer
- Raw JSON response stored without modification
- Preserves original source data

Table:

bronze_weather_history

---

### Silver Layer
- Flattened nested JSON structure
- Renamed and standardized columns
- Cleaned data for analytics

Table:

silver_weather_history

---

### Gold Layer
- Applied business transformations
- Created temperature categories:
    - Cold
    - Moderate
    - Hot

Table:

gold_weather_history

---

### Historical Tracking
Used append mode to preserve historical weather records instead of overwriting previous data.

Benefits:

- Trend analysis
- Time intelligence
- Historical comparisons

---

### Partitioning

Partitioned data by:

- Year
- Month

Benefits:

- Faster queries
- Reduced scan cost
- Better performance

Table:

gold_weather_partitioned

---

### Pipeline Automation

Created a Fabric Data Pipeline:

API Bronze
↓
Silver History
↓
Gold History
↓
Partitioning

Configured sequential execution and scheduling.

---

### Power BI Dashboard

Dashboard contains:

- City KPI
- Current Temperature KPI
- Current Humidity KPI
- Wind Speed KPI
- Historical Trend Analysis

---

## Future Improvements

- Multi-city weather ingestion
- Weather forecasting API
- AI/ML prediction layer
- Real-time streaming
- Anomaly detection

---
Author

Ahmed Irshad Hussain
