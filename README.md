# SQL Data Warehouse ETL Project

## 🚀 Project Overview
This project demonstrates a modern SQL Data Warehouse architecture using a multi-layered ETL (Extract, Transform, Load) approach. It is designed to ingest, cleanse, and transform data from multiple sources into a robust analytics-ready warehouse.

---

## 📂 Data Sources
- **CRM System:**
  - `cust_info.csv`, `prd_info.csv`, `sales_details.csv`
- **ERP System:**
  - `CUST_AZ12.csv`, `LOC_A101.csv`, `PX_CAT_G1V2.csv`

All source files are located in the `datasets/` directory.

---

## 🏗️ Data Architecture
- **Bronze Layer:** Raw data ingestion
- **Silver Layer:** Cleansed and conformed data
- **Gold Layer:** Business-ready, aggregated data

---

## 🛠️ ETL Process
- **Bronze Scripts:**
  - `scripts/bronze/ddl_bronze.sql` (DDL for raw tables)
  - `scripts/bronze/proc_load_bronze.sql` (Load procedures)
- **Silver Scripts:**
  - `scripts/silver/ddl_silver.sql` (DDL for cleansed tables)
  - `scripts/silver/proc_load_silver.sql` (Transformation procedures)
- **Gold Scripts:**
  - `scripts/gold/ddl_gold.sql` (DDL for analytics tables)
- **Initialization:**
  - `scripts/init_database.sql` (Create database and schemas)

---

## 🧪 Data Quality
- `tests/quality_checks_silver.sql` (Silver layer checks)
- `tests/quality_checks_gold.sql` (Gold layer checks)

---

## 📁 Folder Structure
```
├── datasets/           # Source data files
│   ├── source_crm/
│   └── source_erp/
├── scripts/            # ETL SQL scripts
│   ├── bronze/
│   ├── silver/
│   └── gold/
├── tests/              # Data quality checks
├── README.md           # Project documentation
```

---

## ⚡ Getting Started
1. Clone this repository:
   ```sh
   git clone https://github.com/VedantShah26/SQl-Data-Warehouse-ETL-Project.git
   cd SQl-Data-Warehouse-ETL-Project
   ```
2. Review and run `scripts/init_database.sql` to set up your database.
3. Execute ETL scripts in order: Bronze → Silver → Gold.
4. Run quality checks in the `tests/` folder.

---

## 📜 License
This project is licensed under the terms of the [LICENSE](LICENSE).
