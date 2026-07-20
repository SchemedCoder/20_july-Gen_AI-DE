# GenAI Data Engineering Platform

> Enterprise-grade Data Engineering Platform with Kafka, PySpark, Snowflake, Airflow, FastAPI, PostgreSQL, and Agentic AI powered by local LLMs (Ollama).

![Python](https://img.shields.io/badge/Python-3.11-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-Latest-green)
![Kafka](https://img.shields.io/badge/Apache-Kafka-orange)
![Snowflake](https://img.shields.io/badge/Snowflake-Data%20Warehouse-blue)
![PySpark](https://img.shields.io/badge/PySpark-Streaming-red)
![Docker](https://img.shields.io/badge/Docker-Compose-blue)
![License](https://img.shields.io/badge/License-MIT-success)

---

# Overview

The **GenAI Data Engineering Platform** is a production-inspired portfolio project that demonstrates how modern data engineering and Generative AI work together in an enterprise environment.

Instead of a simple chatbot or notebook, this project simulates a real retail data platform where streaming data is ingested, validated, transformed, stored in a cloud data warehouse, and monitored using AI agents.

The project showcases the technologies commonly used by Data Engineers and AI Engineers in production systems.

---

# Objectives

- Build a scalable streaming data platform.
- Implement a Medallion Architecture (Bronze → Silver → Gold).
- Stream events using Apache Kafka.
- Process streaming data using PySpark Structured Streaming.
- Store analytical data in Snowflake.
- Orchestrate pipelines with Apache Airflow.
- Validate data quality using Great Expectations.
- Build AI agents using local LLMs with Ollama.
- Expose REST APIs using FastAPI.
- Monitor the platform using Prometheus and Grafana.
- Containerize the platform using Docker Compose.

---

# High-Level Architecture

```text
                 Retail Event Simulator
                           │
                           ▼
                     Apache Kafka
                           │
                           ▼
             PySpark Structured Streaming
                           │
             ┌─────────────┴─────────────┐
             ▼                           ▼
         Bronze Layer              Data Quality
             │                           │
             ▼                           ▼
         Silver Layer              Validation Reports
             │
             ▼
          Gold Layer
             │
             ▼
         Snowflake DW
             │
      ┌──────┴───────────┐
      ▼                  ▼
 FastAPI APIs      AI Agents (Ollama)
      │                  │
      └──────────┬───────┘
                 ▼
      Grafana / Swagger UI
```

---

# Technology Stack

| Category | Technology |
|-----------|------------|
| Programming | Python 3.11 |
| Backend API | FastAPI |
| Streaming | Apache Kafka |
| Processing | PySpark Structured Streaming |
| Data Warehouse | Snowflake |
| Workflow Orchestration | Apache Airflow |
| Database | PostgreSQL |
| Data Quality | Great Expectations |
| Generative AI | Ollama (Llama / Qwen) |
| Vector Search | FAISS |
| Monitoring | Prometheus & Grafana |
| Containerization | Docker Compose |
| Testing | Pytest |
| CI/CD | GitHub Actions |

---

# Planned Project Phases

| Phase | Description |
|--------|-------------|
| Phase 1 | Platform Foundation |
| Phase 2 | Retail Event Simulator |
| Phase 3 | Kafka Streaming |
| Phase 4 | PySpark Streaming |
| Phase 5 | Data Quality Framework |
| Phase 6 | Snowflake Data Warehouse |
| Phase 7 | Airflow Orchestration |
| Phase 8 | AI Agents |
| Phase 9 | Metadata RAG |
| Phase 10 | Dashboard & APIs |
| Phase 11 | Monitoring |
| Phase 12 | Production Readiness |

---

# Repository Structure

```
GenAI-Data-Engineering-Platform/

backend/
docker/
docs/
tests/
scripts/
simulator/
kafka/
spark/
snowflake/
airflow/
agents/
shared/

docker-compose.yml
requirements.txt
.env.example
README.md
```

---

# Features

- Enterprise-style project structure
- Event-driven architecture
- Streaming data pipelines
- Medallion Architecture
- Snowflake analytics warehouse
- AI-assisted data investigation
- SQL generation using LLMs
- Metadata search
- Data quality monitoring
- REST APIs
- Docker deployment
- Automated testing
- Production-ready documentation

---

# Why This Project?

This repository is designed as a portfolio project for aspiring Data Engineers and AI Engineers. It combines modern data engineering practices with practical Generative AI integration, using local open-source models to avoid paid API dependencies.

---

# Status

🚧 **Current Version:** v0.1.0 (Phase 1 – Foundation)

Work is being developed incrementally, with each phase producing a runnable, testable milestone.

---

# License

This project is licensed under the MIT License.
