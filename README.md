# Data Center Impact Explorer

A data science capstone project investigating the environmental, infrastructure, political, and community impacts of data center development across the United States.

The project integrates multiple public datasets with the FracTracker Alliance Data Center Database to explore factors that may influence where data centers are built and how they affect surrounding communities.

---

## Team

- Anna Grace
- Jillian Kunze
- Andrea MacGregor
- Morgan Murphy

---

## Project Objectives

This project explores several research questions related to data center development, including:

- How do data centers impact local power infrastructure?
- Are there political factors associated with where data centers are developed?
- Do environmental conditions influence site selection?
- How can disparate public datasets be integrated for county-level analysis?

---

## Repository Structure

```
Data/
│
├── Data_Centers_Database - FracTracker Data Centers.csv
├── Electricity/
├── Politics/
├── Health/
└── Drought/

Script/
├── Dev_ZIP_to_FIPS.ipynb
├── Preprocessing ELEC.ipynb
├── Preprocessing Politics.ipynb
├── EDA ELEC.ipynb
├── EDA Politics.ipynb
├── EDA Health.ipynb
└── EDA Drought.ipynb
```

---

## Data Sources

The project combines several publicly available datasets, including:

- **FracTracker Alliance U.S. Data Center Database**
- **U.S. Energy Information Administration (EIA)** electricity data
- **MIT Election Data and Science Lab** political data
- **Area Health Resources (AHR)**
- **National Health Interview Survey (NHIS)**
- **National Survey on Drug Use and Health (NSDUH)**
- **U.S. Drought Monitor**

---

## Repository Contents

### Development

- ZIP code to county (FIPS) conversion workflow
- Data integration utilities
- County-level aggregation methods

### Preprocessing

Data cleaning and preparation for:

- Electricity data
- Political datasets

### Exploratory Data Analysis

EDA notebooks examining:

- Electricity and power infrastructure
- Political indicators
- Health datasets
- Drought conditions

Each notebook documents the preprocessing, data quality assessment, and exploratory analyses performed for its respective dataset.