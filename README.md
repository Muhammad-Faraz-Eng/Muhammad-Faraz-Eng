# 💫 About Me

**Muhammad Faraz** — Data Engineer

Results-oriented Data Engineer with hands-on experience building **production-grade, end-to-end data pipelines** on Azure and AWS. I specialize in medallion architecture design, real-time streaming with Kafka and Azure Event Hubs, workflow orchestration with Apache Airflow, and data transformation with dbt. Passionate about configuration-driven pipeline design, data quality automation, and integrating AI/RAG capabilities into analytics platforms.

Currently contributing to production Kubernetes-deployed data infrastructure at **ExpertFlow**, where I work on Airflow-orchestrated ETL platforms, Docker image hardening, CVE remediation, and multi-database pipeline reliability.

---

## 🌐 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-faraz-410050319/)
[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:farazshokat6@gmail.com)

📱 **Phone:** 0321-7508045

---

## 🚀 Featured Projects

### 1. End-to-End Production Data Platform
**Stack:** Python · Apache Airflow · dbt · Azure Data Lake Storage · LangChain · Ollama · Docker · PostgreSQL

Designed and deployed a complete **Medallion Architecture (Bronze → Silver → Gold)** data platform ingesting from SQL Server and REST APIs.

- Built YAML-driven configuration system to eliminate hardcoding and enable extensibility for new data sources
- Developed automated schema validation framework with type casting, deduplication, and quarantine logic for invalid records — achieved **100% data quality compliance**
- Delivered a **star-schema warehouse** (4 fact/dimension tables) with 4 analytics dashboards
- Integrated **LangChain + Ollama RAG system** enabling natural language querying over the data platform

---

### 2. Uber End-to-End Data Engineering Project
**Stack:** Python · FastAPI · Azure Event Hubs · Faker · Jinja2 · Docker

Built a real-time ride data engineering platform simulating and streaming Uber ride events at scale.

- Engineered a data generation module producing realistic ride confirmations with dynamic pricing (base fare, distance, surge), 10+ US cities, and 5 vehicle types (UberX, UberXL, Comfort, Black, UberPOOL)
- Implemented **Azure Event Hubs streaming pipeline** for real-time ingestion enabling downstream analytics and ML workloads
- Built a **FastAPI** application as the pipeline interface with REST endpoints and Jinja2-templated web UI

---

### 3. RetailFlow – Config-Driven ETL Pipeline
**Stack:** Python · Apache Airflow · PostgreSQL · Apache Superset · Docker

Architected a modular, production-safe ETL system for retail analytics.

- Designed **Medallion Architecture** (Bronze/Silver/Gold) with OOP principles and YAML-driven config — new sources can be added with zero code changes
- Enforced **idempotent loads** using PostgreSQL UPSERT on business keys; orchestrated scheduling, retries, and dependencies with Airflow DAGs
- Integrated **Apache Superset** for real-time dashboards: Sales by Region, Revenue by Category, Daily Trends

---

### 4. E-commerce Fraud Detection Streaming Pipeline
**Stack:** Python · Apache Kafka · Apache Airflow · dbt · PostgreSQL · Docker Compose

Built a containerized, production-style streaming fraud detection pipeline.

- Developed Kafka producer/consumer apps to stream real-time transactions into PostgreSQL; coordinated by an Airflow DAG managing consumer launch, quality validation, and multi-layer dbt transformations as DockerOperator tasks
- Built a **3-layer dbt project**: Raw (JSON flattening) → Staging (incremental SCD Type 1 & 2) → Marts (dimensional model + fraud summary view)
- Fully containerized stack (Postgres, Zookeeper, Kafka, Airflow) via Docker Compose — **100% reproducible** across environments

---

### 5. ExpertFlow – Production Data Platform (cx-data-platform)
**Stack:** Apache Airflow 3.2.1 · Python 3.13 · Kubernetes · Helm · Docker · dbt-mysql · Debian 12

Production-grade Kubernetes-deployed data pipeline platform at ExpertFlow.

- Resolved **Kubernetes CrashLoopBackOff** failures in the Transflux data pipeline service (Helm 5.1.0) — root causes: incorrect MySQL client_flag in connection URLs and Airflow 3.x import path regressions
- Conducted **CVE remediation** using Grype/Trivy scans: pinned redshift-connector, asyncssh, idna to patched versions; produced architectural recommendations (multi-stage builds, distroless base images, pip-compile lock files)
- Fixed **DAG import failures** from wildcard import class shadowing, YAML template parsing bug, and SSL FileNotFoundError from empty MySQL cert secrets via ConfigMap rebuild
- Resolved **dbt-mysql 1.7.0 / dbt-core ≥1.9.0** version incompatibility using `--no-deps` with manual transitive dependency installation

---

## 🎓 Education

**Bachelor of Computer Science** — Superior University, Lahore, Pakistan

---

## 📜 Certifications

- PySpark – Apache Spark Programming *(Udemy)*
- Azure Databricks & Spark For Data Engineer *(Udemy)*

---

## 💻 Tech Stack

### ☁️ Cloud Platforms
![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)
![Azure Synapse](https://img.shields.io/badge/Azure%20Synapse-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Microsoft Fabric](https://img.shields.io/badge/Microsoft%20Fabric-0F6CBD?style=for-the-badge&logo=microsoft&logoColor=white)

### ⚙️ Data Processing & Orchestration
![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=Apache%20Airflow&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-FDEE21?style=for-the-badge&logo=apachespark&logoColor=black)
![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-000?style=for-the-badge&logo=apachekafka)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![AWS Glue](https://img.shields.io/badge/AWS%20Glue-4B9CD3?style=for-the-badge&logo=amazonaws&logoColor=white)

### 🗄️ Databases & Storage
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)

### 🐍 Languages
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Bash Script](https://img.shields.io/badge/bash_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

### 🐳 DevOps & Infrastructure
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

### 📊 Analytics & BI
![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

---

## 📊 GitHub Stats

![](https://github-readme-stats.vercel.app/api?username=Muhammad-Faraz-Eng&theme=dark&hide_border=false&include_all_commits=true&count_private=false)<br/>
![](https://nirzak-streak-stats.vercel.app/?user=Muhammad-Faraz-Eng&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=Muhammad-Faraz-Eng&theme=dark&hide_border=false&include_all_commits=true&count_private=false&layout=compact)

### ✍️ Random Dev Quote
![](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=radical)

---

[![](https://visitcount.itsvg.in/api?id=Muhammad-Faraz-Eng&icon=0&color=0)](https://visitcount.itsvg.in)
