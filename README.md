# WAU-Weekly-Active-User-chart

Project Overview
This project focuses on developing a Weekly Active Users (WAU) chart by leveraging modern data engineering tools. The workflow includes ETL/ELT pipelines orchestrated using Apache Airflow to process and analyze user engagement data efficiently.

Project Components
1. Data Sources
   
  user_session_channel – Raw user session data

  session_timestamp – Session timestamp details

2. ETL Pipeline (Extract, Transform, Load)
   
Objectives:

  - Ingest raw data from Snowflake

  - Perform initial extraction and staging

  - Prepare data for further transformations

Key Steps:

  - Establish a connection to Snowflake

  - Extract user_session_channel and session_timestamp

  - Load data into a staging environment

3. ELT Pipeline (Extract, Load, Transform)
Objectives:

  - Integrate and transform raw data

  - Generate a session_summary table within the analytics schema

  - Implement data quality checks to ensure accuracy

Transformation Logic:

  - Join user_session_channel with session_timestamp

  - Aggregate session data at a weekly level

  - Identify and manage duplicate records

4. Data Visualization
  - Develop a Weekly Active Users (WAU) chart

  - Analyze trends in user engagement

Data Flow
  - Raw Data Ingestion (ETL Pipeline)

  - Data Transformation (ELT Pipeline)

Setup Instructions
  - Configure the Snowflake connection

  - Deploy and schedule Airflow DAGs

  - Validate data transformations

ETL Screenshots:
![image](https://github.com/user-attachments/assets/0783fc23-55e9-4c03-8e70-db63b2bdea3c)

ELT Screenshot:
![image](https://github.com/user-attachments/assets/4677e628-6139-433a-80d8-8ed52273b21d)

