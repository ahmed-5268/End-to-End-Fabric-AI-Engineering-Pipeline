# Star Schema & Enterprise BI Modeling — Microsoft Fabric

This phase extends the existing Medallion Architecture pipeline by transforming the Gold Layer into a proper Enterprise Star Schema model for scalable analytics and business intelligence.

---

# Objective

The original Gold layer contained simple aggregated data:

| category    | total_revenue |
| ----------- | ------------- |
| Electronics | 500000        |
| Clothing    | 90000         |

While useful for basic reporting, this structure could not support:

* Time intelligence
* Quarterly comparisons
* Dynamic drilldowns
* Enterprise BI analytics
* Scalable semantic modeling

To solve this, the Gold layer was redesigned into a Star Schema architecture.

---

# Architecture

## Fact Table

### `fact_sales`

Stores transactional metrics:

* sale_id
* product_id
* date_id
* revenue
* quantity

---

## Dimension Tables

### `dim_product`

Stores descriptive product/category information.

Columns:

* product_id
* category

### `dim_date`

Stores analytical time attributes.

Columns:

* date_id
* date
* month
* quarter
* year

---

# Key Concepts Implemented

## Star Schema Modeling

Implemented enterprise dimensional modeling using:

* Fact tables
* Dimension tables
* One-to-Many relationships

---

## Surrogate Key Generation

Used:

* `row_number()` for sequential transaction IDs
* `dense_rank()` for dimension consistency

### Why `dense_rank()`?

Example:

| category | sub_category |
| -------- | ------------ |
| Clothing | Shirts       |
| Clothing | Pants        |

Both belong to the same category and should share the same dimension identifier.

Using `row_number()` would generate different IDs and break analytical consistency.

---

# Power BI Semantic Modeling

Created relationships:

* `dim_product.product_id → fact_sales.product_id`
* `dim_date.date_id → fact_sales.date_id`

Relationship configuration:

* One-to-Many
* Single Direction Filtering

---

# DAX Measures Implemented

* Total Revenue
* YTD Revenue
* Previous Month Revenue
* Revenue Growth %

---

# Enterprise BI Concepts Learned

* Dimensional Modeling
* Filter Propagation
* Cardinality
* Semantic Layer Design
* Time Intelligence
* Analytical Modeling

---

# Tech Stack

* Microsoft Fabric
* PySpark
* Delta Lake
* Power BI
* DAX
* Lakehouse Architecture

---

# Project Evolution

✅ Medallion Architecture
✅ Incremental Load + MERGE + Partitioning
✅ Deployment & Automation
✅ Star Schema + DAX + Semantic Modeling

🔜 API Ingestion
🔜 AI/ML Integration
🔜 Real-Time Streaming Pipelines
