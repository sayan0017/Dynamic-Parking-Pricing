# dynamic-parking-pricing
Dynamic Pricing for Urban Parking Lots- Prices that remain static throughout the day can lead to inefficiencies — either overcrowding or underutilization. To improve utilization, dynamic pricing based on demand, competition, and real-time conditions is crucial.
# 🚗 Dynamic Pricing for Urban Parking Lots

**Capstone Project | Summer Analytics 2025**  
**Hosted by: Consulting & Analytics Club × Pathway**

---

## 📌 Overview

Urban parking spaces are limited and demand varies throughout the day.  
Static pricing often causes underutilization or overcrowding.  
This project builds an **intelligent, real-time dynamic pricing engine** for 14 urban parking lots using:
- **Historical occupancy**
- **Queue length**
- **Nearby traffic conditions**
- **Special events**
- **Vehicle type**
- **Competitor prices**

The goal: **Optimize revenue and utilization** while keeping price updates smooth and explainable.

---

## ⚙️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Python** | Core logic & data processing |
| **Pandas, NumPy** | Data manipulation & demand function |
| **Pathway** | Real-time data streaming simulation |
| **Bokeh** | Real-time interactive visualizations |
| **Google Colab** | Development & execution environment |
| **GitHub** | Version control & collaboration |

---

## 📊 System Architecture

```mermaid
flowchart TD
    A[Real-Time Data Stream - Pathway] --> B[Preprocessing - Pandas, NumPy]
    B --> C[Pricing Engine - Baseline and Demand-Based Models]
    C --> D[Smoothing and Constraints]
    C --> E[Competitor Price Logic - Haversine Distance]
    D --> F[Price Output Stream]
    E --> F
    F --> G[Bokeh Visualization]
    F --> H[Rerouting Suggestion if Overburdened]
