# Stock Market Real-Time Data Analysis Using Kafka

## Overview
This project demonstrates the integration of **Apache Kafka**, **AWS S3**, and **AWS Athena** for **real-time stock market data analysis**. The system uses **Kafka** for streaming data, where a **Kafka Producer** sends stock market data to a Kafka topic and a **Kafka Consumer** receives it. The data is then stored in **AWS S3** and can be queried using **AWS Athena**.

## Key Concepts
- **Real-Time Streaming**: Data is processed and analyzed as it arrives in real-time, similar to applications like Google Maps or Amazon notifications.
- **Apache Kafka**: A distributed event store and stream processing platform that handles real-time data streams.
  - **Producers**: Generate and send stock market data to Kafka topics.
  - **Consumers**: Consume and process data from Kafka topics.
  - **Brokers**: Manage Kafka data streams and topics.

- **Data Serialization**: Kafka producers send data in **JSON** format, which needs proper serialization for efficient handling.

- **AWS Services**:
  - **Amazon S3**: Cloud storage for storing consumed data.
  - **AWS Glue**: Data cataloging for automatically detecting the schema of stored data.
  - **Amazon Athena**: Querying service for querying the data stored in S3.

## Real-Time Data Flow
1. The **Kafka Producer** sends stock market data to Kafka topics.
2. The **Kafka Consumer** receives data and uploads it to **AWS S3** in real-time.
3. Data in S3 is cataloged by **AWS Glue**, making it available for querying with **AWS Athena**.

## Conclusion
This project showcases how to build a real-time data pipeline using **Apache Kafka**, **AWS S3**, **AWS Glue**, and **AWS Athena** for streaming, storing, and querying stock market data. It demonstrates a complete cycle from data production to consumption, storage, and analysis.
