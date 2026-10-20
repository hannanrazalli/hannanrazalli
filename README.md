# Hannan Razalli

**Data Engineering & Analytics Engineering · Kuala Lumpur, Malaysia**

Design engineer transitioning into data engineering, with experience in rail design and precision manufacturing. I build independent data pipeline projects using Python, SQL, Airflow, dbt and AWS. Open to Data Engineering and Analytics Engineering opportunities.

[LinkedIn](https://www.linkedin.com/in/abdullah-hannan-razalli-085aa3141/) · [Email](mailto:a.hannanrazalli@gmail.com)

## Featured projects

### Multi-Asset Correlation Pipeline

Two implementations of the same daily batch pipeline for equity indices, Bitcoin, a gold ETF and USD/MYR exchange rates, with SQL models for returns and rolling correlations over 30 shared observations.

#### [Athena implementation →](https://github.com/hannanrazalli/assets-correlation-pipeline)

- **Pipeline:** Python → S3 → Glue crawlers and Data Catalog → dbt on Athena, orchestrated with Airflow.
- **Modeling:** Incremental Apache Iceberg fact table with MERGE, plus returns and correlation views.
- **Engineering:** 36 configured dbt tests; GitHub Actions for linting, DAG import checks, dbt parsing and EC2 deployment. Airflow runs through Astro and Docker.

#### [Redshift implementation →](https://github.com/hannanrazalli/assets-correlation-pipeline-redshift)

- **Pipeline:** Python → S3 → Redshift COPY → dbt on Redshift, orchestrated with Airflow.
- **Modeling:** Incremental Redshift fact table with MERGE, plus materialized returns, correlation and reporting tables.
- **Engineering:** 36 configured dbt tests; S3 file checks before COPY; Astro and Docker runtime with EC2 as the deployment host. CI/CD is planned.

Both repositories document architecture, setup, pipeline behaviour and analytical limitations. Test counts describe configured checks.

## Core stack

**Languages:** Python · SQL  
**Data platforms:** Airflow · dbt Core · AWS S3, Glue, Athena, Redshift  
**Development & deployment:** Docker · Astro CLI · Git · GitHub Actions · AWS EC2
