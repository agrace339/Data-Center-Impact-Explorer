# Data Center Impact Explorer

*Drexel University MS in Data Science Capstone I*

A data science capstone project analyzing the relationship between data centers and surrounding communities across the United States and investigating the potential impacts of data center development on local areas.

The project integrates multiple public datasets with data from the the FracTracker Alliance U.S. Data Centers Tracker to explore factors that may influence where data centers are built and existing conditions or issues within the surrounding areas that could potentially be exacerbated by data center development.

---

## Team

- Anna Grace
- Jillian Kunze
- Andrea MacGregor
- Morgan Murphy

---

## Project Objectives

This project explores several research questions related to data center development, including the following:

- Data centers have a high water demand; are they located in areas already prone to drought, when they might pose additional strain? 
- Data centers also have high electricity demand; what are the conditions for electricity production and pricing where they are located? 
- Data centers produce pollution that can cause or exacerbate certain health conditions; what are the existing health concerns in local communities that could be aggravated?
- Local governments play a role in data center siting in terms of zoning, permitting, and incentives; what are the political conditions in areas with data centers?

---

## Repository Structure

```
<mark>Everyone can add their data to the folder as needed and then record it here -- but please be extra careful about permissions for reposting data!!!</mark>
Data/
│
├── Data_Centers_Database - FracTracker Data Centers.csv
├── Electricity/
├── Politics/
├── Health/
└── Drought/

Script/
│
├── Inspection Data Centers and Politics.ipynb
├── Dev_ZIP_to_FIPS.ipynb
├── Preprocessing AEO2026.ipynb
├── Preprocessing ELEC.ipynb
├── Preprocessing Politics.ipynb
├── Health_Data_Cleaning_and_Investigation.ipynb
├── Industrial Electricity Prices with AEO2026.ipynb
├── Build State-Year ELEC Dataset.ipynb
├── EDA ELEC.ipynb
├── EDA Politics.ipynb
└── EDA Drought.ipynb
```
<mark>Should we divide up the Script folder into sub-folders, since we have so many files in there now?</mark>

<mark>We should also probably add a folder with all our presentations/reports</mark>

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

<mark> Note which data is included in the repository and which is not</mark>

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
