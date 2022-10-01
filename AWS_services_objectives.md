***AWS Services and it's objectives***

Organized by technology

Table of content:
- [**Analytics**](#analytics)
  - [**Athena:**](#athena)
  - [**Amazon EMR**](#amazon-emr)
  - [**AWS Glue**](#aws-glue)
  - [**Amazon Kinesis services**](#amazon-kinesis-services)
  - [**Amazon Quicksight**](#amazon-quicksight)
  - [**Amazon Redshift**](#amazon-redshift)
  - [**AWS Glue DataBrew**](#aws-glue-databrew)
  - [**CloudSearch**](#cloudsearch)
  - [**AWS Data Exchange**](#aws-data-exchange)
  - [**Data Pipeline**](#data-pipeline)
  - [**Amazon FinSpace**](#amazon-finspace)
  - [**AWS Lake Formation**](#aws-lake-formation)
  - [**MSK**](#msk)
  - [**Amazon OpenSearch Service**](#amazon-opensearch-service)

---

# **Analytics**
  
## **Athena:**

Amazon Athena is an interactive query service that makes ir easy to analyze data in Amazon S3 and other federated data sources using standard SQL.

*Benefits and features:*

**Start Querying now:** 
Athena is serverless. 

**Powerful:** 
Athena is ideal for quick, ad-hoc querying, but it can also handle complex analysis, including large joins, window functions, and arrays.

**Cost effective:**
Athena charges only for data scanned. Athena relies on Amazon S3 and the AWS Glues data catalog, separate charges apply.

**Fast:**
Athena automatically executes queries in parallel, so most results come back within seconds.

*Use cases*

**Query AWS service logs:**
Use Athena to query logs for service and application troubleshooting, performance analysis, and security audits.

**Query from any data source:**
Federated query is a new Athena feature that executes SQL queries across data stored in relational, non-relational, object, and custom sources.

**Extract, Transform and Load data into S3 data lake:**
Use Athena for extract, transform and load (ETL) jobs for data processing.

**Model-training and invoking machine learning models:**
Athena provides an easy way to run inference using machine learning (ML) models deployed on Amazon SageMaker directly from SQL queries.

*Related Services*

**Amazon QuickSight:**
Use Athena to generate reports or explore data with business intelligence tools or SQL clients connected with a JDBC or an ODBC driver.

**AWS Glue:**
Create tables and query data in Athena based on a central metadata store with the ETL and data discovery features of AWS Glue.

---

## **Amazon EMR**

Easily run and scale **Apache Spark**, **Hive**, **Presto**, and other big data workloads

**How it works:**
Amazon EMR is the industry-leading cloud big data solution for **petabyte-scale** data processing, interactive analytics, and machine learning using open-source frameworks such as Apache Spark, Hive and Presto.

**Use cases**

**Perform big data analytics:**
Run large-scale data processing and what-if analysis using statistical algorithms and predictive models to uncover hidden patterns, correlations, market trends, and customer preferences.

**Build scalable data pipelines:**
Extract data from a variety of sources, process it at scale, and make it available for applications and users.

**Process real-time data streams:**
Analyze events from streaming data sources in real-time to create long-running, highly-available, and fault-tolerant streaming data pipelines.

**Accelerate data science and ML adoption:**
Analyze data using ope-source ML frameworks such as Apache Spark MLlib, TensorFlow, and Apache MXNet. Connect to Amazon SageMaker Studio for large-scale model training, analysis, and reporting.

---

## **AWS Glue**

**Serverless data integration:**
Move datasets of nearly any size and prepare them for analytics and machine learning. AWS Glue has data integration tools for every skillset and manages all the infrastructure.

**Benefits and features**

**AWS Glue Data Catalog:**
Track your data assets and make them accessible from your analytics tools of choice.

**Job management:**
Edit, clone, and monitor your ETL jobs.

**Code-based job authoring:**
Write your own code for Apache Spark and Python Shell ETL and data integration jobs.

**Connectors:**
Read and write to dozens of supported data stores and build custom connectors.

**Crawlers for data discovery:**
Automatically detect the schema and structure of your data and add it to the AWS Glue Data Catalog.

**Visual job authoring:**
Author ETL and data integration jobs in a no-code interface and/or with SQL-based transformations.

**Job run and resource monitoring:**
Track job run completion and success, monitor resource usage, and debug issues.

**AWS Glue DataBrew:**
Visualize, clean, and normalize data without writing any code.

---

## **Amazon Kinesis services**

Collect, process, and analyze data streams in real time.

**Kinesis Data Streams**

**Collect and store data streams:**
Collect gigabytes of data per second and make it available for processing and analyzing in real time.

**Real-time data capture:**
Ingest and store data streams from hundreds of thousands of data sources:
 - Log and event data collection
 - IoT device data capture
 - Mobile data collection
 - Gaming data feed

**Kinesis Data Firehose**

**Process and deliver data streams:**
Prepare and load real-time data streams into data stores and analytics tools.

**Load real-time data:**
Load streaming data into data lakes, data stores, and analytics tools for:
 - Log and event analytics
 - IoT data analytics
 - Clickstream analytics
 - Security monitoring

**Kinesis Data Analytics**

**Analyze streaming data:**
Get actionable insights from streaming data in real time.

**Get insights in real time:**
Analyze streaming data and gain actionable insights in real time:
 - Real-time streaming ETL
 - Real-time log analytics
 - Ad tech and digital marketing analytics
 - Real-time IoT device monitoring

**Use Cases**

**Solution Implementation - AWS Streaming Data Solution for Amazon Kinesis**

The AWS Streaming Data Solution for Amazon Kinesis helps developers more easily configure the core AWS services necessary to capture, store, process, and deliver streaming data by offering two AWS CloudFormation templates. One option is designed to capture data from non-AWS environments such as mobile clients, enable throttling at the API level, and leverage AWS Lambda to handle errors for Amazon Kinesis streams. The second option leverages Apache Flink and provides a fully managed service to handle backups automatically. This option also supports the Amazon Kinesis Producer Library (KPL).

**Evolve from Batch to Real-Time Analytics**

With Amazon Kinesis services, you can perform real-time analytics on data that has been traditionally analyzed using batch processing. Common streaming use cases include sharing data between different applications, streaming extract-transform-load, and real-time analytics. For example, you can use Kinesis Data Firehose to continuously load streaming data into your S3 data lake or analytics services.

**Build Real-Time Analytics**

You can use Amazon Kinesis services for real-time application monitoring, fraud detection, and live leader-boards. You can ingest streaming data using Kinesis Data Streams, process it using Kinesis Data Analytics, and emit the results to any data store or application using Kinesis Data Streams with millisecond end-to-end latency. Learn about what your customers, applications, and products are doing right now and react promptly.

**Analyze IoT Device Data**

You can use Amazon Kinesis services to process streaming data from IoT devices such as consumer appliances, embedded sensors, and TV set-top boxes. You can then use the data to send real-time alerts or take other actions programmatically when a sensor exceeds certain operating thresholds. To build your application, you can use our sample IoT analysis code. 

---

## **Amazon Quicksight**

**The most popular cloud-native, serverless BI service**

Amazon QuickSight allows everyone in your organization to understand your data by asking questions in natural language, exploring through interactive dashboards, or automatically looking for patterns and outliers powered by machine learning.

QuickSight powers millions of dashboard views weekly for customers, allowing their end-users to make better data-driven decisions.

**Key features**

**Enable BI for everyone with QuickSight Q**

Ask conversational questions of your data and use Q’s ML-powered engine to receive relevant visualizations without the time consuming data preparation from authors and admins. 

**Perform advanced analytics with ML insights**

Discover hidden insights from your data, perform accurate forecasting and what-if analysis, or add easy-to-understand natural language narratives to dashboards by leveraging AWS' expertise in machine learning.

**Embed analytics to differentiate your applications**

Easily embed interactive visualizations and dashboards, sophisticated dashboard authoring, or natural language query capabilities in your applications to differentiate user experience and unlock new monetization opportunities.

**Benefits**

**Connect and scale all of your data**

Connect to all your data in AWS, 3rd party clouds, or on-premises
SPICE in-memory storage to scale data exploration to thousands of users
Combine data from multiple sources and create complex data models for governed data sharing

**Build customizable dashboards**

Pixel-perfect dashboard design for customized, use-case specific dashboards
Deliver personalized email reports and alerts for end-users
On-the-go access using QuickSight’s iOS, Android, or mobile web access

**Leverage ML integrations for insights**

Anomaly Detection to continuously analyze all of your data for anomalies and variations
Forecast business metrics and perform interactive what-if analysis with point-and-click
Auto-Narratives that can be customized and woven into dashboards for deeper context for users

**Enable true self-service BI for everyone**

Q enables end-users to dive deep into data through simple questions without BI training
Easy visual analysis of data using QuickSight’s 100% web-based authoring interface
Embed QuickSight capabilities in applications for data-driven user experiences

**Native AWS services integrations**

Private VPC connectivity for secure AWS access to Amazon Redshift, Snowflake, Exasol,
Amazon RDS and more
Native IAM permissions for Amazon S3 and Amazon Athena with fine-grained access
control for serverless data exploration
Amazon SageMaker integration allows easy integration of sophisticated ML models
without complex data pipelines

**No servers to manage, pay by usage**

Serverless architecture auto-scales to hundreds of thousands of users with high availability; no need to over-provision for peak usage
SPICE in-memory engine auto-scales to provide consistent fast response times for end-users and analysts; no need to scale databases for high workloads
Pay-per-session optimizes costs by only paying for actual usage; no need to buy thousands of end-user licenses for large-scale BI or embedded analytics

---

## **Amazon Redshift**

**Accelerate your time to insights with fast, easy, and secure analytics at scale.**

Amazon Redshift makes it easier for you to run and scale analytics without having to manage your data warehouse. Get insights by running real-time and predictive analytics on all of your data, across operational databases, data lake, data warehouse, and thousands of third-party datasets.

**Provision and manage clusters**

With a few clicks, you can create your first Amazon Redshift provisioned cluster in minutes.

**Use cases**

**Accelerate all your analytics workloads**

Use Amazon Redshift to get sub-second results for reports, dashboards, and interactive analysis, and to get fast results for complex queries on any scale of data.

**Modernize your on-premises data warehouse**

Modernize your on premises data warehouse to a fast, scalable, easy to manage, and cost-effective cloud data warehouse running on Amazon Redshift.

**Unified data warehouse and data lake**

Unlock insights with Amazon Redshift by running queries across your data warehouse and data lake.

---

## **AWS Glue DataBrew**

**Clean and normalize data up to 80% faster**

AWS Glue DataBrew is a visual data preparation tool that enables users to clean and normalize data without writing any code, to reduce the time it takes to prepare data for analytics and machine learning (ML) by up to 80% compared to today’s conventional, code-based data preparation. You can choose from over 250 pre-built transformations to automate data preparation tasks, such as filtering anomalies, converting data to standard formats, and correcting invalid values, all without the need to write code.

---

## **CloudSearch**

Managed Search Service

---

## **AWS Data Exchange**

Easily exchange data in the cloud

---

## **Data Pipeline**

Orchestration for Data-Driven Workflows

---

## **Amazon FinSpace**

Store, catalog, prepare, and analyze financial industry data

---

## **AWS Lake Formation**

AWS Lake Formation makes it easy to set up a secure data lake

---

## **MSK**

Fully managed, highly available, and secure service for Apache Kafka

---

## **Amazon OpenSearch Service**

Run and Scale OpenSearch and Elasticsearch Clusters (successor to Amazon Elasticsearch Service)