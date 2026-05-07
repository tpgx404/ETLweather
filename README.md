# Weather ETL Pipeline using Apache Airflow, PostgreSQL & Docker

A beginner-friendly ETL (Extract, Transform, Load) data engineering project built using **Apache Airflow**, **PostgreSQL**, **Docker**, and the **Open-Meteo API**.

This pipeline automatically fetches live weather data, transforms it, and stores it inside a PostgreSQL database using Airflow DAG orchestration.

## 🚀 Project Overview
This project demonstrates a complete ETL workflow:
* **Extract:** Live weather data from the Open-Meteo API.
* **Transform:** Raw JSON responses converted into structured data.
* **Load:** Processed weather data stored into PostgreSQL.
* **Orchestrate:** Entire workflow managed using Apache Airflow DAGs.
* **Containerize:** All services run via Docker and Docker Compose.
* **Environment:** Optimized for running locally or inside GitHub Codespaces.

## 🛠 Tech Stack
* **Language:** Python
* **Orchestration:** Apache Airflow
* **Database:** PostgreSQL
* **Containerization:** Docker & Docker Compose
* **Environment:** GitHub Codespaces
* **Data Source:** Open-Meteo Weather API

## 🏗 Architecture
```mermaid
graph TD
    A[Open-Meteo API] -->|JSON Data| B[Apache Airflow DAG]
    subgraph ETL Process
    B --> C[Extract]
    C --> D[Transform]
    D --> E[Load]
    end
    E --> F[(PostgreSQL Database)]```

## ✨ Features
Automated ETL pipeline: Fully hands-off data processing.
Real-time Integration: Fetches up-to-date weather metrics.
Relational Storage: Structured data storage in PostgreSQL.
Task Orchestration: Efficient monitoring and scheduling via Airflow.
Dockerized: Consistent environment across different machines.
Modular DAG: Clean, maintainable Python code structure.
Beginner-friendly: Easy to understand and extend for learning purposes.
