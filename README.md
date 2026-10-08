## Hi, I'm Hannan

I'm a design engineer in rolling stock, eight years in, working on locomotive projects. I'm moving into data engineering, and none of that move has happened through my day job. Everything below I've taught myself, and the pipeline project is where I'm trying to show I can do the work properly.

Based in Kuala Lumpur. Open to data engineering roles and adjacent ones.

<br>

### What I'm building right now

**[assets-correlation-pipeline](https://github.com/hannanrazalli/assets-correlation-pipeline)**

A daily batch pipeline that tracks four assets: the KLCI, the S&P 500, Bitcoin and gold (via GLD), with FX rates from Frankfurter. It computes a 30-day rolling correlation between them, to answer a simple question: if you hold a mix of these, do they actually move in different directions, or does it just feel diversified?

- History goes back to 1 January 2021
- A full run takes about five minutes
- 20+ data quality checks

Some of the decisions behind it:

- **S3 + Glue (crawler and Data Catalog) + Athena.** The data is small, so a serverless setup makes more sense than paying for a warehouse that sits idle most of the day.
- **Batch, not streaming.** The data arrives once a day. Streaming would add moving parts without solving any real problem here.
- **Separate S3 folders for stocks, gold and Bitcoin**, even though they come from the same source. The data isn't shaped the same, and splitting them keeps the crawler from mixing schemas and makes Hive-style partitioning easier.
- **Airflow on Astronomer** for orchestration, with **GitHub Actions** for CI.

Most of what has gone wrong so far has been my own code. Fixing it has taught me more than any tutorial did.

<br>

### Toolbox

**What I use and can build with:**
Python, SQL (PostgreSQL, MySQL), Apache Airflow (Astronomer), dbt Core, BigQuery, AWS (S3, Glue, Athena, IAM), Docker, Git, GitHub Actions

**Patterns I've worked with:**
Medallion architecture, incremental loads and MERGE, SCD Type 2, late-arriving data

**Still learning:**
PySpark and Azure Databricks. I've done guided projects but nothing production-like yet, and I'd rather say so than pad the list.

<br>

### Certifications

- AWS re/Start, completed
- AWS Certified Cloud Practitioner, next up
- Graduate Engineer, Board of Engineers Malaysia (BEM)

<br>

### Outside work

3D design and printing. It's the engineering habit I never dropped.

<br>

### Contact

[LinkedIn](https://www.linkedin.com/in/abdullah-hannan-razalli-085aa3141/) · [Email](mailto:a.hannanrazalli@gmail.com)

<!-- Add this line back once the portfolio is finished:
 · [Portfolio](https://hannan-da-porfolio.my.canva.site/de-portfolio-hannan-razalli)
-->
