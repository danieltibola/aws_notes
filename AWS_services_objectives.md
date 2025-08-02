# ***AWS Services and it's objectives***

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
- [**Application Integration**](#application-integration)
  - [**Amazon EventBridge**](#amazon-eventbridge)
  - [**Simple Notification Service (SNS)**](#simple-notification-service-sns)
  - [**Simple Queue Service (SQS)**](#simple-queue-service-sqs)
  - [**Step Functions**](#step-functions)
  - [**Amazon AppFlow**](#amazon-appflow)
  - [**Managed Apache Airflow**](#managed-apache-airflow)
  - [**Amazon MQ**](#amazon-mq)
  - [**SWF**](#swf)
- [**AR & VR**](#ar--vr)
  - [**Amazon Sumerian**](#amazon-sumerian)
- [**AWS Cost Management**](#aws-cost-management)
  - [**AWS Budgets**](#aws-budgets)
  - [**Cost Explorer**](#cost-explorer)
  - [**AWS Application Cost Profiler**](#aws-application-cost-profiler)
  - [**AWS Billing Conductor**](#aws-billing-conductor)
  - [**AWS Marketplace Subscriptions**](#aws-marketplace-subscriptions)
- [**Blockchain**](#blockchain)
  - [**Amazon Managed Blockchain**](#amazon-managed-blockchain)
- [**Business Applications**](#business-applications)
  - [**Alexa for Business**](#alexa-for-business)
  - [**Amazon Chime**](#amazon-chime)
  - [**Amazon Connect**](#amazon-connect)
  - [**Amazon Honeycode**](#amazon-honeycode)
  - [**Amazon Pinpoint**](#amazon-pinpoint)
  - [**Amazon Simple Email Service**](#amazon-simple-email-service)
  - [**Amazon WorkDocs**](#amazon-workdocs)
  - [**Amazon WorkMail**](#amazon-workmail)

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

---

# **Application Integration**

## **Amazon EventBridge**

**Build event-driven applications at scale**

Amazon EventBridge is a serverless event bus that makes it easier to build event-driven applications at scale using events generated from your applications, integrated Software-as-a-Service (SaaS) applications, and AWS services.

**Benefits and features**

**Build event-driven architectures**

EventBridge simplifies the process of building event-driven architectures. With EventBridge, your event targets don’t need to be aware of event sources because you can filter and publish directly to EventBridge. There is no setup required. Improve developer agility as well as application resiliency with loosely coupled event-driven architectures.

**Connect SaaS apps**

EventBridge ingests data from supported SaaS applications and routes it to AWS services and SaaS targets (through API destinations - an HTTP invocation endpoint target for events) without writing custom integration code. You can use EventBridge to connect your SaaS apps, or use events from your SaaS apps to trigger workflows.

**Write less custom code**

EventBridge makes it easier to connect applications. You can ingest, filter, transform and deliver events without writing custom code. The EventBridge schema registry stores a collection of easy-to-find event schemas and enables you to download code bindings for those schemas in your IDE so you can represent the event as a strongly-typed object in your code. Automatically add schemas discovered from your event bus to the registry through the schema discovery feature.

**Reduce operational overhead**

With EventBridge, there are no servers to provision, patch, and manage. EventBridge automatically scales based on the number of events ingested, and you pay only for events published by your AWS or SaaS applications. EventBridge has built-in distributed availability, fault-tolerance and a native event archive and replay capability that makes it easier to recover from failures or build a new application state from old events.

**Use cases**

**Re-architect for speed**

Use EventBridge to accelerate modernizing and re-designing your architecture with decoupled services and applications. With EventBridge, there is no need for heavy coordination between event producer and consumer applications or services. You can speed up your organization’s development process by allowing teams to iterate on features without explicit dependencies between systems.

**Monitoring and auditing**

You can monitor and audit your AWS environments and respond to operational changes in your applications in real-time to prevent infrastructure vulnerabilities. For example, when your resources are accessed by cross-accounts or public accounts, you can configure an Amazon Access Analyzer event to be generated and sent to an AWS Lambda Function using EventBridge to remove the unintended permissions.

**Extend functionality via SaaS integrations**

You can extend the functionality of your applications by easily connecting them to other SaaS applications via EventBridge. For example, you can send custom events to EventBridge when a new user has been created in a free tier and send that event via API Destinations to Zendesk CRM.

**Customize SaaS with AI/ML**

You can enrich your events from SaaS applications using AWS Artificial Intelligence/Machine Learning services and gain valuable insights. For example, you can load your data from Shopify to EventBridge to trigger a workflow and use AI services such as Amazon Comprehend for image tagging of new retail products.

---

## **Simple Notification Service (SNS)**

**Pub/sub messaging for microservices and serverless applications.**

Amazon SNS is a highly available, durable, secure, fully managed pub/sub messaging service that enables you to decouple microservices, distributed systems, and event-driven serverless applications. Amazon SNS provides topics for high-throughput, push-based, many-to-many messaging.

**Benefits and features**

**Reliably deliver messages with durability**

Amazon SNS uses cross availability zone message storage to provide high message durability. Amazon SNS reliably delivers messages to valid AWS endpoints, such as Amazon SQS queues and AWS Lambda functions.

**Automatically scale your workload**

Amazon SNS leverages the proven AWS cloud to dynamically scale with your application. Amazon SNS is a fully managed service, taking care of the heavy lifting related to capacity planning, provisioning, monitoring, and patching.

**Simplify your architecture with Message Filtering**

Amazon SNS helps you simplify your pub/sub messaging architecture by offloading the message filtering logic from your subscriber systems, and message routing logic from your publisher systems.

**Keep messages private and secure**

Amazon SNS topic owners can set topic policies that restrict who can publish and subscribe to a topic. Amazon SNS also ensures that data is encrypted in transit and at rest, and provides VPC endpoints for message privacy.

---

## **Simple Queue Service (SQS)**

**A message queuing service**

Amazon SQS provides queues for high-throughput, system-to-system messaging. You can use queues to decouple heavyweight processes and to buffer and batch work. Amazon SQS stores messages until microservices and serverless applications process them.

**Benefits and features**

**Highly scalable Standard and FIFO queues**

Queues scale elastically with your application. Nearly unlimited throughput and no limit to the number of messages per queue in Standard queues. First-In-First-Out delivery and exactly once processing in FIFO queues.

**Durability and availability**

Your queues are distributed on multiple servers. Redundant infrastructure provides highly concurrent access to messages.

**Security**

Protection in transit and at rest. Transmit sensitive data in encrypted queues. Send messages in a Virtual Private Cloud.

**Batching**

Send, receive, or delete messages in batches of up to 10 messages or 256KB to save costs.

---

## **Step Functions**

**Assemble functions into business-critical applications**

AWS Step Functions is a serverless function orchestrator that makes it easy to sequence AWS Lambda functions and multiple AWS services into business-critical applications. Through its visual interface, you can create and run a series of checkpointed and event-driven workflows that maintain the application state.

**How it works**

1- Define your visual workflow in Workflow Studio and the console will auto-generate the code for you. You can also code it yourself using code snippets in the console or locally with VS Code.

2 - Specify the resources, such as Lambda functions and SNS topics, that you want to trigger in your workflow.

3 - Start an execution to visualize and verify that the steps of your workflow are operating as intended. Inspect and debug your execution history from the console directly.

**Benefits and features**

**Built-in error handling**

AWS Step Functions tracks the state of each step, so you can automatically retry failed or timed-out tasks, catch specific errors, and recover gracefully, whether the task takes seconds or months to complete.

**Execution event history**

AWS Step Functions creates a detailed event log for every execution, so when things do go wrong, you can quickly identify not only where, but why. All of the execution history is available visually and programmatically to quickly troubleshoot and remediate failures.

**Automatic scaling**

AWS Step Functions automatically scales the operations and underlying compute to run the steps of your application for you in response to changing workloads. Step Functions scales automatically to help ensure the performance of your application workflow remains consistently high as the frequency of requests increases.

**High availability**

AWS Step Functions has built-in fault tolerance. Step Functions maintains service capacity across multiple Availability Zones in each region to help protect application workflows against individual machine or data center facility failures. There are no maintenance windows or scheduled downtimes.

**Pay per use**

With AWS Step Functions, you pay only for the transition from one step of your application workflow to the next, called a state transition. Billing is metered by state transition, regardless of how long each state persists (up to one year).

**Administrative security**

AWS Step Functions is integrated with AWS Identity and Access Management (IAM). IAM policies can be used to control access to the Step Functions APIs.

**Use cases**

**Web service integration**

Build workflows that coordinate tasks across different services. Yelp transformed a monolithic business-critical code base into a simpler and more resilient billing service.

**Data processing**
The Guardian newspaper automated serverless data processing and subscriber management using AWS Step Functions, AWS Lambda, and Amazon CloudWatch Events.

---

## **Amazon AppFlow**

Amazon AppFlow integrates apps and automates data flows without code.

---

## **Managed Apache Airflow**

Run Apache Airflow without provisioning or managing servers.

## **Amazon MQ**

Managed message broker service for Apache ActiveMQ and RabbitMQ

---

## **SWF**

Workflow Service for Coordinating Application Components

---

# **AR & VR**

## **Amazon Sumerian**

Easily create and run browser-based 3D, augmented reality (AR), and virtual reality (VR) applications.

Amazon Sumerian will be transitioning the existing experience and functionality to allow customers to author scenes using Babylon.js and publish with AWS Amplify. **The Amazon Sumerian service is no longer accepting new customers.**

**Benefits**

**Create a 3D scene in minutes**

Easily create and embed 3D scenes into new or existing web pages with Babylon.js.

**Easily integrate with Sumerian Hosts**

Sumerian Hosts are available open source on GitHub for easy integration with your Babylon.js and Three.js applications.

**Deliver anytime, anywhere**

One-click host your 3D experience using AWS Amplify to deploy your scenes anywhere.

---

# **AWS Cost Management**

## **AWS Budgets**

You can use AWS Budgets to set custom budgets that alert you when your costs and usage, utilization, or coverage of Savings Plans and RIs exceed your budgeted amount.

AWS Budgets information is updated up to three times a day. Updates typically occur between 8 to 12 hours after the previous update.

**You can create the following types of budgets:**

- **Cost budgets** – Plan how much you want to spend on a service.

- **Usage budgets** – Plan how much you want to use one or more services.

- **RI utilization budgets** – Define a utilization threshold and receive alerts when your RI usage falls below that threshold. This lets you see if your RIs are unused or under-utilized.

- **RI coverage budgets** – Define a coverage threshold and receive alerts when the number of your instance hours that are covered by RIs fall below that threshold. This lets you see how much of your instance usage is covered by a reservation.

- **Savings Plans utilization budgets** – Define a utilization threshold and receive alerts when the usage of your Savings Plans falls below that threshold. This lets you see if your Savings Plans are unused or under-utilized.

- **Savings Plans coverage budgets** – Define a coverage threshold and receive alerts when your Savings Plans eligible usage that is covered by Savings Plans fall below that threshold. This lets you see how much of your instance usage is covered by Savings Plans.

---

## **Cost Explorer**

Cost Explorer is a tool that enables you to visualize, understand, and manage your AWS costs and usage over time. With Cost Explorer, you can filter and group by values such as API operation, Availability Zone, AWS service, custom cost allocation tag, Amazon EC2 instance type, purchase option, AWS Region, usage type, usage type group, and more. If you use consolidated billing, you can also filter by member account. In addition, you can see a forecast of future costs based on your historical cost data.

After you have achieved your desired results with filters and group-bys, you can either download your results by choosing Download as CSV or save the report by clicking Save to report library.

You can enable Cost Explorer for your account using this procedure on the Billing and Cost Management console. **You can't enable Cost Explorer using the API.** After you enable Cost Explorer, AWS prepares the data about your costs for the current month and the last 12 months, and then calculates the forecast for the next 12 months. The current month's data is available for viewing in about 24 hours. The rest of your data takes a few days longer. Cost Explorer updates your cost data at least once every 24 hours.

**Use cases**

**Build custom applications**

Directly access the interactive, ad-hoc analytics engine that powers AWS Cost Explorer. The Cost Explorer API allows you to programmatically query your cost and usage data.

**Use granular filtering**

AWS Cost Explorer helps you visualize, understand, and manage your AWS costs and usage over a daily or monthly granularity. You can also access your data with further granularity by enabling hourly and resource level granularity.

**Forecasting with Cost Explorer**

You create a forecast by selecting a future time range for your report. You can use a forecast to estimate your AWS bill and set alarms and budgets for based on predictions.

---

## **AWS Application Cost Profiler**

Cost per tenant and workload

---

## **AWS Billing Conductor**

Simplifying your billing practice

---

## **AWS Marketplace Subscriptions**

Digital catalog where you can find, buy, and deploy software

---

# **Blockchain**

## **Amazon Managed Blockchain**

Easily create and manage scalable blockchain networks

Amazon Managed Blockchain is a fully managed service that makes it easy to join public networks or create and manage scalable private networks using the popular open-source Hyperledger Fabric and Ethereum frameworks. You can write smart contracts and applications and run them on the blockchain network to transact securely.

**Benefits and features**

**Fully managed**

Get started with blockchain in minutes. With Amazon Managed Blockchain, you can quickly create blockchain networks that span multiple AWS accounts and eliminate manual provisioning of hardware and configuring of software, security, and network settings.

**Choice of framework**

Choice of frameworks between Hyperledger Fabric and Ethereum.

**Reliable and secure**

Amazon Managed Blockchain leverages Amazon Quantum Ledger Database Technology (QLDB) to improve the reliability of the Hyperledger Fabric Ordering Service. Also, Managed Blockchain uses AWS Key Management Service (KMS) technology to secure the Hyperledger Fabric Certificate Authority.

**Integrated**

Send blockchain network activity from Amazon Managed Blockchain to AWS analytics services like Amazon Redshift to get additional insights from your network.

**Sample use cases**

**Financial services**

Financial institutions can reduce the time and cost of cross-boundary asset transfers by using an Amazon Managed Blockchain network to directly send payments to other network members in a trusted way.

**Supply chain**

Manufacturing businesses can use an Amazon Managed Blockchain network as a transparent and efficient way to keep track of ownership of goods that move across global supply chain networks.

---

# **Business Applications**

## **Alexa for Business**

Alexa for Business Provides Tools to Manage Alexa in Your Organization

---

## **Amazon Chime**

Amazon Chime is a communications service that transforms online meetings

---

## **Amazon Connect**

Amazon Connect is a contact center that enables engagement at any scale.

---

## **Amazon Honeycode**

Build mobile and web apps without programming

---

## **Amazon Pinpoint**

Engage Users via Email, SMS, Push & Analytics

---

## **Amazon Simple Email Service**

Email Sending and Receiving Service

---

## **Amazon WorkDocs**

Secure Enterprise Storage and Sharing Service

---

## **Amazon WorkMail**

Secure Email and Calendaring Service

---
