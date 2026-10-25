# SQL Server Data Warehouse Project | End-to-End ETL & Analytics

## 📌 Project Overview

This project demonstrates the design and implementation of a modern **SQL Server Data Warehouse** that integrates sales data from two source systems: **Customer Relationship Management (CRM)** and **Enterprise Resource Planning (ERP)**.

The project follows the **Medallion Architecture (Bronze, Silver, and Gold)** to transform raw CSV files into clean, integrated, and analysis-ready data. It covers the complete data engineering workflow, from data ingestion and data cleansing to dimensional modeling and analytical reporting.

The primary objective is to build a centralized data warehouse that supports reliable business intelligence and data-driven decision-making.

## 🎯 Project Objectives

- Design a modern data warehouse using Microsoft SQL Server.
- Ingest raw data from CRM and ERP source systems.
- Develop ETL pipelines to load, transform, and integrate data.
- Identify and resolve data quality issues.
- Implement a layered data architecture using Bronze, Silver, and Gold layers.
- Build fact and dimension tables using a star schema.
- Perform SQL-based exploratory and business analysis.
- Document the architecture, data model, and implementation process.

## 🏗️ Data Architecture

The project follows the Medallion Architecture, separating data processing into three layers.

### 1. Bronze Layer — Raw Data

- Loads source data from CSV files into SQL Server.
- Preserves the raw data as received from the source systems.
- Serves as the foundation for subsequent transformation processes.

### 2. Silver Layer — Cleaned and Integrated Data

- Cleans and standardizes the raw data.
- Handles missing values, duplicates, and inconsistent formats where applicable.
- Resolves data quality issues and integrates CRM and ERP data.
- Prepares reliable datasets for analytical modeling.

### 3. Gold Layer — Business-Ready Data

- Organizes transformed data into a dimensional model.
- Implements fact and dimension tables using a star schema.
- Provides a simplified structure for analytical queries and reporting.
- Supports business insights and data-driven decision-making.

## 🔄 ETL Workflow

The project follows this end-to-end data pipeline:

**Source CSV Files → Bronze Layer → Silver Layer → Gold Layer → SQL Analytics**

1. **Extract:** Ingest raw CRM and ERP datasets from CSV files.
2. **Load:** Store the source data in the Bronze layer.
3. **Transform:** Clean, standardize, validate, and integrate the data in the Silver layer.
4. **Model:** Create analytical fact and dimension tables in the Gold layer.
5. **Analyze:** Use SQL queries to explore sales data and derive business insights.

## 📂 Repository Structure

```text
sql-data-warehouse-project/
│
├── 00_setup/
│   └── Setup guide and Docker configuration
│
├── 01_datasets/
│   ├── source_crm/
│   │   └── CRM source CSV files
│   └── source_erp/
│       └── ERP source CSV files
│
├── 02_docs/
│   ├── Data architecture diagrams
│   ├── Project requirements
│   └── Data model documentation
│
├── 03_scripts/
│   ├── init_database.sql
│   ├── bronze/
│   │   └── Raw data ingestion scripts
│   ├── silver/
│   │   └── Data cleansing and transformation scripts
│   └── gold/
│       └── Analytical data modeling scripts
│
└── 04_tests/
    └── Data quality validation scripts
```

## 🛠️ Technologies Used

- **Microsoft SQL Server** — Data storage and warehouse implementation.
- **T-SQL** — Data manipulation, transformation, stored procedures, and analytical queries.
- **SQL Server Management Studio (SSMS)** — Database development and query execution.
- **CSV Files** — Source data from CRM and ERP systems.
- **Git & GitHub** — Version control and project documentation.
- **draw.io** — Data architecture and dimensional modeling diagrams.
- **Docker** — Optional environment setup where supported by the project guide.

## 🚀 Getting Started

### Prerequisites

- Microsoft SQL Server or a compatible SQL Server environment.
- SQL Server Management Studio (SSMS) or another compatible SQL client.
- Git (optional, for cloning the repository).
- The source CSV files included in the project.

### Installation and Execution

**Step 1: Clone the repository**

```bash
git clone <your-github-repository-url>
cd sql-data-warehouse-project
```

**Step 2: Review the setup guide**

Navigate to the `00_setup/` directory and follow the instructions for configuring SQL Server and creating the required database.

**Step 3: Configure source file paths**

The default source file location used by the loading procedure is:

```text
C:\sql\dwh_project\01_datasets\
```

Place the dataset folder at the expected location or update the six CSV file paths in:

```text
03_scripts/bronze/proc_load_bronze.sql
```

Ensure SQL Server has permission to access the source files. If using Docker or another operating system, configure the appropriate mounted paths and file permissions.

**Step 4: Initialize the database**

Execute the following script first in SQL Server Management Studio:

```text
03_scripts/init_database.sql
```

**Step 5: Load the Bronze layer**

Execute the scripts in `03_scripts/bronze/` to load the raw source data into the warehouse.

**Step 6: Transform the Silver layer**

Execute the scripts in `03_scripts/silver/` to cleanse, standardize, and integrate the data.

**Step 7: Build the Gold layer**

Execute the scripts in `03_scripts/gold/` to create the business-ready fact and dimension tables.

**Step 8: Validate data quality**

Run the relevant scripts in `04_tests/` to validate the Silver and Gold datasets.

**Step 9: Perform data analysis**

Use SQL queries against the Gold layer to explore sales performance and answer business questions.

*Note: Execute the scripts in the intended order and follow any additional instructions provided in the setup guide.*

## 📊 Key Learning Outcomes

Through this project, I aim to strengthen my understanding of:

- End-to-end data warehouse development.
- ETL pipeline design and implementation using T-SQL.
- Data cleansing, standardization, and integration.
- Medallion Architecture and layered data processing.
- Dimensional modeling and star schema design.
- Data quality testing and validation.
- Analytical SQL queries and business intelligence fundamentals.
- Version control and project documentation using GitHub.

## 📋 Project Scope

- **Data sources:** CRM and ERP.
- **Input format:** CSV.
- **Database platform:** Microsoft SQL Server.
- **Architecture:** Bronze, Silver, and Gold layers.
- **Data model:** Star schema with fact and dimension tables.
- **Data scope:** Latest dataset only; historical data tracking is not required.
- **Primary outcome:** A clean, integrated, and analysis-ready data warehouse.

## 👨‍💻 About Me

I am an engineering student developing my skills in **SQL, data analytics, and data engineering**, with an interest in using data to solve real-world business problems.

I enjoy learning through hands-on projects that connect technical concepts with practical applications. Through this project, I am building a stronger foundation in database management, ETL pipeline development, data modeling, and analytical problem-solving.

I am continuously exploring opportunities to apply my technical skills, learn new tools, and grow in the fields of data analytics and data engineering.

## 🤝 Connect With Me

- **LinkedIn:** [Chakradhar Allu]([https://www.linkedin.com/](https://www.linkedin.com/in/chakradhar-allu-22117a290/?isSelfProfile=true))
- **GitHub:** [Chakradhar Allu]([https://github.com/](https://github.com/alluchakradhar972-wq))

---

⭐ If you find this project useful, feel free to explore the repository and share your feedback.

