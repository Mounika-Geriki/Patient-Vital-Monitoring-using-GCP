# 🩺 Patient_Vital_Monitoring_GCP  
### From Real-Time Vitals to Clinical Insights: A Cloud-Native Streaming Analytics Pipeline  

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![GCP](https://img.shields.io/badge/Google%20Cloud-Active-brightgreen)
![Streaming](https://img.shields.io/badge/Streaming-Pub%2FSub%20%7C%20Dataflow-orange)
![Data Warehouse](https://img.shields.io/badge/Warehouse-BigQuery-yellow)
![Visualization](https://img.shields.io/badge/Visualization-Power%20BI-gold)
![Architecture](https://img.shields.io/badge/Architecture-Medallion-bronze)
![Status](https://img.shields.io/badge/Status-Production--Ready-success)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-purple)

---

## 🔍 Project Overview

An **end-to-end real-time patient vital monitoring system** built on **Google Cloud Platform (GCP)** that transforms **streaming physiological data into business-ready analytics** using a **Bronze–Silver–Gold Medallion Architecture**.

This project simulates patient vitals, streams them using **Pub/Sub**, processes them using **Apache Beam on Dataflow**, stores analytics in **BigQuery**, and visualizes insights through **Power BI dashboards**.

---

## 🚀 Key Capabilities

✅ Real-time patient vital simulation (Python)  
✅ Pub/Sub based ingestion pipeline  
✅ Streaming ETL using Apache Beam on Dataflow  
✅ Medallion Architecture (Bronze, Silver, Gold)  
✅ Automated data validation & risk scoring  
✅ Business-ready BigQuery analytics table  
✅ Power BI clinical monitoring dashboard  
✅ Secure cross-cloud authentication via Service Accounts  

---

## 🏗️ System Architecture

```text
Python Vitals Simulator
        |
        ▼
Google Pub/Sub (Streaming Ingestion)
        |
        ▼
Apache Beam + Dataflow (Real-Time Processing)
   ├── 🥉 Bronze → Raw JSON in GCS
   ├── 🥈 Silver → Cleaned + Risk-Enriched Data in GCS
   └── 🥇 Gold   → Aggregated Patient Analytics in BigQuery
        |
        ▼
Power BI Dashboard (Cloud Visualization)
```

## 🧠 Medallion Data Design

| Layer | Purpose                     | Storage                  |
|--------|------------------------------|---------------------------|
| 🥉 Bronze | Raw event capture            | Google Cloud Storage      |
| 🥈 Silver | Cleaned + Risk Scored        | Google Cloud Storage      |
| 🥇 Gold   | Aggregated analytics         | BigQuery                  |

## 📊 Final Analytics Table (BigQuery)

**Dataset:** `healthcare`  
**Table:** `patient_risk_analytics`

| Column             | Description                     |
|--------------------|----------------------------------|
| `patient_id`       | Patient Identifier               |
| `avg_heart_rate`   | Avg Heart Rate                   |
| `avg_spo2`         | Avg Oxygen Saturation            |
| `avg_temperature` | Avg Body Temperature             |
| `max_risk_level`   | Final Risk Classification        |
