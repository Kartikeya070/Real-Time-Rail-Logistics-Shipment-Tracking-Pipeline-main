# Real-Time-Rail-Logistics-Shipment-Tracking-Pipeline-main
A real-time rail logistics shipment tracking pipeline that streams shipment events using Kafka, processes them with Spark Structured Streaming, applies ETL transformations, and stores results in a data warehouse for analytics. Airflow orchestrates and automates the workflow for scalable end-to-end data engineering.

A modular end-to-end real-time data engineering pipeline simulating a rail logistics shipment tracking system using Apache Kafka, Spark Structured Streaming, Apache Airflow, and Data Warehouse concepts.

---

## 📌 Project Overview

This project simulates a modern rail logistics tracking system where shipment events are continuously generated, streamed, processed, and stored for analytics.

It demonstrates a complete real-time data engineering workflow including ingestion, streaming, transformation, orchestration, and analytics.

---

## 🎯 Key Objectives

- Real-time shipment event ingestion  
- Distributed stream processing  
- ETL orchestration using Airflow  
- Warehouse-ready data modeling  
- Kafka-based streaming architecture  
- Scalable modular pipeline design  

---

## 🏗️ System Architecture

Logistics Events (Shipment Data)  
↓  
Kafka Producer (Event Generator)  
↓  
Apache Kafka (Streaming Layer)  
↓  
Spark Structured Streaming (Processing)  
↓  
ETL Transformation Layer  
↓  
Data Warehouse (Analytics Storage)  
↓  
Apache Airflow (Orchestration)  

---

## 🔄 Data Flow

1. Shipment events are generated (dispatch, transit, delay, delivery)  
2. Kafka Producer sends events to Kafka topics  
3. Kafka acts as a real-time streaming backbone  
4. Spark Structured Streaming consumes events  
5. Data is cleaned, transformed, and aggregated  
6. Processed data is loaded into Data Warehouse  
7. Airflow schedules and manages ETL workflows  

---

## 📁 Project Structure

Real-Time-Rail-Logistics-Shipment-Tracking-Pipeline/  
├── kafka-producer/  
│   └── producer.py  
├── spark-consumer/  
│   └── streaming_consumer.py  
├── airflow-dag/  
│   └── etl_dag.py  
├── data-warehouse/  
│   └── schema.sql  
├── docs/  
│   └── architecture.md  
├── requirements.txt  
└── README.md  

---

## 🧩 Module Breakdown

### 📡 Kafka Producer (kafka-producer/producer.py)

Responsibilities:
- Simulates shipment tracking events  
- Publishes data to Kafka topics  
- Generates real-time logistics streams  

Sample Event:
```json
{
  "shipment_id": "RL1021",
  "location": "Delhi",
  "status": "In Transit",
  "timestamp": "2026-05-22T10:30:00"
}
