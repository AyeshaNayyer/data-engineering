# Project Overview

This project is designed to build a data pipeline with the following components:

## Components

### 1. Data Source
- **API**: The pipeline uses the [randomuser.me API](https://randomuser.me) to generate random user data.

### 2. Apache Airflow
- **Purpose**: Orchestrates the pipeline, managing the flow of data.
- **Storage**: Stores the fetched data in a MySQL database.

### 3. Apache Kafka and Zookeeper
- **Kafka**: Streams data from the MySQL database to the processing engine.
- **Zookeeper**: Manages and coordinates the Kafka brokers.

### 4. Control Center and Schema Registry
- **Control Center**: Monitors Kafka streams.
- **Schema Registry**: Manages schemas within the Kafka ecosystem.

### 5. Apache Spark
- **Purpose**: Handles data processing.
- **Configuration**: Includes master and worker nodes for distributed processing.

### 6. Cassandra
- **Purpose**: Stores the processed data for further use.

## Setup and Execution

To run this project, you'll need to set up the following services in your environment. Follow the steps below to configure and start the pipeline:

1. Clone the repository.
2. Set up the necessary environment variables in the `.env` file.
3. Use Docker Compose to spin up all services.
   ```bash
   docker-compose up -d
