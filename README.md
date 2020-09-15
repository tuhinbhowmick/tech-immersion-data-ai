# Tech Immersion Mega Data & AI Workshop (Updated)

## Setup: Connecting to your VM with Remote Desktop

When setting up a cloud infrastructure, it's a good idea to create a VM where you can install all of the tools and applications you need to manage your environment. This is called a jumpbox. A jumpbox has been created for you. In order to use it, you need to open Remote Desktop Connection.

You will need three pieces of information:

- Jump VM DNS Name
- VM Admin User Name
- VM Admin Password

Start Remote Desktop and enter the Jump DNS Name as the computer name. When you are asked to enter your credentials, click "More Choices". Click "Use a different account".

In the user name box, enter your VM Admin User Name. Enter your VM Admin Password as the password. Click "Connect". When the warning comes up, click "Yes." You are now connected to your jumpbox and can continue with each individual experience.

## Data: Data-focused

- **Data, Experience 1** - [Business critical performance and security with SQL Server 2019 ](./data-exp1/README.md)

  This experience will highlight the new features of SQL Server 2019 with a focus on performance and security. You will begin by performing an assessment of Contoso Auto's on-premises database to determine feasibility for migrating to SQL Server on a VM in Azure, and then complete the database migration. Next, you will gain hands-on experience by running queries using some of the new query performance enhancements and evaluating the results. You will evaluate the data security and compliance features provided by SQL Server 2019 by using the Data Discovery & Classification tool in SSMS to identify tables and columns with PII and GDPR-related compliance issues. You will then address some of the security issues by layering on dynamic data masking, row-level security, and Always Encrypted with secure enclaves.

- **Data, Experience 2** - [Handling Big Data with SQL Server 2019 Big Data Clusters](./data-exp2/README.md)

  Highlight the new features of SQL Server 2019 with a focus on Big Data Clusters and data virtualization. Attendees will gain hands-on experience with querying both structured and unstructured data in a unified way using T-SQL. This capability will be illustrated by joining different data sets, such as product stock data in flat CSV files in Azure Storage, product reviews stored in Azure SQL Database, and transactional data in SQL Server 2019 for exploratory data analysis within Azure Data Studio. This joined data will be prepared into a table used for reporting, highlighting query performance against this table due to intelligent query processing. With the inclusion of Apache Spark packaged with Big Data Clusters, it is now possible to use Spark to train machine learning models over data lakes and use those models in SQL Server in one system. Attendees will learn how to use Azure Data Studio to work with Jupyter notebooks to train a simple model that can predict vehicle battery lifetime, train a simple model that can predict vehicle battery lifetime, score new data and save the result as an external table. Finally, attendees will experience the data security and compliance features provided by SQL Server 2019 by using the Data Discovery & Classification tool in SSMS to identify tables and columns with PII and GDPR-related compliance issues, then address the issues by layering on dynamic data masking to identified columns.

- **Data, Experience 3** - [Unlocking new capabilities with friction-free migrations to Azure SQL Managed Instance](./data-exp3/README.md)

  Show how databases previously prevented from using PaaS services can be migrated to SQL MI and take advantage of features only available in Azure. Migrate an on-premises parts catalog database, currently running on SQL Server 2012 and using Service Broker, to SQL MI. Create an online secondary database for reporting on operations and finance using SQL MI, using transactional replication.

- **Data, Experience 4** - [Leveraging Cosmos DB for near real-time analytics](./data-exp4/README.md)

  In this experience, attendees will use Azure Cosmos DB to ingest streaming vehicle telemetry data as the entry point to a near real-time analytics pipeline built on Cosmos DB, Azure Functions, Event Hubs, Azure Stream Analytics, and Power BI. To start, attendees will complete performance-tuning on Cosmos DB to prepare it for data ingest, and use the change feed capability of Cosmos DB to trigger Azure Functions for data processing. The function will enrich the telemetry data with location information, then send it to Event Hubs. Azure Stream Analytics extracts the enriched sensor data from Event Hubs, performs aggregations over windows of time, then sends the aggregated data to Power BI for data visualization and analysis. A vehicle telemetry data generator will be used to send vehicle telemetry data to Cosmos DB.

