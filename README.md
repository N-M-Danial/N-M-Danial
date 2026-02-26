<h1 align="center">Nik Danial | Data Scientist | Smart City Analytics</h1>
<h3 align="center">Designing real-time traffic intelligence systems for live command environments</h3>

---

# Flagship Systems

---

# FlowLab — Traffic Intelligence Platform

<img width="1919" height="912" alt="image" src="https://github.com/user-attachments/assets/dc483cc9-6e7c-4fb2-b61b-320f5e81e4be" />

Interactive, operations-grade traffic analytics system built for real-world monitoring environments.

FlowLab transforms raw CCTV vehicle counts into actionable corridor intelligence.

## Core Capabilities

- Real-time Level of Service (LOS) monitoring  
- Corridor-wide congestion visualization  
- Volume-to-Capacity (V/C) ratio computation  
- Full-day playback with time-slider control  
- Peak hour detection & congestion state classification  
- Multi-corridor performance comparison  

Designed for traffic control centers that require clarity, not dashboards for demo purposes.

---

## FlowLab AI — Predictive Traffic Engine

<img width="1919" height="774" alt="image" src="https://github.com/user-attachments/assets/a8ceaa67-0b3e-4e54-b953-1b039f955a30" />

FlowLab’s forecasting module delivers 24-hour next-day predictions at the individual road level.

### Model Architecture

- Gradient boosting via XGBoost  
- Autoregressive hour-by-hour forecasting logic  
- Road-specific model segmentation  

### Feature Engineering Strategy

- Lag-based hourly traffic features  
- Rolling mean congestion trends  
- Hour-of-day encoding  
- Weekday pattern learning  
- Road capacity constraints  
- Weighted training to emphasize congestion states  

### Outputs

- Hourly predicted traffic volume  
- Forecasted V/C ratios  
- Projected LOS grading  

Focus: Operational forecasting that anticipates congestion before it manifests.

---

# TrafficPulse — CCTV Health & Event Intelligence

<img width="1310" height="613" alt="image" src="https://github.com/user-attachments/assets/b0c8f59c-d390-4b83-911f-7b47472b81dd" />

Operational reliability platform for surveillance-based traffic systems.

TrafficPulse ensures camera networks remain visible, measurable, and accountable.

## System Functions

- Live CCTV connectivity status monitoring  
- Uptime / downtime analytics  
- Silent failure detection  
- Incident trend tracking  
- Historical event analysis  
- Snapshot viewer with AI detection overlays  

Purpose: Maintain surveillance integrity inside traffic command centers.

---

# Real-Time Streaming Data Architecture

Production-ready ingestion and serving infrastructure powering both FlowLab and TrafficPulse.

## Architecture Stack

- RabbitMQ → Event streaming layer  
- PostgreSQL → Structured storage & historical indexing  
- FastAPI → Secure API serving layer  

## Design Principles

- Clean separation of ingestion and analytics layers  
- Scalable CCTV AI event streaming  
- Structured query interfaces for dashboards  
- CSV-ready endpoints for downstream systems  

Built for continuous ingestion, not batch experimentation.

---

# MaxHub Suite — Internal Traffic Report Automation Framework

<img width="880" height="641" alt="image" src="https://github.com/user-attachments/assets/e444d1d3-f798-4966-a412-02139643cb24" />

Modular CLI-based system that standardizes traffic data workflows across operations teams.

MaxHub converts fragmented CCTV exports into validated, production-ready reports.

## Components

### MaxForm
- Connects to Alibaba MaxCompute  
- Retrieves CCTV volume & speed data  
- Applies preprocessing & threshold-based imputation  

### MaxValid
- Missing value detection  
- Null record identification  
- Hourly interval validation  

### MaxGen
- Automated multi-sheet Excel report generation  
- LOS computation  
- Structured formatting for official submission  

### MaxCheck
- CCTV-wide data quality scanner  
- Threshold-based performance screening  

MaxHub represents:

- Data governance enforcement  
- Workflow automation at scale  
- Repeatable reporting infrastructure  
- Internal tooling architecture discipline  

---

# Technical Stack

## Languages  
Python · SQL · Power Query M  

## Machine Learning  
XGBoost · Time-Series Feature Engineering · Congestion Modeling  

## Backend & APIs  
FastAPI · RabbitMQ · PostgreSQL  

## Data Infrastructure  
Alibaba MaxCompute · OSS · MS SQL Server  

## Visualization  
Streamlit · Power BI · Matplotlib · QGIS  

## Transport Engineering  
Level of Service (LOS) Modeling · Corridor Flow Analytics · PTV Visum  

---

# Engineering Philosophy

- Systems > Scripts  
- Infrastructure > Notebooks  
- Reliability > Visual polish  
- Operational clarity > Academic benchmarks  
- Automate first, optimize second  
- Enforce data quality before analytics  

---

# Domain Focus

- Smart City Traffic Operations  
- CCTV-Based Vehicle Intelligence  
- Corridor Congestion Forecasting  
- Command Room Systems Engineering  
- Urban Traffic Data Infrastructure  

---

# Connect

- GitHub: https://github.com/N-M-Danial  
- Email: nik.muhammad.danial94@email.com  

---
