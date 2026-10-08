# Hi, I'm Hannan Razalli 👋

**Design Engineer → Data Engineer** | 8+ Years Design Engineering Background | Based in Kuala Lumpur, Malaysia  
*Open to Data Engineering & Analytics Engineering Roles*

---

### 💡 About Me
I bring 8 years of design engineering in the rolling stock industry into **Data Engineering**. 

Transitioning into DE self-taught means my focus is entirely on demonstrable engineering standards:
- **Production-minded pipelines** built with clean code, modular design, and robust orchestration.
- **Data quality guardrails** using tests that catch schema drift and nulls before downstream consumption.
- **Pragmatic architecture decisions** driven by cost, performance, and scale rather than hype.

---

### 🛠️ Technical Stack

| Category | Tools & Technologies |
| :--- | :--- |
| **Languages** | `Python`, `SQL (PostgreSQL, MySQL)` |
| **Orchestration & Modeling** | `Apache Airflow (Astronomer)`, `dbt Core`, `Medallion Architecture`, `SCD Type 2`, `Incremental MERGE` |
| **Cloud & Storage** | `AWS (S3, Glue, Athena, IAM)`, `Google BigQuery` |
| **DevOps & CI/CD** | `Docker`, `Git`, `GitHub Actions` |
| **Currently Exploring** | `PySpark`, `Azure Databricks` *(Guided implementations)* |

---

### 📊 Featured Project

#### 🚀 [`assets-correlation-pipeline`](https://github.com/YOUR-USERNAME/assets-correlation-pipeline)
> **A daily batch pipeline tracking correlation across traditional & crypto assets to evaluate portfolio diversification.**

* **The Problem:** Are multi-asset holdings genuinely diversified, or do market shocks cause asset classes to lock step?
* **The Solution:** Automates daily ingestion of asset prices (Jan 2021–Present) across KLCI, S&P 500, Bitcoin, and Gold (GLD) to calculate a rolling 30-day correlation matrix.
* **Scale & Reliability:** Processes a 6,400+ row fact table with **20+ automated data quality checks** per run (~5 min total execution time).
* **Tech Stack:** `AWS S3` · `AWS Glue` · `AWS Athena` · `Apache Airflow` · `GitHub Actions`

<details>
<summary><b>📐 Architectural & Design Choices (Click to expand)</b></summary>

* **Serverless First:** Chose AWS Athena + S3 over a warehouse (e.g., Redshift/Snowflake) to eliminate idle cluster costs for low-frequency daily batches.
* **Batch Ingestion:** Financial markets settle daily; streaming infrastructure was deliberately omitted to minimize operational cost and complexity.
* **Hive Partitioning:** Structured S3 prefix paths per asset class to enable cost-effective partition pruning during Athena queries.
</details>

---

### 📜 Credentials & Professional Registrations
* 🎓 **Graduate Engineer** – Board of Engineers Malaysia (BEM)
* ☁️ **AWS re/Start Graduate** – Amazon Web Services
* ⏳ *In Progress:* AWS Certified Cloud Practitioner

---

### 📬 Connect with Me
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)]([https://linkedin.com/in/YOUR-LINKEDIN](https://www.linkedin.com/in/abdullah-hannan-razalli-085aa3141/))
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:a.hannanrazalli@gmail.com)
<!-- 
[![Portfolio](https://img.shields.io/badge/Portfolio-00C4CC?style=flat&logo=canva&logoColor=white)](https://hannan-da-porfolio.my.canva.site/de-portfolio-hannan-razalli)
-->
