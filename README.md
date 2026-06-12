# Workforce_Performance_Analysis

![](https://github.com/DQuanBui/Workforce_Performance_Analysis/blob/main/workforce.png)

## Project Overview
The Workforce Performance Analytics project tackles a high-cost problem for any large retail operation: understanding what drives employee performance, engagement, and attrition so leaders can retain talent and protect revenue. Using a multi-table dataset of nearly 500K records spanning employees, monthly performance, store KPIs, and business outcomes, I built a complete end-to-end ELT pipeline by ingesting raw data into the cloud with Python and AWS S3, loading it into a Snowflake data warehouse, transforming it into a tested dimensional model with dbt, surfacing deep analytical insights with SQL, predicting attrition with a Scikit-learn machine learning model, and delivering interactive Power BI dashboards. This project demonstrates the full modern analytics-engineering workflow, from raw data to production-style data models to predictive insight, showing how a well-built data foundation turns scattered operational data into decisions that reduce turnover cost and improve workforce planning.

## Architecture Overview

- Extract & Load: Python reads the raw source tables, validates and standardizes them (date parsing, null handling for active vs exited employees), and lands partitioned files in an AWS S3 bucket, which are then loaded into Snowflake.

- Transform: dbt builds a layered, tested dimensional model on top of the raw Snowflake tables: staging models clean each source, dimension and fact tables form a star schema, and analytics marts pre-aggregate the business questions.

- Analyze & Predict: SQL queries run against the marts to extract deep workforce insights, while a Scikit-learn model uses the modeled feature tables to predict employee attrition and rank its strongest drivers.

- Visualize: Power BI connects to the Snowflake marts to deliver interactive dashboards for stakeholders.

## Tools
- Languages: Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn), SQL
- Cloud & Warehouse: AWS S3, Snowflake
- Transformation: dbt (data build tool)
- Visualization: Power BI

## Dataset Overview

## Objectives

## Data Modeling (dbt)

## Project Results

## Conclusion

## Contact
For any inquiries or questions regarding the project, please contact me at dbui10@fordham.edu
