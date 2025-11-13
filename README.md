# 🧠 Talend Data Engineering Portfolio — Banking & NBFC Domain

Welcome to my **Talend Open Studio Data Engineering Portfolio**, showcasing a collection of **real-world ETL, data integration, and data warehouse projects** built specifically for **Banking and NBFC (Non-Banking Financial Company)** use cases.

This repository demonstrates my expertise in **designing, building, and automating Talend pipelines** for business-critical data processes such as **Customer 360, Loan Management, Credit Bureau Integration, Payment Analytics, and Fraud Detection.**

---

## 🚀 Key Highlights

- 💾 **End-to-End ETL Workflows** — from raw ingestion to processed and curated data zones.  
- 🧩 **Talend Components Used:** tFileInputDelimited, tMap, tAggregateRow, tFilterRow, tRESTClient, tKafkaInput, tSnowflakeOutput, tPostgresqlOutput, etc.  
- 🧠 **Data Modeling Concepts:** Dimensional modeling, Star Schema, SCD Type 2, Incremental loads.  
- ⚙️ **Job Design Principles:** Parameterized, reusable, metadata-driven jobs with clear naming and error handling.  
- 📊 **Use Case Driven:** Designed for NBFC operational and analytics use cases — such as customer onboarding, loan tracking, EMI collection, and payment defaults.

---

## 🏦 Project Portfolio

### 🧩 1. **Customer 360° Data Integration**

**Goal:** Build a unified Customer 360 dataset by integrating data from CRM, Loan Management, and Payment systems.

**Features:**
- Ingest data from multiple source files and databases.
- Perform data cleansing, de-duplication, and SCD Type 2 merge.
- Generate a **Customer Master Table** for analytics and compliance.

**Talend Components Used:**  
`tFileInputDelimited`, `tMap`, `tJoin`, `tAggregateRow`, `tPostgresqlOutput`

**Data Flow:**  
`Raw Files → Transformation (tMap/tJoin) → SCD Merge → Target Warehouse`

---

### ⚙️ 2. **Loan Disbursement & Repayment ETL**

**Goal:** Automate daily ETL for loan disbursement and repayment tracking for NBFC portfolios.

**Features:**
- Load loan and repayment data from core banking systems.
- Apply business rules to calculate outstanding balance and DPD (Days Past Due).
- Maintain historical snapshots for each customer.

**Talend Components Used:**  
`tOracleInput`, `tMap`, `tFilterRow`, `tAggregateRow`, `tFileOutputDelimited`

**Data Flow:**  
`DB Extract → Transformation → Loan Summary Fact Table`

---

### 💳 3. **Credit Bureau API Integration**

**Goal:** Fetch customer credit score and credit history from external Credit Bureau APIs.

**Features:**
- Call REST APIs for each customer using `tRESTClient`.
- Parse JSON responses using `tExtractJSONFields`.
- Merge credit data with customer master dataset.

**Talend Components Used:**  
`tRESTClient`, `tExtractJSONFields`, `tMap`, `tPostgresqlOutput`

**Data Flow:**  
`API Request → JSON Parse → Transform → Enrich Master Data`

---

### 🕵️‍♀️ 4. **Fraud Detection Batch Pipeline**

**Goal:** Identify suspicious loan or payment transactions using ETL logic.

**Features:**
- Load daily transaction files.
- Apply fraud rules (duplicate PAN, same mobile across multiple accounts, etc.).
- Store flagged transactions for investigation.

**Talend Components Used:**  
`tFileInputDelimited`, `tFilterRow`, `tMap`, `tWarn`, `tLogRow`

**Data Flow:**  
`Transaction File → Rule-Based Filter → Flag → Output Report`

---

### 📊 5. **Payment Analytics & Dashboard ETL**

**Goal:** Build a clean dataset for payment performance analytics.

**Features:**
- Extract data from Payment Gateway & Core Loan Systems.
- Aggregate metrics such as Collection Rate, Bounce Rate, and DPD.
- Load data into a Reporting Layer (PostgreSQL).

**Talend Components Used:**  
`tDBInput`, `tAggregateRow`, `tSortRow`, `tPostgresqlOutput`

**Data Flow:**  
`Raw Payments → Aggregation → Reporting Database`

---

## 🧰 Tech Stack

| Category | Tools / Technologies |
|-----------|----------------------|
| **ETL Tool** | Talend Open Studio for Data Integration |
| **Data Sources** | CSV, Excel, REST APIs, MySQL, Oracle |
| **Data Targets** | PostgreSQL, Snowflake, AWS S3, Flat Files |
| **Data Modeling** | Star Schema, Snowflake Schema, SCD Type 2 |
| **Job Scheduling** | Talend Job Conductor / Windows Task Scheduler |
| **Domain Focus** | Banking & NBFC – Customer, Loan, Payment, Fraud, Credit Bureau |

---
## 🧱 Folder Structure

```bash
NBFC-Talend-Projects/
│
├── Customer360/
│   ├── Jobs/
│   ├── Datasets/
│   ├── Output/
│   └── Documentation/
│
├── LoanDisbursement/
│   ├── Jobs/
│   ├── SQLScripts/
│   └── Logs/
│
├── CreditBureauIntegration/
│   ├── Jobs/
│   ├── APIExamples/
│   └── SampleResponses/
│
├── FraudDetection/
│   ├── Jobs/
│   ├── RuleDefinitions/
│   └── Alerts/
│
└── PaymentAnalytics/
    ├── Jobs/
    ├── Reports/
    └── Output/

```

## 🧠 Learning Outcomes

- Designed **end-to-end ETL pipelines** for NBFC operational data.  
- Implemented **data quality validation** and **error-handling frameworks** in Talend.  
- Applied **SCD Type 2** logic for maintaining historical records.  
- Built **parameterized, reusable Talend jobs** for enterprise-grade data pipelines.

---

## 📬 Contact

**👨‍💻 Author:** Yogesh Salve  
**📩 Email:** yogeshbalkrishnasalve@gmail.com  
**🔗 LinkedIn:** [linkedin.com/in/yogeshsalve](https://www.linkedin.com/in/yogeshsalve/)  
**📦 GitHub:** [github.com/yogeshsalve](https://github.com/yogeshsalve)

---

> 💬 *"Transforming NBFC data pipelines with Talend — one ETL job at a time!"*





