# Hannan Razalli

**Data Engineering & Analytics Engineering · Kuala Lumpur, Malaysia**

Design engineer transitioning into data engineering, bringing 8+ years of experience in the rolling stock industry. I build data pipelines with Python, SQL, Airflow, dbt and AWS. Open to Data Engineering and Analytics Engineering roles.

[LinkedIn](https://www.linkedin.com/in/abdullah-hannan-razalli-085aa3141/) · [Email](mailto:a.hannanrazalli@gmail.com)

## Featured projects

### Multi-Asset Correlation Pipeline

Two implementations of the same daily batch pipeline: ingest equity, Bitcoin, gold ETF and FX data, convert prices to MYR, and compare asset returns across 30 shared observations.

#### [Athena implementation →](https://github.com/hannanrazalli/assets-correlation-pipeline)

- **Pipeline:** Python → S3 → Glue crawlers and Data Catalog → dbt on Athena, orchestrated with Airflow.
- **Modeling:** Incremental Apache Iceberg fact table with MERGE, plus returns and correlation views.
- **Engineering:** 32 configured dbt tests; GitHub Actions for linting, DAG import checks, dbt parsing and EC2 deployment. Airflow runs through Astro and Docker.

#### [Redshift implementation →](https://github.com/hannanrazalli/assets-correlation-pipeline-redshift)

- **Pipeline:** Python → S3 → Redshift COPY → dbt on Redshift, orchestrated with Airflow.
- **Modeling:** Incremental Redshift fact table with MERGE, plus materialized returns, correlation and reporting tables.
- **Engineering:** 36 configured dbt tests; S3 file checks before COPY; Astro and Docker runtime with EC2 as the deployment host. CI/CD is planned.

Both repositories document architecture, setup, pipeline behaviour and analytical limitations. Test counts describe configured checks.

## Core stack

**Languages:** Python · SQL (PostgreSQL, MySQL, Redshift)  
**Data platforms:** Airflow · dbt Core · AWS S3, Glue, Athena, Redshift · BigQuery  
**Development & deployment:** Docker · Astro CLI · Git · GitHub Actions · AWS EC2

## Background

8+ years in rolling stock design engineering · Graduate Engineer, Board of Engineers Malaysia (BEM) · AWS re/Start graduate
