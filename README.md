# ⚡ Realtime Data Streaming | End-to-End Data Engineering Project

This project demonstrates a **complete realtime data engineering pipeline** — from data ingestion to processing, storage, and visualization. It integrates the full modern data stack with tools like **Apache Kafka, Airflow, Spark, Cassandra**, and **Docker**, simulating a production-grade environment for streaming analytics.

---

## 🧠 **System Architecture**


c:\Users\mhmda\OneDrive\Documents\My_Programming_Projects\Realtime Data Streaming, End-to-End Data Engineering Project\e2e-data-engineering-main\Data engineering architecture.png


The system is designed as an interconnected, containerized data pipeline:

1. **Data Source** — Generates live data using the `randomuser.me` API  
2. **Apache Airflow** — Orchestrates the pipeline, scheduling and fetching data into PostgreSQL  
3. **Apache Kafka + Zookeeper** — Streams data from PostgreSQL to Spark in realtime  
4. **Schema Registry & Control Center** — Ensures stream management and monitoring  
5. **Apache Spark** — Processes incoming Kafka streams for transformation and enrichment  
6. **Cassandra** — Stores processed data for fast and scalable retrieval  
7. **Docker** — Containerizes the full pipeline for easy deployment and scalability  

---

## 🧩 **Technologies Used**

| Layer | Tools & Frameworks |
|-------|--------------------|
| **Orchestration** | Apache Airflow |
| **Messaging / Streaming** | Apache Kafka, Apache Zookeeper |
| **Processing** | Apache Spark |
| **Storage** | PostgreSQL, Cassandra |
| **Containerization** | Docker, Docker Compose |
| **Language** | Python |

---

## 🎯 **What You’ll Learn**

- Building a realtime data pipeline from ingestion to storage  
- Orchestrating workflows with Apache Airflow  
- Implementing event-driven architecture with Apache Kafka  
- Distributed synchronization with Apache Zookeeper  
- Data transformation and enrichment using Apache Spark  
- Persisting processed data in Cassandra and PostgreSQL  
- Containerizing and scaling with Docker Compose  

---

## ⚙️ **Getting Started**

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/MohamadAub/realtime-data-streaming-pipeline.git
cd realtime-data-streaming-pipeline

2️⃣ Start the Docker Services
docker-compose up

3️⃣ Access Airflow UI

Open your browser and go to:
http://localhost:8080

Use Airflow to trigger the pipeline DAGs.

4️⃣ Check Kafka Streams

Control Center URL:
http://localhost:9021

5️⃣ Explore Cassandra & PostgreSQL

1- Cassandra: stores processed data
2- PostgreSQL: raw data from Airflow ingestion


Project Architecture Diagram

      +---------------------+
      |  RandomUser API     |
      +----------+----------+
                 |
                 v
        +--------+---------+
        |   Apache Airflow  |----> PostgreSQL
        +--------+---------+
                 |
                 v
        +--------+--------+
        |   Apache Kafka  |
        +--------+--------+
                 |
                 v
        +--------+--------+
        |  Apache Spark   |
        +--------+--------+
                 |
                 v
        +--------+--------+
        |   Cassandra     |
        +-----------------+

📚 Learning Goals
	•	Hands-on understanding of data streaming concepts
	•	Event-driven architecture design using Kafka
	•	Containerized deployments with Docker
	•	Batch vs. streaming data processing
	•	Workflow automation using Airflow

⸻

🚀 Future Improvements
	•	Add data visualization dashboards (Grafana / Power BI)
	•	Include data quality checks (Great Expectations)
	•	Extend to cloud services (AWS MSK, GCP Pub/Sub, or Azure Event Hubs)
	•	Real-time alerting & monitoring system

⸻

🤝 Contributing

Contributions are welcome!
Fork the repository, make your changes, and submit a Pull Request.

⸻

📄 License

This project is licensed under the MIT License.

⸻

🌐 Connect with Me

👤 Mohamad El Ayoubi
🔗 https://github.com/MohamadAub
✉ mmelayoubi@gmail.com
📍 Paris, France