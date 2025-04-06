
# MOVING DATA FROM ON-PREMISE SQL SERVER TO AZURE CLOUD STORAGE FOR ANALYSIS: AN END-TO-END AZURE DATA ENGINEERING PROJECT
While I enjoy building dashboards and uncovering hidden insights to support data-driven decisions, every Business Intelligence Analyst should also master end-to-end data engineering solutions. This not only accelerates business intelligence operations but also adds valuable skills to your professional toolkit. This weekend, I built a scalable Azure data engineering pipeline to transform raw layoff data into actionable insights. Here’s how I did it:
# PROBLEM STATEMENT
Your company collects layoff data from various on-premises sources but struggles with:
1.	Data silos – Layoff data stored in on-premises systems (SQL Server/CSV) with no centralized analytics access.
2.	Manual processes – Reliance on ad-hoc scripts and manual uploads causes delays and errors.
3.	Data inconsistencies – Raw data issues affect analysis, with no dashboard to track trends.
# THE TASK
Build an end-to-end pipeline that:
•	Ingest and transform data Databricks.
•	Store processed data in query-optimized Parquet format.
•	Connect to Power BI for visualization.
•	Create an interactive dashboard showing Top 10 Companies and countries affected by layoffs, and funding received between 2020 and 2023.
# MY STEP-BY-STEP SOLUTION
1.  I created a resource group, storage account, and containers
2.	I created linked services and datasets in Azure Data Factory to connect to SQL Server.
3.	Pulled data from SQL Server using a self-hosted integration runtime.
4.	Ingested data into the raw Azure Blob Storage container.
5.	Mounted Databricks to Azure Blob Storage using access keys.
6.	Transformed the data in Databricks by correcting data types, handling duplicates and null values, and resolving other inconsistencies.
7.	Wrote the clean data back to the transformed layer in Blob Storage.
8.	Built an interactive Power BI report showing key metrics.
# WHY THIS MATTERS
•	Eliminated manual work: Automated ingestion → insights.

•	Improved trust: Consistent data types and enforced quality checks.

•	Scalable foundation: Ready for future data growth.


Tech Stack: Azure Data Factory, Databricks (PySpark), Blob Storage, Power BI

#DataEngineering #Azure #BusinessIntelligence #ETL #DataAnalytics

![DIAGRAM](https://github.com/user-attachments/assets/378a6a3e-0983-47f0-8333-cf57843be613)

![layoff_page-0002](https://github.com/user-attachments/assets/24d62c9b-388a-4f98-a1dd-10e2c13265ce)


