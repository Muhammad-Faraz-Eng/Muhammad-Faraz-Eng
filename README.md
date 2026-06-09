# 💫 About Me

**Muhammad Faraz** — Data Engineer

Results-oriented Data Engineer with hands-on experience building **production-grade, end-to-end data pipelines** on Azure and AWS. I specialize in medallion architecture design, real-time streaming with PySpark and Azure Event Hubs, workflow orchestration with Apache Airflow, cloud ETL with Azure Data Factory and AWS Glue, and data transformation with dbt. Passionate about configuration-driven pipeline design, data quality at scale, and integrating AI/RAG capabilities into analytics platforms.

Currently contributing to production Kubernetes-deployed data infrastructure at **ExpertFlow**, working on Airflow-orchestrated ETL platforms, Docker image hardening, CVE remediation, and multi-database pipeline reliability.

---

## 🌐 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-faraz-410050319/)
[![Email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:muhammadfarazeng@gmail.com)

📱 **Phone:** 0321-7508045

---

## 🚀 Featured Projects

### 1. [Databricks-DBT End-to-End Data Engineering](https://github.com/Muhammad-Faraz-Eng/Databricks-DBT-End-to-End-Data-Engineering-Project)
**Stack:** PySpark · Databricks · dbt · Delta Lake · Unity Catalog · Azure Data Lake Storage · Autoloader

Built a complete **Medallion Architecture (Bronze → Silver → Gold)** pipeline using PySpark Streaming and Databricks Autoloader.

- Autoloader automatically detects and ingests new files from multiple sources; Bronze layer stores raw data as-is
- Silver layer enforces data quality (deduplication, type fixing, calculated fields); Gold layer implements dbt star schema with **SCD Type 2** for full historical tracking when source data changes
- Databricks **Unity Catalog** provides data governance and lineage documentation; automated scheduling delivers production-ready analytics datasets

---

### 2. [RetailPulse – Full-Stack Data Platform](https://github.com/Muhammad-Faraz-Eng/RetailPulse-End-to-End-Medallion-Data-Engineering-Pipeline-ADF-dbt-Airflow-RAG-)
**Stack:** Python · Azure Data Factory · Apache Airflow · dbt · Azure Data Lake Storage · Azure SQL · Metabase · LangChain · Ollama

A complete retail data platform from ingestion to AI-powered querying.

- YAML-config-driven Bronze ingestion via **Azure Data Factory** with schema validation, Parquet storage in ADLS, and quarantine logic for bad records
- Silver layer cleans and standardizes; Gold layer uses **dbt star schema** (fct_sales, dim_products, dim_stores); **Apache Airflow** orchestrates the full DAG with retries and failure alerts
- Delivered **4 Metabase dashboards** (Sales Overview, Product Analytics, Store Performance, Currency Insights)
- Integrated **LangChain + Ollama RAG** system enabling plain-English business queries at zero API cost (local model)

---

### 3. [Real-Time Healthcare Data Engineering Pipeline](https://github.com/Muhammad-Faraz-Eng/End-to-End-Real-Time-Healthcare-Data-Engineering-Pipeline)
**Stack:** Python · Azure Event Hubs · Databricks · PySpark Streaming · Azure Synapse Analytics · Power BI · SCD Type 2

Real-time patient flow tracking system with instant dashboard updates.

- Python generates patient flow events (arrival, ER transfer, ICU admission) → **Azure Event Hubs** → **Databricks PySpark Streaming** processes Bronze/Silver/Gold layers instantly
- **SCD Type 2** preserves full patient movement history; **Azure Synapse Analytics** star schema (fct_patient_events, dim_departments, dim_doctors, dim_patient_info) powers complex analytics
- **Power BI dashboards** refreshing every minute: live patient locations, department capacity, wait times, and flow trends — enabling proactive capacity planning

---

### 4. [AWS Glue ETL Pipeline – Masterclass](https://github.com/Muhammad-Faraz-Eng/AWS-Glue-Masterclass-2026-End-to-End-ETL-Pipeline)
**Stack:** AWS Glue · Amazon S3 · PySpark · AWS Glue Data Catalog · Parquet · Event-Driven Triggers · CTAS

End-to-end AWS-native ETL platform with automated, event-driven processing.

- Architected a **3-layer S3 data lake** (Raw / Processed / Analytics) with date-and-region partitioning; built **Glue Data Catalog** documenting all datasets and column metadata for company-wide discoverability
- PySpark ETL scripts handle null removal, type fixing, joins, and Parquet output; **CTAS** and external table patterns for SQL-based transformations
- Event-driven **S3 triggers** fire ETL automatically on new file arrival — zero manual intervention, pay-per-minute Glue pricing for cost-efficient batch workloads

---

### 5. ExpertFlow – Production Data Platform (Job Role Contribution)
**Stack:** Apache Airflow 3.2.1 · Python 3.13 · Kubernetes · Helm · ConfigMaps · Docker · dbt-mysql · GitLab CI · Trivy · Grype

Production-grade Kubernetes-deployed data pipeline platform at ExpertFlow.

- **Kubernetes & Helm:** Deployed and maintained the Transflux data platform on Kubernetes (`expertflow` namespace, Helm 5.1.0); debugged CrashLoopBackOff failures by tracing pod logs and container exit codes, identifying and correcting an incorrect MySQL `client_flag` in connection URLs and a misconfigured Helm values override
- **ConfigMap Debugging:** Rebuilt ConfigMaps to resolve an SSL `FileNotFoundError` caused by empty MySQL certificate secret mounts; authored `sed`-based fixes across config templates to inject correct certificate paths at pod runtime, eliminating SSL failures across all replicas
- **Platform Migration:** Led migration from Airflow 2.x to **Airflow 3.2.1** on Python 3.13 / Debian 12; updated deprecated import paths, resolved DB schema incompatibilities, fixed DAG import failures from wildcard import class shadowing, and patched a YAML template parsing bug with a runtime `isinstance` guard
- **Security (Trivy & Grype in GitLab CI):** Integrated container vulnerability scans into the GitLab CI pipeline; triaged reports, pinned redshift-connector, asyncssh, and idna to patched versions, added suppression entries for accepted-risk CVEs; produced a hardening report recommending multi-stage Docker builds, distroless base images, and pip-compile lock files
- **dbt Compatibility:** Resolved dbt-mysql 1.7.0 / dbt-core ≥1.9.0 version incompatibility using `--no-deps` with manual transitive dependency resolution, restoring the full dbt transformation pipeline

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
![Azure Data Factory](https://img.shields.io/badge/Azure%20Data%20Factory-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

### 🗄️ Databases & Storage
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-FF9900?style=for-the-badge&logo=amazons3&logoColor=white)

### 🐍 Languages
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![Bash Script](https://img.shields.io/badge/bash_script-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

### 🐳 DevOps & Infrastructure
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab%20CI-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white)
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
