<h1 align="center">Gaurav Singh</h1>

<p align="center">
  Senior Data Engineer &nbsp;·&nbsp; Azure Databricks &nbsp;·&nbsp; Hyderabad, India
</p>

<p align="center">
  <a href="mailto:gauravml247@gmail.com"><img src="https://img.shields.io/badge/Email-me-D14836?style=flat-square" alt="Email"></a>&nbsp;
  <a href="https://www.linkedin.com/in/analyticsingh/"><img src="https://img.shields.io/badge/LinkedIn-analyticsingh-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>&nbsp;
  <a href="https://github.com/databrickslabs/dqx/pull/1510"><img src="https://img.shields.io/badge/Databricks%20Labs%20DQX-contributor-FF3621?style=flat-square&logo=databricks&logoColor=white" alt="DQX contributor"></a>
</p>

<!-- One placeholder left: YOUR_EMAIL (appears twice). -->

Senior Data Engineer with 8+ years building production data platforms on Azure Databricks — PySpark, Delta Lake, Unity Catalog, Kafka, Airflow, Iceberg — across retail, pharma R&D, fintech and maritime shipping. Previously owned 200+ production pipelines processing 5+ TB/day behind real-time personalisation for 10M+ daily users. Contributor to [Databricks Labs DQX](https://github.com/databrickslabs/dqx).

Two founding-team stints, both acquired (Codejudge → Skuad Labs → Payoneer). I ship with Claude and Cursor in the loop, prefer config-driven frameworks over one-off jobs, and build privacy into the data layer rather than bolting it on.

## Open source

**Databricks Labs DQX — `is_geo_within_distance`** · [PR #1510](https://github.com/databrickslabs/dqx/pull/1510) · under review <!-- flip to "merged" when it lands -->

A row-level geofencing check for the DQX data-quality framework: flags points farther than *N* metres from a reference point using geodesic distance (`st_distancespheroid` on the WGS 84 ellipsoid) rather than planar degrees. Accepts WKT/WKB/EWKT/GeoJSON via `try_to_geometry`, mixes SRID 0 and 4326 safely, reports invalid and non-point geometries instead of failing, supports per-row distance expressions, and keeps null semantics consistent with the rest of the geo checks. Ships with unit, integration and performance tests, reference docs, and a fix to the existing geo relationship examples. Motivated by vessel-position geofencing in maritime shipping.

## Production work

<!-- Numbers below are the ones from your resumes — confirm each before publishing. -->

- **Eligibility 2.0 — config-driven PySpark rules framework** (Kroger / 84.51°). YAML-defined eligibility rules compiled into a multi-task Databricks Workflow, deployed with Asset Bundles and covered by pytest/BDD — new rules ship as config, not code. Cut dataset onboarding time by 40%. Presented at the KPM Tech Showcase.
- **Privacy Compliance Platform — GDPR/CCPA deletion at scale** (GSK Vaccines R&D). GraphFrames identity graph resolves a data subject's full footprint, then cascades PII deletion across Apache Iceberg tables. 99.4% SLA adherence.
- **Real-time personalisation data platform** (retail). 200+ Spark pipelines on a Medallion/Delta Lake architecture, 5+ TB/day, 10M+ daily users — 70% lower query latency, 35% fewer pipeline failures, 25% engagement uplift.
- **Data catalog RAG search.** OpenAI embeddings + LangChain over the internal data catalog on Databricks; reduced analyst dependency on engineering for ad-hoc discovery by 30%.
- **Platform automation.** SharePoint → Unity Catalog ingestion (Graph API + Auto Loader + `MERGE INTO`); Freshservice ↔ Databricks webhooks that turn job failures into tracked tickets automatically.
- **Payroll & compliance data platform** (Skuad Labs). 3+ TB/day of international payroll transactions across 150+ countries on AWS (S3, EMR, Redshift), with idempotent, reconciled loads.

Client work is proprietary — happy to walk through architecture and trade-offs on a call.

## Stack

| Area | Tools |
|---|---|
| **Platform** | Azure Databricks, Unity Catalog, Delta Lake (Medallion), Azure Data Factory, Microsoft Fabric / OneLake |
| **Processing** | PySpark, Spark SQL & tuning (Z-Ordering, partition pruning, broadcast joins), Apache Iceberg, GraphFrames, Auto Loader |
| **Streaming & orchestration** | Apache Kafka, Apache Airflow, Databricks Workflows |
| **Engineering** | Databricks Asset Bundles, Azure DevOps YAML CI/CD, Terraform, pytest + chispa (95%+ coverage) |
| **AI / LLM** | LangChain, OpenAI APIs (RAG); Claude and Cursor in the daily workflow |
| **Also** | Python, SQL, Oracle; AWS (S3, EMR, Redshift) from earlier roles |

## Experience

<!-- Add years to each line. -->
- **Stolt-Nielsen** — Senior Data Engineer, India Development Center (2026 – present)
- **Tech Mahindra** — Senior Data Engineer; clients: Kroger / 84.51°, GSK Vaccines R&D <!-- confirm you're cleared to name clients publicly -->
- **Skuad Labs** — founding team (acquired by Payoneer)
- **Codejudge** — founding team (Sequoia-backed; acquired by Skuad Labs)
- Earlier: production ETL for Equifax US's financial data platform

## Certifications & education

- Microsoft Certified: Azure Data Engineer Associate (DP-203) <!-- add Credly link -->
- Databricks Certified Professional Data Engineer <!-- add credential link -->
- PG Diploma in Data Science, IIIT Bangalore (2021) · B.Tech Civil Engineering, AKTU (2019)

## Now

- Contributing geospatial data-quality checks to DQX.
- Where I'm heading: AdTech and retail media — audience and identity resolution, data clean rooms, privacy-preserving measurement.
- Open to Senior / Lead Data Engineer roles on Azure + Databricks — Bangalore, Hyderabad or remote. <!-- visible to your current employer; soften or cut if needed -->

## Contact

Fastest is email: **gauravml247@gmail.com** — I reply within a day. LinkedIn works too: [linkedin.com/in/analyticsingh](https://www.linkedin.com/in/analyticsingh/).

<!-- Optional: add a cal.com or Calendly link so people can book 20 minutes directly. -->
