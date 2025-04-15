# PostgreSQL to Elasticsearch with Debezium and Logstash

This project demonstrates a streaming pipeline using **Debezium** to capture change data from **PostgreSQL** and forward it to **Elasticsearch** using **Kafka**, **Kafka Connect**, and **Logstash**. Everything is orchestrated with Docker Compose.

## 📦 Services Overview

- **PostgreSQL** – Source database.
- **Zookeeper** – Kafka dependency.
- **Kafka** – Message broker for Debezium.
- **Kafka Connect** – Runs Debezium PostgreSQL connector.
- **Elasticsearch** – Destination data store.
- **Logstash** – Consumes Kafka topics and pushes data to Elasticsearch.
- **Kibana** (optional) – UI for Elasticsearch.

## 🐳 Docker Compose

```bash
docker-compose up -d
