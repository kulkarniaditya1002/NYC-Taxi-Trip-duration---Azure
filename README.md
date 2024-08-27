# NYC Taxi Trip Duration Prediction Using Azure Data Lake & Databricks

## Project Overview

This project implements a data lake solution for analyzing and transforming data, followed by training machine learning models. The goal is to predict the trip duration of NYC taxis using a dataset from 2014. The solution leverages Azure Blob Storage, Azure Databricks, and Apache Spark for processing and analyzing the data.

## Project Architecture

### Components:
1. **Azure Blob Storage**: Used to store the dataset, visualization plots, and results.
2. **Azure Databricks**: Used for preprocessing, exploratory data analysis, data transformation, and training machine learning models.
3. **Compute Engine (ETL Compute)**: The cluster/machine on which the Databricks Spark notebook runs. Specifications: 14GB RAM, 4 Core CPU.
4. **Resource Group**: Logical container for resources deployed in an Azure subscription.

## Dataset

- **Data Source**: New York City Taxi Cab trips, 2014, sourced from NYC Open Data via Kaggle.
- **Data Size**: 2.36 GB, with 14,999,999 rows and 18 columns.
- **Data Format**: CSV format including fields like vendor ID, pickup/dropoff datetime, passenger count, trip distance, location coordinates, payment details, fare amount, etc.

[Kaggle Dataset Link](https://www.kaggle.com/datasets/kentonnlp/2014-new-york-city-taxi-trips/data)

## Procedure

1. **Create an Azure Account**: [Azure Free Account](https://azure.microsoft.com/en-us/free/)
2. **Create Azure Blob Storage Account**: Store raw and processed data.
3. **Create Azure Databricks Workspace**: Set up notebooks for ETL, data analysis, and model training.
4. **Mount Azure Blob Storage on Databricks**: Use Spark to read and write data.
5. **Data Preprocessing and Transformation**:
    - Data Cleaning: Handle duplicates, null values, and apply filters.
    - Feature Engineering: Indexing, label encoding, and dropping unnecessary columns.
6. **Exploratory Data Analysis (EDA)**: Analyze and visualize the data.
7. **Model Training**:
    - Models Used: Gradient Boosting and Random Forest.
    - Data Split: 80%-20% for training and testing.

## Conclusion

- **Scalability**: Azure's distributed cloud services are ideal for big data analysis.
- **Azure Blob Storage**: Efficient for storing unstructured data, making it a suitable choice for a data lake.
- **Azure Databricks**: Provides comprehensive features for ETL, data analysis, model training, and workflow automation.

## References

- Azure Databricks Documentation
- Kaggle NYC Taxi Trip Dataset
- Azure Blob Storage Documentation
