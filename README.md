In this project we will be doing data engineering work on Pizza Sales data

environment:
1. Azure data lake storage gen 2 account (ADLS)
2. MS-SQL Server
3. Azure data factory
4. Azure data bricks
5. power BI desktop


Steps:
1. Import pizza_sales.csv into the sql server. table name = [dbo].[pizza_sales]
2. Create container in ADLS. e.g. pizza-data
3. inside the above container create two folders. e.g. raw, transform
4. Create Azure data factory pipeline e.g. pizza_adf_pipeline
5. use self hosted integrated runtime to connect with on-pres sql server from Azure data factory
6. pipeline will extract data from [dbo].[pizza_sales] table in SQL and store into  raw folder in container pizza-data in ADLS
7. use databricks to transform the extracted data in above step. (attached Pizza_Sales_trnsformation notebook for your referance)
8. databricks will store the transformed data into container pizza-data under transform folder.
9. load data from transform folder into Power BI and create reports.
10. attached pbix file for your referance (Pizza Sales.pbix)
