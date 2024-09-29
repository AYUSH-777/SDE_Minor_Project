# Stock Market Kafka Real-Time Data Engineering Project

## Introduction
This project involves executing an end-to-end real-time data engineering pipeline for stock market data using Kafka. The aim is to stream, store, and analyze stock market data using various technologies such as Python, Apache Kafka, and AWS services like Glue, Athena, and S3.

## Architecture
The architecture includes:

- **Data Generation**: A Python-based stock market simulation that streams stock data.
- **Data Streaming**: Apache Kafka is used to stream the stock market data in real-time.
- **Data Storage**: The streamed data is ingested and stored in AWS S3.
- **Data Cataloging**: AWS Glue Crawler and Glue Data Catalog are used for automatic metadata creation.
- **Data Querying**: Amazon Athena is used for querying the stock data stored in S3 using SQL.

## Technologies Used
- **Programming Language**: Python (SDK - Boto3)
- **Amazon Web Services (AWS)**:
  - **S3**: For storing stock market data.
  - **Athena**: For querying stock data.
  - **Glue Crawler**: For scanning S3 data and creating metadata.
  - **Glue Data Catalog**: For managing metadata.
  - **EC2**: For hosting Apache Kafka.
- **Apache Kafka**: For real-time data streaming.

## Dataset
- **Dataset Used**: `indexProcessed.csv` (contains stock market data used in the simulation).

## Project Steps
1. **Simulate stock data** using Python.
2. **Stream data with Kafka** and store it into Amazon S3.
3. **Use AWS Glue** to catalog the data.
4. **Query and analyze** the data using Amazon Athena.
