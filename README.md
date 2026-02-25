# Bus Terminal Ridership Forecasting & Data Warehouse Design

## Table of Contents

- [Project Overview](#project-overview)
- [System Architecture](#system-architecture)
- [Data Warehouse Schema](#data-warehouse-schema)
- [Historical Trend Analysis](#historical-trend-analysis)
- [Long-Term Forecasting (2026–2030)](#long-term-forecasting-20262030)
- [Yearly Ridership Forecast (2026–2030)](#yearly-ridership-forecast-20262030)
- [Carrier-Level Forecasting](#carrier-level-forecasting)
- [Tech Stack](#tech-stack)
- [System Requirements](#system-requirements)
- [Installation Guide](#installation-guide)
- [Design Decisions](#design-decisions)
- [Power BI Dashboard](#power-bi-dashboard)
- [Business Use Case](#business-use-case)
- [How to Run](#how-to-run)
- [Academic Context](#academic-context)
- [Repository Structure](#repository-structure)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

## Project Overview

This project analyzes historical bus terminal ridership data and develops a structured data warehouse along with long-term passenger forecasting (2026–2030).

The solution integrates:

- Data Cleaning & Preprocessing (Python)
- Dimensional Data Warehouse Design (SQL – Star Schema)
- Time Series Forecasting
- Carrier-Level Ridership Modeling
- Business Intelligence Visualization (Power BI)

The objective is to enable data-driven decision-making for capacity planning, operational optimization, and strategic forecasting.

## System Architecture

The project follows a complete data analytics pipeline:

```
Raw Data (Excel)
↓
Data Cleaning & Feature Engineering (Python)
↓
SQL Data Warehouse (Star Schema)
↓
Time Series Forecasting Model
↓
Power BI Dashboard & Visual Analytics
```

## Data Warehouse Schema

The dimensional model includes:

- FACT_RIDERSHIP (Fact Table)
- DIM_DATE
- DIM_CARRIER
- DIM_SERVICE_TYPE
- DIM_EXTERNAL_FACTORS

![data_warehouse_schema png](https://github.com/user-attachments/assets/949d62fb-c42f-4c41-a3fd-42816026d862)


## Historical Trend Analysis

Monthly ridership trends were analyzed to identify:

- Seasonality patterns
- Growth trends
- Demand fluctuations
- Year-over-year increases

![monthly_historical_trend png](https://github.com/user-attachments/assets/5d43b0bf-c3c2-4af7-beaf-52f62de1e1df)


Key Observations:

- Strong seasonal variation across months
- Increasing yearly ridership trend
- Mid-year peak demand periods

## Long-Term Forecasting (2026–2030)

A time-series forecasting model was developed to project future ridership demand.

The model captures:

- Trend components
- Seasonality
- Long-term growth trajectory

![monthly_forecast_combined png](https://github.com/user-attachments/assets/7d4b7dbb-6166-4f92-99a6-f2dd0051ca70)


## Yearly Ridership Forecast (2026–2030)

Annual passenger totals were projected to evaluate long-term growth.

![yearly_forecast_2026_2030 png](https://github.com/user-attachments/assets/0fb5d951-f41e-4e8a-bce1-d15ab83bc190)


The forecast indicates consistent upward growth through 2030.

## Carrier-Level Forecasting

Carrier-level segmentation analysis was performed to evaluate performance differences and demand patterns.

![carrier_level_forecast png](https://github.com/user-attachments/assets/55a09cbe-20cc-4a3f-b876-f0076c317eef)


This analysis supports:

- Carrier performance benchmarking
- Resource allocation optimization
- Strategic operational planning

## Tech Stack

### Programming & Analytics
- Python
- SQL
- Power BI

### Python Libraries
- Pandas
- NumPy
- Matplotlib
- Prophet (Time Series Forecasting)

### Data Modeling
- Star Schema Design
- Fact & Dimension Tables
- SQL Warehouse Implementation

## System Requirements

Before running the project locally, ensure the following:

- Python 3.8+
- Jupyter Notebook
- Power BI Desktop (Latest Version)
- SQL Server / MySQL (for warehouse schema execution)
- Git (for cloning the repository)

Required Python Libraries:

- pandas
- numpy
- matplotlib
- prophet

## Installation Guide

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Bus-Terminal-Ridership-Forecasting.git
```

### 2. Install Required Python Libraries

```bash
pip install pandas numpy matplotlib prophet
```

### 3. Run Notebooks

- Open data_preprocessing.ipynb
- Execute long_term_forecasting.py.ipynb

### 4. Open Power BI Dashboard

- Open .pbix files in Power BI Desktop


## Design Decisions

### Technology Stack

- Python for data preprocessing and forecasting
- SQL for dimensional warehouse modeling
- Power BI for visualization and reporting

### Data Modeling

- Implemented Star Schema architecture
- Created Fact and Dimension tables
- Optimized joins for aggregation performance

### Forecasting Approach

- Time series modeling using Prophet
- Incorporated trend and seasonality components
- Generated multi-year forecast projections (2026–2030)

### Visualization Design

- Clean executive-style dashboards
- Clear hierarchy of KPIs
- Segmented carrier comparison
- Trend + forecast visualization layering

## Power BI Dashboard

The Power BI dashboards provide:

- Interactive ridership visualization
- Trend exploration
- Carrier comparison
- Forecast display
- Operational insights

Dashboard files:

- Fall 2025_BANL-6430-02_Group 5_Dashboard.pbix
- Visualizations.pbix

## Business Use Case

This project enables:

- Data-driven ridership prediction
- Long-term infrastructure planning
- Capacity management decisions
- Carrier performance evaluation
- Scalable analytics architecture

## How to Run

1. Execute `data_preprocessing.ipynb` to clean and structure the dataset.
2. Run `long_term_forecasting.py.ipynb` to generate long-term projections (2026–2030).
3. Use the SQL scripts to create the Star Schema warehouse.
4. Open the `.pbix` files in Power BI Desktop to interact with dashboards and forecast visualizations.

## Academic Context

This project was completed as part of BANL-6430 Business Analytics coursework and demonstrates integration of:

- Data Engineering
- Predictive Modeling
- Data Warehousing
- Business Intelligence Visualization

## Repository Structure

```
Bus-Terminal-Ridership-Forecasting/
│
├── data_preprocessing.ipynb
├── long_term_forecasting.py.ipynb
├── Combined_Tables.xlsx
├── Fall 2025_BANL-6430-02_Group 5_Dataset.sql
├── Data_Warehouse_Tables.sql
├── Fall 2025_BANL-6430-02_Group 5_Dashboard.pbix
├── Visualizations.pbix
├── Final Project Report.docx
├── Final Project Presentation.pptx
├── SQL_SchemaDesign.docx
├── Data Cleaning and Preprocessing.docx
├── Long-Term Forecasting (2026-30).docx
├── Predictive Factors and Carrier Level Forecasting.docx
├── PowerBI Visualization.docx
└── README.md
```

## Future Enhancements

- Real-time ridership API integration
- Weather-based ridership impact modeling
- Machine learning model comparison (ARIMA, LSTM)
- Automated ETL pipeline
- Interactive forecasting dashboard in Power BI

## Author

**Sujeeth Parikipandla**  
Graduate Student – Business Analytics  
Focused on Predictive Modeling, Data Warehousing & Business Intelligence
