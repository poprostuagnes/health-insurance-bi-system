# Health Insurance Business Intelligence & Predictive Analytics System

A comprehensive, production-grade **Business Intelligence (BI)** and **Data Mining** enterprise system designed for the medical insurance sector. The pipeline processes a high-volume dataset containing over **1,000,000 unique patient records**, transforming raw financial and physiological data into actionable strategic insights.

The project was developed as an engineering system implementation at the **Rzeszów University of Technology** (Field: *Data Engineering and Analysis*).

---

## Tech Stack & System Architecture

The project implements a complete, end-to-end data pipeline leveraging the full **Microsoft Business Intelligence** ecosystem:

*   **Data Warehouse (SQL Server):** Designed a physical relational database model utilizing a high-performance **Star Schema** (`Fact_Insurance` surrounded by optimized dimension tables: `Dim_Patient`, `Dim_Medical`, `Dim_Profile`, and `Dim_Coverage`). Developed a robust **Staging Area** to buffer and isolate raw I/O data streams.
*   **Data Integration & Quality (SSIS):** Automated sequential data ingestion through multiple Data Flow Tasks. Implemented strict data cleansing routines via **Fuzzy Lookup** algorithms (for typographical auto-correction) and transactional stability through kaskade validation and soft error-handling (`Redirect Row` log redirection).
*   **Multidimensional Analytics (SSAS):** Built an **OLAP Cube** featuring multi-level analytics hierarchies (*socio-geographic* and *demographic* drill-down dimensions). Developed dynamic, pre-compiled calculated measures and strategic financial risk alert monitors (**KPIs**) using advanced **MDX (Multi-Dimensional Expressions)**.
*   **Data Mining & AI Engine (SSAS Data Mining):** Configured and evaluated three competing machine learning algorithms via **DMX (Data Mining Extensions)** queries:
    *   *Microsoft Decision Trees* (for transparent, rule-based cost division routing)
    *   *Microsoft Clustering* (for unsupervised segment discovery and patient cohort mining)
    *   *Microsoft Neural Network* (for handling multi-layered, non-linear sensitivity analytics)
*   **Data Visualization & Reporting (Power BI):** Designed interactive, C-level analytical executive dashboards connected directly via a server-side **Connect Live** mechanism to process queries in milliseconds.

---

## Executive Summary & Key Findings

*   **Risk Factors Discovered:** The Neural Network and Decision Tree predictive models mathematically proved that the highest financial risk factor (information gain) for the portfolio is **nicotine addiction correlated with physiological obesity ($BMI > 30$)** and mature age.
*   **Model Validation:** Direct validation on the Power BI dashboard (focusing on the 18–41 age cohort) demonstrated that the **Neural Network** and **Decision Tree** models provide the highest precision, dynamically aligning with real-world financial cost trends, whereas clustering serves best for global static baselines.
*   **Business Impact:** The system equips insurance actuaries with an early warning mechanism, enabling predictive premium optimization, CRM integration, and proactive healthcare prevention routing (e.g., targeted wellness program discounts).

---

##  Repository Structure & Documentation

*   `/Dim *.dim`, `/*.cube`, `/*.dsv`, `/*.dmm` — Native Microsoft XML architecture and schema definition files mapping out dimensions, cube aggregations, and data mining models.
*   `Sprawozdanie1.pdf` — Full academic engineering documentation containing comprehensive technical specifications, process schematics, ETL graphs, and BI design parameters (written in Polish).

---

