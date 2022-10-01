***AWS Services and it's objectives***

Organized by technology

Table of content:
- [**Analytics**](#analytics)
  - [**Athena:**](#athena)
  - [**Amazon EMR**](#amazon-emr)

---

# **Analytics**
  
## **Athena:**

Amazon Athena is an interactive query service that makes ir easy to analyze data in Amazon S3 and other federated data sources using standard SQL.

*Benefits and features:*

Start Querying now: 
Athena is serverless. 
Powerful: 
Athena is ideal for quick, ad-hoc querying, but it can also handle complex analysis, including large joins, window functions, and arrays.
Cost effective:
Athena charges only for data scanned. Athena relies on Amazon S3 and the AWS Glues data catalog, separate charges apply.
Fast:
Athena automatically executes queries in parallel, so most results come back within seconds.

*Use cases*

Query AWS service logs:
Use Athena to query logs for service and application troubleshooting, performance analysis, and security audits.
Query from any data source:
Federated query is a new Athena feature that executes SQL queries across data stored in relational, non-relational, object, and custom sources.
Extract, Transform and Load data into S3 data lake:
Use Athena for extract, transform and load (ETL) jobs for data processing.
Model-training and invoking machine learning models:
Athena provides an easy way to run inference using machine learning (ML) models deployed on Amazon SageMaker directly from SQL queries.

*Related Services*

Amazon QuickSight:
Use Athena to generate reports or explore data with business intelligence tools or SQL clients connected with a JDBC or an ODBC driver.

AWS Glue:
Create tables and query data in Athena based on a central metadata store with the ETL and data discovery features of AWS Glue.

---

## **Amazon EMR**

Easily run and scale **Apache Spark**, **Hive**, **Presto**, and other big data workloads

How it works:
Amazon EMR is the industry-leading cloud big data solution for **petabyte-scale** data processing, interactive analytics, and machine learning using open-source frameworks such as Apache Spark, Hive and Presto.

**Use cases**

Perform big data analytics:
Run large-scale data processing and what-if analysis using statistical algorithms and predictive models to uncover hidden patterns, correlations, market trends, and customer preferences.

Build scalable data pipelines:
Extract data from a variety of sources, process it at scale, and make it available for applications and users.

Process real-time data streams:
Analyze events from streaming data sources in real-time to create long-running, highly-available, and fault-tolerant streaming data pipelines.

Accelerate data science and ML adoption:
Analyze data using ope-source ML frameworks such as Apache Spark MLlib, TensorFlow, and Apache MXNet. Connect to Amazon SageMaker Studio for large-scale model training, analysis, and reporting.

---

##