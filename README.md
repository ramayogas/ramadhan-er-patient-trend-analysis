# Ramadhan ER Patient Trend Analysis

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow?style=flat)
<!-- ![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat) -->

**Tool:** SQL (PostgreSQL) · Power BI  
**Domain:** Healthcare  
**Dataset:** Simulated Dataset

> Dataset is fully simulated and anonymized. No real patient or hospital data is used.

A healthcare analytics project focused on identifying Emergency Room (ER) visit and diagnosis trends before, during, and after Ramadhan using PostgreSQL and Power BI.

---

## Overview

Hospitals often experience operational pattern shifts during Ramadhan, including changes in ER visit volume, patient arrival behavior, and diagnosis distribution. Understanding these trends helps hospitals optimize staffing, resource allocation, and emergency preparedness.

This project analyzes ER patient visits across three periods:

- **3 months before Ramadhan**
- **During Ramadhan**
- **3 months after Ramadhan**

The analysis focuses on patient visit trends and diagnosis patterns to generate actionable operational insights through SQL analysis and BI dashboards.

**Dataset:** Simulated ER patient visit records  
**Database:** PostgreSQL  
**Visualization:** Power BI  
**Domain:** Healthcare Analytics / Emergency Room Operations

---

## Problem Statement

This project aims to answer the following business questions:

1. How do ER patient visit trends change during the 3 months before Ramadhan?
2. What diagnosis categories are most common before Ramadhan?
3. How do ER visits and diagnosis trends change during Ramadhan?
4. What operational patterns emerge after Ramadhan?
5. Which diagnosis categories consistently dominate across all periods?
6. Are there shifts in peak visit periods and patient distribution during Ramadhan?

The goal is to support hospital operational decision-making through data-driven insights and interactive dashboards.

---

## Pipeline

```text
raw_er_visits.csv
        ↓
01_raw_ingestion.sql      → Load raw CSV into PostgreSQL
        ↓
02_data_cleaning.sql      → Standardize and validate data
        ↓
03_final_tables.sql       → Build cleaned analytical tables
        ↓
04_analysis.sql           → Trend & diagnosis analysis
        ↓
05_dashboard_export.sql   → Export aggregated BI datasets
        ↓
dashboard/
        ↓
Power BI Dashboard