- **Data, Experience 5** - [Simplifying data movement with Azure Data Factory](./data-exp5/README.md)

  In this experience, attendees will learn how to use Azure Data Factory to help Contoso Auto easily create pipelines that orchestrate data movement.

* **Data, Experience 6** - [Delivering the Modern Data Warehouse with Azure SQL Data Warehouse, Azure Databricks, and Power BI](./data-exp6/README.md)

  A modern data warehouse lets you bring together all your data at any scale easily, and to get insights through analytical dashboards, operational reports, or advanced analytics for all your users. In this experience we will demonstrate how to transform data gathered from various sources, including Cosmos DB, into Azure Data Lake Storage Gen2, Azure Databricks and Azure SQL DW to build a modern data warehouse.

* **Data, Experience 7** - [Open Source Databases at Scale](./data-exp7/README.md)

  In this experience, attendees will use advanced features of the managed PostgreSQL PaaS service on Azure to make Conto Auto's database more scalable and able to handle the rapid ingest of streaming data while simultaneously generating and serving pre-aggregated data for reports.

## AI: AI & Machine Learning-focused

- **AI, Experience 1** - [Quickly build comprehensive Bot solutions with the Virtual Assistant Solution Accelerator](./ai-exp1/README.md)

  Show how the Virtual Assistant Solution accelerator can rapidly accelerate developing conversation bots. This exercise will use the automotive Virtual Assistant starter solution, which converts the user’s speech to actions, such as controlling the vehicle’s climate settings and radio. Attendees will register a new skill that monitors car sensor data and alerts the driver when there is a potential problem with the vehicle. Part of the process is to create an Adaptive Card to show vehicle data, recommendation for service (call out to function to get battery replacement prediction), and an option to contact the nearest service center. To entice the driver to service the car at that time, the bot will have them select a gift card of their choice that will give them a promo code for a coupon at that service center.

- **AI, Experience 2** - [Yield quick insights from unstructured data with Knowledge Mining and Cognitive Services](./ai-exp2/README.md)

  Highlight how building a cognitive search pipeline using Cognitive Services and Knowledge Mining can yield quick insights into unstructured data. Cognitive search is an AI feature in Azure Search, used to extract text from images, blobs, and other unstructured data sources - enriching the content to make it more searchable in an Azure Search index. Attendees will create a cognitive search pipeline in Azure Search, using Cosmos DB and an Azure Storage account as data sources, and apply pre-configured and custom cognitive skills to enrich the data in the indexing pipeline.

- **AI, Experience 3** - [Better models made easy with Automated Machine Learning](./ai-exp3/README.md)

  Show how automated ML capability in Azure Machine Learning can be used for Life Cycle Management of the manufactured vehicles and how AML helps in creation of better vehicle maintenance plans. Attendees will train a Linear Regression model to predict the number of days until battery failure using Automated Machine Learning the visual interface from the Azure Portal and optionally from within Jupyter Notebooks. They will also use the model interpretability features of the Azure Machine Learning Python SDK to understand which features have the greatest impact on the model's predictions.

- **AI, Experience 4** - [Creating repeatable processes with Azure Machine Learning pipelines](./ai-exp4/README.md)

  Attendees will learn how Contoso Auto can benefit from creating re-usable machine learning pipelines with Azure Machine Learning.

- **AI, Experience 5** - [Making deep learning portable with ONNX](./ai-exp5/README.md)

  Attendees will experience how Contoso Auto can leverage Deep Learning technologies to scan through their vehicle specification documents to find compliance issues with new regulations. Then they will deploy this model, standardizing operationalization with ONNX. They will see how this simplifies inference runtime code, enabling pluggability of different models and targeting a broad range of runtime environments from Linux based web services to Windows/.NET based apps.

- **AI, Experience 6** - [MLOps with Azure Machine Learning and Azure DevOps](./ai-exp6/README.md)

  Attendees will experience how Contoso Auto can use MLOps to formalize the process of training and deploying new models using a DevOps (CI/CD) approach.
