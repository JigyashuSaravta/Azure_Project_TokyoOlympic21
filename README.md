# Azure_Project_TokyoOlympic21
This project demonstrates the development of an end-to-end data pipeline using Microsoft Azure's cloud computing services. The core dataset for this project is the 2021 Tokyo Olympics data from Kaggle.

## Project Overview
The goal of this project was to create a robust, scalable data engineering system capable of handling, transforming, and analyzing large datasets in a cloud environment. This system is designed for real-world applications, such as large-scale international athletic events like the Olympics, providing deep analytical insights from massive volumes of data.

## Data Flow
![DataFlow](https://github.com/JigyashuSaravta/Azure_Project_TokyoOlympic21/assets/105642798/ca956e18-0a94-4909-a26f-b45f3be7ce7c)

## Project Steps
1. Data Source: The data for this project was sourced from Kaggle and fethced from my Github repo and contains the 2021 Tokyo Olympics dataset.
2. Data Ingestion: Azure Data Factory was used to automate the extraction of Olympic data from GitHub. This service simplifies the construction and scheduling of data-driven workflows, allowing raw data to be fed directly into Azure Data Lake Storage Gen 2 without user intervention.
3. Raw Data Storage: The ingested raw data is stored in Azure Data Lake Storage Gen 2.
4. Data Transformation: Data transformation is performed using Azure Databricks, a big data analytics platform powered by Apache Spark. This service provides a collaborative workspace for processing large amounts of data, including data cleansing, transformation, and normalization.
5. Transformed Data Storage: The transformed data is stored again in Azure Data Lake Storage Gen 2.
6. Data Analysis: Azure Synapse Analytics is used for data analysis, combining big data and data warehousing. Synapse allows for executing complex queries over processed datasets and directly connecting to data visualization tools like Tableau.
7. Data Visualization: An interactive dashboard is created using Tableau, connected to Azure Synapse via OAuth for real-time analytics. The dashboard provides a user-friendly interface for displaying various visualizations.

## Tableau Dashboard
<img width="582" alt="Screenshot 2024-07-02 at 7 42 37 PM" src="https://github.com/JigyashuSaravta/Azure_Project_TokyoOlympic21/assets/105642798/0c1753b6-dd45-4f88-89db-8d54daf944ce">


## Analysis and Discoveries
- Gender Participation: Visualizations highlighted gender participation in several sports, revealing discrepancies and equality in athlete activity.
- Medal Distribution: Analysis of the medal count provided insights into which nations lead, indicating the success of their sports programs.
- Team Participation: Statistics on the number of teams each country had provided insights into each country's funding and participation levels in various sports.
- Interactive Insights: The dashboard includes interactive filters for dynamic querying, allowing users to focus on specific parts of the data, such as a nation, sport, or discipline, thereby enhancing the dashboard’s usability.

## Intended Audience
This project is targeted at:

- Data engineers
- Cloud architects
- Analytics teams
- Authorities in charge of large-scale athletic events
- Individuals learning Azure data services and data engineering principles
