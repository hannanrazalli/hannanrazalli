## Hi, I'm Hannan

Design engineer in rolling stock, eight years in, moving into data engineering. None of that move has come through my day job. I've taught myself, and the project below is where I'm trying to prove I can do the work properly.

Based in Kuala Lumpur. Open to data engineering roles and adjacent ones.

### Currently building

**[assets-correlation-pipeline](https://github.com/hannanrazalli/assets-correlation-pipeline)**: a daily batch pipeline that tracks the KLCI, S&P 500, Bitcoin and gold (GLD) and computes a 30-day rolling correlation between them. The question it answers: if you hold a mix of these, do they actually move in different directions, or does it just feel diversified?

History from January 2021, 6,409 rows in the fact table, 20+ data quality checks, about five minutes per run.

I went serverless (S3, Glue, Athena) because the data is small and a warehouse would sit idle. It's batch because the data lands once a day. Stocks, gold and Bitcoin each get their own S3 folder, because the data isn't shaped the same and it keeps the crawler from mixing schemas. Airflow (Astronomer) orchestrates it and GitHub Actions handles CI.

### Toolbox

**Use regularly:** Python, SQL (PostgreSQL, MySQL), Airflow, dbt Core, BigQuery, AWS (S3, Glue, Athena, IAM), Docker, Git, GitHub Actions
**Patterns:** Medallion architecture, incremental loads and MERGE, SCD Type 2, late-arriving data
**Still learning:** PySpark and Azure Databricks. Guided projects only so far, nothing production-like.

AWS re/Start completed. Cloud Practitioner next.

Outside work I do 3D design and printing.

[LinkedIn](https://www.linkedin.com/in/abdullah-hannan-razalli-085aa3141/) · [Email](mailto:a.hannanrazalli@gmail.com)

<!-- Add back once the portfolio is finished:
 · [Portfolio](https://hannan-da-porfolio.my.canva.site/de-portfolio-hannan-razalli)
-->
