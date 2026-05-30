# Renewable Energy ETL and Analytics Pipeline

## Overview

This project implements a complete ETL (Extract, Transform, Load) and analytics pipeline using renewable energy production data.

The objective is to transform raw dimensional and fact datasets into a validated analytical dataset capable of supporting SQL-based business analysis and visualization.

The pipeline includes data quality validation, duplicate detection, referential integrity checks, warehouse assembly, SQL analytics, and trend visualization.

---

## Project Architecture

```text
Raw Data
    ↓
Data Ingestion
    ↓
Data Quality Validation
    ↓
Data Cleaning
    ↓
Warehouse Assembly
    ↓
SQLite Analytical Layer
    ↓
SQL Analysis
    ↓
Visualization & Reporting
```

---

## Dataset Structure

### Dimensions

* Country Dimension
* Energy Source Dimension
* Time Dimension

### Fact Table

Energy production measurements indexed by:

* country_id
* source_id
* time_id

---

## Data Quality Checks

The pipeline performs:

### Missing Value Analysis

Identification of null values before transformations.

### Duplicate Detection

Detection and removal of duplicated measurements.

### Referential Integrity Validation

Verification that all foreign keys in the fact table exist within their corresponding dimensions.

---

## Transformations

The project performs:

* Duplicate removal
* Dimension enrichment
* Fact and dimension integration
* Analytical dataset generation

---

## SQL Analytics

The analytical layer is implemented using SQLite.

Examples of techniques used:

* Common Table Expressions (CTEs)
* Aggregate Functions
* Window Functions
* Year-over-Year calculations

### Example Business Questions

1. Which countries maintain high renewable participation in their energy matrix?

2. How has Brazil's renewable share evolved over time?

3. What are the year-over-year growth trends for renewable energy production?

---

## Visualization

The project generates analytical visualizations including:

* Renewable energy participation over time
* Year-over-Year growth analysis
* Combined trend and growth reporting

---

## Technologies

* Python
* Pandas
* SQLite
* SQL
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Key Skills Demonstrated

### Data Engineering

* ETL Design
* Data Validation
* Data Cleaning
* Dimensional Modeling
* Data Warehousing Concepts

### Analytics

* SQL Analysis
* Window Functions
* Business Metrics
* Data Visualization

---

## Future Improvements

* Automated pipeline execution
* Scheduled ingestion workflows
* Cloud storage integration
* Dashboard deployment
* Data quality monitoring

---

## Author

Lúcia Katze Lyra

Data Engineering and Analytics enthusiast/Dev
