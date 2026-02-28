# 🚗 Chicago Residential Parking Permit Zones (2015–2026)
### Street Segment-Level Residential Parking Zone Designations — Standard & Buffer  
**EDA + Four Pillars of Data Analytics + Executive Dashboard (Notebook Project)**

> A clean, publication-ready analytics notebook that explores Chicago’s Residential Parking Permit Zones at the street-segment level—covering descriptive, diagnostic, predictive, and prescriptive analytics with consistent visuals and a unified “Chicago Midnight Teal” theme.

---

## Contents
- [Project Overview](#project-overview)
- <!--citation:1-->
- [Repository Structure](#repository-structure)
- [Analytics Framework: The Four Pillars](#analytics-framework-the-four-pillars)
- [Dashboard & Visual Theme](#dashboard--visual-theme)
- [How to Run (Local)](#how-to-run-local)
- [How to Run (Notebook / Colab)](#how-to-run-notebook--colab)
- [Modeling Notes](#modeling-notes)
- <!--citation:2-->
- [Data Ethics & License](#data-ethics--license)
- <!--citation:3-->

---

## Project Overview
This repository contains a **book-like Jupyter Notebook** that performs:
- End-to-end **Exploratory Data Analysis (EDA)**
- The **Four Major Pillars of Data Analytics**
- A compact **Executive Dashboard** (multi-panel summary)
- A consistent UI/visual identity across plots and highlights

The focus is on generating insights that could support:
- Urban planning
- Parking enforcement strategy
- Legislative impact analysis
- GIS-ready segmentation logic (street segments, not polygons)

---

## Dataset
**Title:** Chicago Residential Parking Permit Zones (2015–2026)  
**Portal:** Chicago Open Data Portal  
**Dataset Page:** `https://data.cityofchicago.org/d/u9xt-hiju`  
**Download Used by Notebook (CSV API):**
- `https://data.cityofchicago.org/api/views/u9xt-hiju/rows.csv?accessType=DOWNLOAD`

**What the data represents**
- Each record is a **street segment** that belongs to a **Residential Parking Zone**
- Zones are defined via **Chicago City Council legislation**
- Two segment types:
  - **Standard:** physical signage exists
  - **Buffer:** no signage, but residents can purchase permits; may overlap other segments

**Core columns used**
- `zone`, `street_direction`, `street_name`, `street_type`
- `odd_even`
- `addr_low`, `addr_high` (address range)
- `ward_low`, `ward_high`
- `buffer` and derived `is_buffer`

---

## Repository Structure
Recommended structure (adjust if needed):

```text
.
├── notebook/
│   └── chicago_parking_zones_eda.ipynb
├── outputs/
│   └── chicago_parking_dashboard.png

├── data/                       # optional if you store a snapshot
│   └── chicago_parking_zones.csv
├── requirements.txt
└── README.md
```
<img width="2315" height="1957" alt="a5f9efdc-63c9-43fe-a170-3250c9ba9b44" src="https://github.com/user-attachments/assets/4064e792-9974-46a9-bedc-548df135ea30" />
