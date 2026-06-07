# Clinical Data Lakehouse Modernization

## Project Overview

This project focuses on building a modern Clinical Data Lakehouse to centralize, process, and analyze clinical trial data from ClinicalTrials.gov. The solution leverages AWS S3, Databricks, and Power BI to transform raw clinical data into business-ready insights and interactive dashboards.

The platform follows the Medallion Architecture (Bronze, Silver, Gold) to ensure data quality, scalability, and efficient analytics.

---

## Business Challenge

Clinical trial data is generated across multiple sponsors, research organizations, and healthcare institutions. As data volume increases, organizations face challenges such as:

* Data fragmentation across systems
* Inconsistent data formats
* Limited visibility into trial performance
* Manual reporting processes
* Delayed decision-making

---

## Project Objective

The objective of this project is to build a centralized Clinical Data Lakehouse that:

* Improves data quality and consistency
* Enables scalable data processing
* Provides analytics-ready datasets
* Supports interactive reporting
* Facilitates data-driven decision making

---

## Dataset

**Source:** ClinicalTrials.gov

ClinicalTrials.gov is a publicly accessible clinical research database maintained by the U.S. National Library of Medicine (NLM) under the National Institutes of Health (NIH).

### Dataset Includes

* Study Information
* Sponsor Details
* Study Status
* Study Phase
* Enrollment Information
* Geographic Locations
* Funder Information

---

## Technology Stack

| Component                | Technology             |
| ------------------------ | ---------------------- |
| Cloud Storage            | AWS S3                 |
| Data Processing          | Databricks             |
| Data Transformation      | PySpark, SQL           |
| Data Architecture        | Medallion Architecture |
| Data Modeling            | Star Schema            |
| Reporting                | Power BI               |
| Conversational Analytics | Genie Space            |

---

## Solution Architecture

ClinicalTrials.gov Dataset
→ AWS S3
→ Databricks Bronze Layer
→ Databricks Silver Layer
→ Databricks Gold Layer
→ Power BI Dashboards & Genie Space

---

## Medallion Architecture

### Bronze Layer

* Stores raw clinical trial data
* Preserves source data integrity
* Serves as the foundation for downstream processing

### Silver Layer

* Cleans and standardizes data
* Removes duplicates and inconsistencies
* Performs data quality validation

### Gold Layer

* Creates business-ready datasets
* Builds fact and dimension tables
* Supports reporting and analytics

---

## Data Processing Workflow

### Extract

* Load clinical trial data from AWS S3

### Transform

* Data cleansing
* Standardization
* Validation
* Deduplication

### Load

* Store processed data in Bronze, Silver, and Gold layers

---

## Data Model

A Star Schema was implemented to support efficient reporting and dashboard development.

### Fact Table

* Clinical Trial Metrics
* Enrollment Metrics

### Dimension Tables

* Sponsor
* Study Phase
* Study Status
* Location
* Funder Type

---

## Dashboards

### Clinical Trial Portfolio Health

Provides an overview of trial activity, study status, and enrollment trends.

### Sponsor Performance Intelligence

Analyzes sponsor contributions, trial distribution, and performance metrics.

### Geographic & Site Analytics

Visualizes trial activity across countries and research locations.

### Phase & Status Intelligence

Examines study phases, completion status, and operational trends.

---

## Genie Space

Genie Space enables users to explore clinical trial data using natural language queries.

Example Questions:

* Which sponsor has the highest trial count?
* Which phase has the highest enrollment?
* Show completed trials by year.

---

## Key Insights

* Completed studies represent the largest share of the clinical trial portfolio.
* Phase 1 and Phase 2 studies contribute significant trial activity.
* Sponsor participation is concentrated among leading organizations.
* Trial activity is concentrated in key geographic regions.
* Enrollment patterns vary across study phases.

---

## Business Impact

* Centralized clinical trial analytics platform
* Improved data quality and consistency
* Reduced manual reporting effort
* Faster access to insights
* Enhanced decision-making capabilities
* Scalable foundation for future analytics initiatives

---

## Future Enhancements

* Predictive Analytics
* Real-Time Data Integration
* AI-Assisted Trial Monitoring
* Advanced Recruitment Forecasting
* Enhanced Conversational Analytics

---

## Author

Clinical Data Lakehouse Modernization Project

Built using AWS S3, Databricks, Power BI, and Genie Space.
