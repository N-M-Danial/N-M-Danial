<h1 align="center">Nik Danial</h1>
<h3 align="center">Data Scientist & Engineer for Urban Mobility & Smart City Operations</h3>

---

## Overview

This portfolio documents the design, development, and deployment of production-grade traffic intelligence infrastructure for urban command environments. The systems presented here address the operational demands of real-time corridor monitoring, predictive congestion modelling, surveillance network management, and automated reporting — each grounded in rigorous data engineering principles and transport domain expertise.

---

## Systems

---

### FlowLab (Traffic Intelligence Platform)

<img width="1919" height="912" alt="FlowLab Dashboard" src="https://github.com/user-attachments/assets/dc483cc9-6e7c-4fb2-b61b-320f5e81e4be" />

FlowLab is an operations-grade traffic analytics platform designed for deployment within live traffic control environments. The system ingests raw CCTV-derived vehicle count data and transforms it into structured corridor-level intelligence, enabling operators to make informed, time-sensitive decisions with minimal interpretive overhead.

#### Core Capabilities

- Real-time Level of Service (LOS) assessment across monitored corridors
- Corridor-wide congestion state visualisation
- Volume-to-Capacity (V/C) ratio computation and threshold classification
- Full-day temporal playback via interactive time-slider interface
- Automated peak hour identification and congestion state categorisation
- Multi-corridor performance benchmarking and comparative analysis

---

### FlowLab AI (Predictive Traffic Forecasting Engine)

<img width="1919" height="774" alt="FlowLab AI Forecasting Interface" src="https://github.com/user-attachments/assets/a8ceaa67-0b3e-4e54-b953-1b039f955a30" />

FlowLab AI extends the core platform with a 24-hour ahead forecasting capability, generating road-level traffic volume predictions to support proactive congestion management.

#### Model Architecture

- Gradient boosting via XGBoost with road-specific model segmentation
- Autoregressive hour-by-hour forecasting logic for temporal coherence

#### Feature Engineering

- Lag-based hourly traffic volume features
- Rolling mean congestion trend indicators
- Cyclical hour-of-day encoding
- Weekday behavioural pattern learning
- Road capacity constraint integration
- Class-weighted training schema to emphasise congestion-state prediction accuracy

#### Forecast Outputs

- Hourly predicted traffic volume
- Forecasted V/C ratios
- Projected LOS grading

The system is oriented toward operational forecasting — anticipating congestion conditions before they materialise rather than describing them post-hoc.

---

### FlowLab Pulse (CCTV Health & Event Intelligence)

<img width="1310" height="613" alt="FlowLab Pulse Monitoring Interface" src="https://github.com/user-attachments/assets/b0c8f59c-d390-4b83-911f-7b47472b81dd" />

FlowLab Pulse is an operational reliability platform for surveillance-based traffic monitoring infrastructure. It provides command centre operators with continuous visibility into the health, availability, and performance of CCTV-based detection networks.

#### System Functions

- Live connectivity status monitoring across the CCTV estate
- Uptime and downtime analytics with historical trend tracking
- Silent failure detection for cameras reporting anomalously low activity
- Incident trend analysis and historical event review
- Snapshot viewer with AI detection overlay integration

---

## Real-Time Streaming Data Architecture

The underlying data infrastructure powering both FlowLab and FlowLab Pulse is a production-ready ingestion and serving pipeline designed for continuous, high-throughput operation.

#### Architecture Stack

- **RabbitMQ** — Event streaming and message queuing layer
- **PostgreSQL** — Structured storage with historical indexing
- **FastAPI** — Secure, performant API serving layer

#### Design Principles

- Strict separation of ingestion and analytics concerns
- Scalable CCTV AI event streaming without batch dependency
- Structured query interfaces for dashboard consumption
- CSV-ready endpoints for downstream system integration

---

## MaxHub Suite (Internal Traffic Report Automation Framework)

<img width="880" height="641" alt="MaxHub CLI Workflow" src="https://github.com/user-attachments/assets/e444d1d3-f798-4966-a412-02139643cb24" />

MaxHub is a modular, CLI-based automation framework that standardises traffic data workflows across operations teams. It converts fragmented CCTV export data into validated, submission-ready reports through a structured pipeline of discrete, composable components.

#### Components

**MaxForm**
Connects to Alibaba MaxCompute to retrieve CCTV volume and speed data. Applies preprocessing routines and threshold-based imputation to resolve data integrity issues at ingestion.

**MaxValid**
Performs systematic validation across ingested records, covering missing value detection, null record identification, and hourly interval completeness verification.

**MaxGen**
Generates multi-sheet Excel reports with automated LOS computation and structured formatting conforming to official submission standards.

**MaxCheck**
Executes CCTV-wide data quality scans using threshold-based performance criteria to flag cameras failing minimum data reliability requirements.

MaxHub embodies the principles of data governance enforcement, workflow automation at scale, and repeatable reporting infrastructure — qualities essential to operational consistency in live traffic management environments.

---

## Technical Stack

| Domain | Technologies |
|---|---|
| **Languages** | Python, SQL, Power Query M |
| **Machine Learning** | XGBoost, Time-Series Feature Engineering, Congestion Modelling |
| **Backend & APIs** | FastAPI, RabbitMQ, PostgreSQL |
| **Data Infrastructure** | Alibaba MaxCompute, OSS, MS SQL Server |
| **Visualisation** | Streamlit, Power BI, Matplotlib, QGIS |
| **Transport Engineering** | Level of Service Modelling, Corridor Flow Analytics, PTV Visum |

---

## Engineering Philosophy

The design of these systems reflects a set of considered principles developed through operational experience:

- **Systems over scripts** — sustainable architecture takes precedence over ad-hoc solutions
- **Infrastructure over notebooks** — production reliability demands structured engineering, not exploratory tooling
- **Reliability over visual polish** — operational utility is measured by uptime and accuracy, not aesthetics
- **Operational clarity over academic benchmarks** — performance is evaluated against real-world constraints
- **Automation first** — repetitive workflows are systematically eliminated through tooling
- **Data quality before analytics** — no insight is valid if the underlying data is not trustworthy

---

## Domain Focus

- Smart City Traffic Operations
- CCTV-Based Vehicle Intelligence
- Corridor Congestion Forecasting
- Command Room Systems Engineering
- Urban Traffic Data Infrastructure

---

## Contact

- **GitHub:** [github.com/N-M-Danial](https://github.com/N-M-Danial)
- **Email:** nik.muhammad.danial94@email.com
