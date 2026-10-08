# Abdullah Hannan Razalli

**Aspiring Data Engineer** · Kuala Lumpur, Malaysia · Open to work

I'm a design engineer with eight years in rolling stock, moving into data engineering. The move is self-taught and happening outside my day job, so I focus on building things I can show: pipelines that run, tests that catch problems, and decisions I can explain.

<br>

## Featured project

### [assets-correlation-pipeline](https://github.com/hannanrazalli/assets-correlation-pipeline)

A daily batch pipeline that tracks the KLCI, S&P 500, Bitcoin and gold (GLD) and calculates a 30-day rolling correlation between them. It answers one question: if you hold a mix of these assets, do they really move in different directions, or does it only feel diversified?

| | |
|---|---|
| **History** | January 2021 to present |
| **Fact table** | 6,409 rows |
| **Data quality checks** | 20+ |
| **Run time** | About 5 minutes |
| **Stack** | S3, Glue (crawler, Data Catalog), Athena, Airflow (Astronomer), GitHub Actions |

**Why I built it this way**

- **Serverless (S3, Glue, Athena):** the data is small, so a warehouse would sit idle and cost more for no benefit.
- **Batch ingestion:** the data lands once a day, so streaming would only add complexity.
- **Separate S3 folders per asset class:** the data isn't shaped the same, and separating it keeps the crawler from mixing schemas and makes Hive partitioning simpler.

<br>

## Skills

| | |
|---|---|
| **Use regularly** | Python, SQL (PostgreSQL, MySQL), Airflow, dbt Core, BigQuery, AWS (S3, Glue, Athena, IAM), Docker, Git, GitHub Actions |
| **Patterns** | Medallion architecture, incremental loads and MERGE, SCD Type 2, late-arriving data |
| **Learning** | PySpark, Azure Databricks (guided projects only, nothing production-like yet) |

<br>

## Credentials

AWS re/Start (completed) · AWS Certified Cloud Practitioner (next) · Graduate Engineer, BEM

<br>

## Beyond work

I design and 3D print things in my spare time.

<br>

## Get in touch

[LinkedIn](https://www.linkedin.com/in/abdullah-hannan-razalli-085aa3141/) · [Email](mailto:a.hannanrazalli@gmail.com)

<!-- Add back once the portfolio is finished:
 · [Portfolio](https://hannan-da-porfolio.my.canva.site/de-portfolio-hannan-razalli)
-->
