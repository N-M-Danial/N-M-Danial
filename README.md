<h1 align="center">Nik Danial | Traffic Intelligence Engineer | Smart City Systems</h1>
<h3 align="center">Architecting operational traffic analytics infrastructure for real-world command environments</h3>

---

## Core Systems & Platforms

### FlowLab — Network Traffic Intelligence Lab

Interactive corridor-level traffic monitoring platform.

- Real-time LOS visualization across monitored road segments
- Full-day time-slider playback
- Peak hour detection & V/C analytics
- Multi-corridor congestion overview
- AI-based next-day traffic forecasting

#### AI View (Predictive Module)
- 24-hour next-day volume forecasting per road
- Built using **XGBoost regressors**
- Engineered features include:
  - Lag-based volume features
  - Rolling mean traffic patterns
  - Hour-of-day & weekday encoding
  - Road-specific capacity & structural constraints
  - Weighted training to emphasize congestion states
- Outputs predicted V/C ratios & LOS grades
- Autoregressive hour-by-hour prediction logic

Focus: Operational forecasting, not theoretical modeling.

---

### TrafficPulse (formerly AliCrew)

CCTV health & event monitoring system for traffic operations.

- Live camera connection status dashboard
- Uptime, downtime & incident tracking
- Historical event trend analysis
- Snapshot viewer with AI detection overlays
- Silent failure detection & camera anomaly flagging

Purpose: Maintain surveillance reliability in command environments.

---

### Real-Time Streaming Data Pipeline

Production-ready ingestion and serving architecture:

- **RabbitMQ** → Event streaming layer  
- **PostgreSQL** → Structured storage & historical indexing  
- **FastAPI** → Secure API serving layer  
- CSV endpoints for dashboard integration  

Designed for:
- Continuous CCTV AI event ingestion
- Scalable query serving
- Clean separation between ingestion and analytics layers

---

### MaxHub Suite (Internal CLI Automation Framework)

Modular CLI-based traffic data automation system.

Built to standardize traffic report workflows across IOC operations.

#### Components:

- **MaxForm**  
  Retrieves & transforms CCTV volume/speed data from Alibaba MaxCompute  
  Includes threshold-based imputation & preprocessing  

- **MaxValid**  
  Validates datasets for:
  - Missing values  
  - Null records  
  - Missing hourly intervals  

- **MaxGen**  
  Automatically generates structured Excel traffic reports  
  Calculates LOS values & builds multi-sheet outputs  

- **MaxCheck**  
  CCTV-wide data quality scanning tool  
  Identifies cameras within acceptable data thresholds  

MaxHub reflects a systemized approach to:
- Data quality governance  
- Workflow automation  
- Repeatable report generation  
- Internal tooling architecture  

---

### TRAX (Traffic Report Automation eXpert)

Streamlit-based operational report engine:

- MaxCompute querying
- Excel generation with OpenPyXL
- Embedded matplotlib charts
- Multi-sheet structured outputs
- Designed to eliminate repetitive manual reporting

---

## Technical Stack

**Languages**
Python · SQL · Power Query M  

**Machine Learning**
XGBoost · Time-Series Feature Engineering · LOS Modeling  

**Backend & APIs**
FastAPI · RabbitMQ · PostgreSQL  

**Data Infrastructure**
Alibaba MaxCompute · OSS · MS SQL Server  

**Visualization & Tools**
Streamlit · Power BI · Matplotlib · QGIS  

**Transport Engineering**
LOS Grading · Corridor Flow Analysis · PTV Visum  

---

## Engineering Philosophy

- Systems > Scripts  
- Reliability > Visual polish  
- Operational clarity > Academic benchmarks  
- Automation-first workflows  
- Data quality enforcement before analytics  

---

## Domain Focus

Smart City Traffic Operations  
CCTV-Based Traffic Analytics  
Corridor-Level Congestion Intelligence  
Command Room Systems Engineering  

---

## 📡 Connect

- GitHub: https://github.com/yourusername  
- Email: yourname@email.com  
- Portfolio: https://yourportfolio.com  

---
