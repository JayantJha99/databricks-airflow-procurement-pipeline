# Enterprise Procurement Data Platform using Databricks and Airflow

## Overview

Built enterprise-scale ETL/ELT pipelines for procurement and supply-chain analytics workflows for renewable energy operations.

The platform processes Purchase Orders (POs), shipments, receipts, Accounts Payable (AP), and ERP transactional data from multiple enterprise systems into analytics-ready datasets for BI and reporting teams.

---

## Business Context

The project handled procurement lifecycle data for renewable energy equipment operations including:

* Windmill components
* Turbine systems
* Purchase orders
* Shipment tracking
* Vendor and distribution workflows

The transformed datasets were consumed by Tableau and Power BI reporting systems.

---

## Architecture
<img width="1024" height="962" alt="image" src="https://github.com/user-attachments/assets/8212fbb5-58a0-4a03-a9fc-16dcb0eb44e7" />

### Ingestion Layer

Source systems:

* SAP
* Oracle ERP
* BAAN
* Powermax
* Alpha
* CCL
* DOOSAN
* SAP Repairs

Data ingestion into Databricks Bronze layer from cloud storage and enterprise systems.

---

### Bronze Layer

* Raw ingestion tables
* Incremental ingestion
* ERP raw data storage
* Partitioned ingestion

---

### Silver Layer

* Deduplication
* Data harmonization
* Business rule implementation
* Incremental transformations

---

### Gold Layer

* PSOTs (Primary Source of Truth)
* CSOTs (Consumer Source of Truth)
* Curated reporting datasets
* Tableau and Power BI reporting

---

## Tech Stack

* Databricks
* PySpark
* Apache Airflow
* SQL
* DBeaver
* AWS S3
* Python
* Power BI
* Tableau
* YAML
* GitHub

---

## Key Features

* Enterprise Airflow DAG orchestration
* YAML-driven workflow creation
* Databricks notebook execution
* Procurement lifecycle processing
* ERP data integration
* Outgestion DAG pipelines
* SQL transformation jobs
* Data reconciliation workflows
* BI reporting datasets

---

## Airflow Orchestration

<img width="1280" height="495" alt="image" src="https://github.com/user-attachments/assets/56ab8e90-ce8c-4acc-8843-1db13fd01e7d" />


Implemented Airflow DAGs for:

* Scheduling workflows
* Databricks notebook execution
* Validation checks
* SQL transformations
* Outgestion pipelines
* Box uploads
* Stakeholder notifications

DAGs were configured using YAML-based workflow metadata including:

* DAG IDs
* CRON schedules
* Retry policies
* Timezones
* Tags

---

## Performance Optimizations

* Reduced query latency by 50%
* Moved complex filter conditions upstream
* Optimized SQL joins and unions
* Reduced unnecessary downstream processing
* Improved pipeline efficiency and operational reliability

---

## Data Quality & Debugging

Resolved enterprise-scale data issues including:

* Currency code mismatches
* NULL propagation
* Cancel flag inconsistencies
* Imported flag validation
* PO distribution reconciliation
* Duplicate active records

---

## CI/CD Workflow

* Feature branch development
* Pull request approval workflow
* Data architect review process
* GitHub-based deployment flow
* Environment promotion from DEV → PROD

---


## Future Improvements

* Delta Live Tables
* Unity Catalog integration
* Real-time streaming architecture
* Data observability tooling
* Automated lineage tracking

---

## Author

Jayant Jha
