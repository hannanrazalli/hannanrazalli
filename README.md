# Abdullah Hannan Razalli

Aspiring Data Engineer · Kuala Lumpur, Malaysia · Open to work

I'm a design engineer with eight years in rolling stock, moving into data engineering. The move is self-taught and happens outside my day job, so I focus on building things I can show: pipelines that run, tests that catch problems, and decisions I can explain.

---

## Technical skills

- **Languages:** Python, SQL (PostgreSQL, MySQL)
- **Orchestration and transformation:** Apache Airflow (Astronomer), dbt Core
- **Cloud and storage:** AWS (S3, Glue, Athena, IAM), Google BigQuery
- **DevOps:** Docker, Git, GitHub Actions
- **Data modelling:** Medallion architecture, incremental loads and MERGE, SCD Type 2, late-arriving data
- **Learning:** PySpark and Azure Databricks (guided projects only, nothing production-like yet)

---

## Featured project

### [assets-correlation-pipeline](https://github.com/hannanrazalli/assets-correlation-pipeline)

A daily batch pipeline that tracks the KLCI, S&P 500, Bitcoin and gold (GLD) and calculates a 30-day rolling correlation between them. It answers one question: if you hold a mix of these assets, do they really move in different directions, or does it only feel diversified?

- Data from January 2021 to present, 6,409 rows in the fact table
- 20+ data quality checks, about 5 minutes per full run
- S3, Glue (crawler and Data Catalog), Athena, Airflow (Astronomer), GitHub Actions

**Design choices:** I went serverless because the data is small and a warehouse would sit idle. Ingestion is batch because the data lands once a day. Each asset class has its own S3 folder, which keeps Hive partitioning simple.

---

## Credentials

- AWS re/Start (completed)
- AWS Certified Cloud Practitioner (next)
- Graduate Engineer, Board of Engineers Malaysia (BEM)

---

## Contact

[LinkedIn](https://www.linkedin.com/in/abdullah-hannan-razalli-085aa3141/) · [Email](mailto:a.hannanrazalli@gmail.com)

<!-- Add back once the portfolio is finished:
 · [Portfolio](https://hannan-da-porfolio.my.canva.site/de-portfolio-hannan-razalli)
-->
