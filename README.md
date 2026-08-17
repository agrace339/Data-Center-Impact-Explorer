# Data Center Impact Explorer

*Drexel University MS in Data Science Capstone I*

A data science capstone project analyzing the relationship between data centers and surrounding communities across the United States and investigating the potential impacts of data center development on local areas.

The project integrates multiple public datasets with data from the the FracTracker Alliance U.S. Data Centers Tracker to explore factors that may influence where data centers are built and existing conditions or issues within the surrounding areas that could potentially be exacerbated by data center development.

<mark>Add link to StreamLit site</mark>

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

<mark>Everyone can add their data to the folder as needed and then record it here -- but please be extra careful about permissions for reposting data!!!</mark>

```
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

The project combines several publicly available datasets, as follows. 

**Data on Data Centers**

* [FracTracker Alliance U.S. Data Centers Tracker](https://experience.arcgis.com/experience/5a4d072ad01449bba5698a80103fb909/page/About): Contains over 1,500 individual data centers in the U.S. with their precision locations and additional information. The data is allowed to be downloaded, shared, and used as long as proper credit is given to FracTracker. <mark>Should we include this data in the repository or not?</mark>

**Data on Drought**

* <mark>Add here - note source(s), reuse permissions, whether data is reposted in this repository</mark>

**Data on Electricity**

* <mark>Add here - note source(s), reuse permissions, whether data is reposted in this repository</mark>

**Data on Health**

* <mark>Add here - note source(s), reuse permissions, whether data is reposted in this repository</mark>

**Data on Politics**

* [National Neighborhood Data Archive (NaNDA) (ICPSR 38506)](https://www.icpsr.umich.edu/web/ICPSR/studies/38506#): Voter registration, turnout, and partisanship by county in the U.S. from 2004 to 2022. The data is public access as a TSV within a downloadable zip file with accompanying documentation, but requires having or making an account to download; redistribution of this dataset is not permitted, so the data is not included in this repository. 
* [American Local Government Elections Database](https://osf.io/mv5e6/overview): Local election results at the city and county level from 1989 to 2021. The data is open access under the CC-By Attribution 4.0 International license. This data was explored in `Inspection Data Center and Politics.ipynb` and `Preprocessing politics.ipynb` but ultimately found to not be comprehensive enough for our project goals, and so is not included in this repository. 

---

## Repository Contents: Scripts 

### Development

- `Inspection Data Centers and Politics.ipynb`: Initial inspection of primary data centers dataset and data related to political factors
- `Dev_ZIP_to_FIPS.ipynb`: Development of ZIP code to FIPS code (county indentifier) conversion workflow
- `Industrial Electricity Prices with AEO2026.ipynb`: <mark>Add description, move to different section if needed</mark>

### Preprocessing

- `Build State-Year ELEC Dataset.ipynb`: <mark>Add description, move to different section if needed</mark>
- `Health_Data_Cleaning_and_Investigation.ipynb`: <mark>Add description, move to different section if needed</mark>
- `Preprocessing AEO2026.ipynb`: <mark>Add description</mark>
- `Preprocessing ELEC.ipynb`: Data cleaning and pre-processing for electricity dataset
- `Preprocessing Politics.ipynb`: Data cleaning and pre-processing for political datasets

### Exploratory Data Analysis

EDA notebooks examining:

- Electricity and power infrastructure (`EDA ELEC.ipynb`)
- Political indicators (`EDA Politics.ipynb`)
- Health datasets <mark>(Is there a notebook for this or is it all in Tableau?)</mark>
- Drought conditions (`EDA Drought.ipynb`)

Each notebook documents the preprocessing, data quality assessment, and exploratory analyses performed for its respective dataset.

<mark>Could link off here to Tableau sites, StreamLit again, etc.</mark>

## <mark>Add section for supplementary materials?</mark>

<mark>Reports, presentations, etc.</mark>

## References

<mark>Add here</mark>
