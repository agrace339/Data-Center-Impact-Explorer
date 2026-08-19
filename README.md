# Data Center Impact Explorer

*Drexel University MS in Data Science Capstone I*

A data science capstone project analyzing the relationship between data centers and surrounding communities across the United States and investigating the potential impacts of data center development on local areas.

The project integrates multiple public datasets with data from the the FracTracker Alliance U.S. Data Centers Tracker to explore factors that may influence where data centers are built and existing conditions or issues within the surrounding areas that could potentially be exacerbated by data center development.

Note: The public StreamLit site is in the works. The link will be pasted here when complete. 

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
Data/
│
├── Electricity/
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
├── Commercial Electricity Prices with AEO2026.ipynb
├── Industrial Electricity Prices with AEO2026.ipynb
├── Build State-Year ELEC Dataset.ipynb
├── EDA ELEC.ipynb
├── EDA Politics.ipynb
├── EDA Drought.ipynb
└── Data_Center_Grid_Strain_Findings.ipynb

Presentations and Reports/
│
├── Launch Report.pdf
├── Launch Presentation.pdf
├── Pitch Presentation.pdf
├── Data Acquisition and Pre-processing Report.pdf
├── EDA Presentation.pdf
└── Final Presentation.pdf

```

*Please note that datasets will be added to the structure shown above as republishing permissions allow*

---

## Data Sources

The project combines several publicly available datasets, as follows. Some data is permitted for reproduction while some is not, so please see below for details and instructions for acquiring data if necessary.  

### Data on Data Centers

* [FracTracker Alliance U.S. Data Centers Tracker](https://experience.arcgis.com/experience/5a4d072ad01449bba5698a80103fb909/page/About): Contains over 1,500 individual data centers in the U.S. with their precision locations and additional information. The data is allowed to be downloaded, shared, and used as long as proper credit is given to FracTracker; however, accessing the data requires agreeing to FracTracker terms and conditions which we are not able to replicate here, so please download the data from the link if you wish to reproduce our work.

### Data on Drought

* [U.S. Drought Monitor Site](https://droughtmonitor.unl.edu/CurrentMap.aspx): Tracks the drought across the U.S. on a weekly basis. The data can be used in tandem with this blurb: The U.S. Drought Monitor is jointly produced by the National Drought Mitigation Center at the University of Nebraska-Lincoln, the United States Department of Agriculture, the National Oceanic and Atmospheric Administration and the National Aeronautics and Space Administration. Map courtesy of NDMC.

### Data on Electricity

* [U.S. Energy Information Administration (EIA) Bulk Data](https://www.eia.gov/opendata/v1/bulkfiles.php): Provides extensive information on electricity generation, customer counts, retail electricity prices, and other energy-related statistics across the United States.

### Data on Health

* [America’s Health Rankings (AHR) 2025 Annual Report](https://www.americashealthrankings.org/publications/reports/2025-annual-report) data provided by the United Health Foundation: Synthesizes data from over 50 reputable, publicly available data sources and includes over 250 measures related to U.S. public health. The report and dataset is public access and free to use, with no account required for access or download. Redistribution of this data is permitted for educational and non-profit purposes. 
* [2024 National Health Interview Survey (NHIS)](https://www.cdc.gov/nchs/nhis/documentation/2024-nhis.html), conducted and published by the National Center for Health Statistics: Information about physical and mental health conditions, disabilities, and health care access at the region level. Redistribution of this dataset is not permitted; however, it is also public access and free to use, with the only requirement explicitly stated being proper attribution of credit to the NCHS.

### Data on Politics

* [National Neighborhood Data Archive (NaNDA) (ICPSR 38506)](https://www.icpsr.umich.edu/web/ICPSR/studies/38506#): Voter registration, turnout, and partisanship by county in the U.S. from 2004 to 2022. The data is public access as a TSV within a downloadable zip file with accompanying documentation, but requires having or making an account to download; redistribution of this dataset is not permitted, so the data is not included in this repository. 
* [American Local Government Elections Database](https://osf.io/mv5e6/overview): Local election results at the city and county level from 1989 to 2021. The data is open access under the CC-By Attribution 4.0 International license. This data was explored in `Inspection Data Center and Politics.ipynb` and `Preprocessing politics.ipynb` but ultimately found to not be comprehensive enough for our project goals, and so is not included in this repository.

### Supporting Data 

* [RowZero FIPS code lists and location mapping](https://rowzero.com/datasets/fips-codes-lookup) (specifically sheet titled “Zip to County”): Provides conversion from ZIP code to FIPS code, which is necessary for joining on location between e.g. the data center data and political data. This dataset is free to use but requires a Row Zero account to download, and so is not reposted in this repository.

---

## Repository Contents: Scripts 

Each notebook documents the preprocessing, data quality assessment, and exploratory analyses performed for its relevant work and respective dataset(s).

### Requirements
* `pandas`
* `matplotlib.pyplot`
* `seaborn`
* `urllib.request`
* `plotly`
* `numpy`
* `sklearn`

### Development

- `Inspection Data Centers and Politics.ipynb`: Initial inspection of primary data centers dataset and data related to political factors
- `Dev_ZIP_to_FIPS.ipynb`: Development of ZIP code to FIPS code (county indentifier) conversion workflow
- `Industrial Electricity Prices with AEO2026.ipynb`
- `Commercial Electricity Prices with AEO2026.ipynb`

### Preprocessing

- `Build State-Year ELEC Dataset.ipynb`
- `Health_Data_Cleaning_and_Investigation.ipynb`
- `Preprocessing AEO2026.ipynb`
- `Preprocessing ELEC.ipynb`: Data cleaning and pre-processing for electricity dataset
- `Preprocessing Politics.ipynb`: Data cleaning and pre-processing for political datasets

### Exploratory Data Analysis

EDA notebooks examining:

- Electricity and power infrastructure (`EDA ELEC.ipynb` and `Data_Center_Grid_Strain_Findings.ipynb`)
- Political indicators (`EDA Politics.ipynb`)
- Drought conditions (`EDA Drought.ipynb`)

---

## Presentations and Reports

We include the presentations and written reports prepared as part of this capstone project in Drexel University course DSCI 591, which can be understood in sequential order: 

- `Launch Report.pdf`: Initial proposal of project, plan of work, and description of team background
- `Launch Presentation.pdf`: Presentation following launch report, with initial data inspection
- `Pitch Presentation.pdf`: Presentation with more detailed background and data overview and inspection
- `Data Acquisition and Pre-processing Report.pdf`: Report describing data sources and pre-processing steps in detail
- `EDA Presentation.pdf`: Presentation of in-progress exploratory data analysis and visualization
- `Final Presentation.pdf`: Presentation of final findings and summary of project

---

## References

### Data Used in Final Analysis and Visualization 

- Clary, W., Gomez-Lopez, I. N., Chenoweth, M., Gypin, L., Clarke, P., Noppert, G., Li, M., & Kollman, K. (2024). National Neighborhood Data Archive (NaNDA): Voter Registration, Turnout, and Partisanship by County, United States, 2004-2022 [Data set]. *Inter-university Consortium for Political and Social Research*. https://www.icpsr.umich.edu/web/ICPSR/studies/38506/versions/V2
- FracTracker. (2026, July). U.S. Data Centers Tracker [Data set]. *FracTracker Alliance*. https://experience.arcgis.com/experience/5a4d072ad01449bba5698a80103fb909/page/Demographics 
- National Center for Health Statistics. (2024). 2024 NHIS Questionnaire, Datasets, and Documentation [Data set]. *U.S. Centers for Disease Control and Prevention*. https://www.cdc.gov/nchs/nhis/documentation/2024-nhis.html
- National Center for Health Statistics. (2024). 2024 NHIS Questionnaire, Datasets, and Documentation [Codebook]. *U.S. Centers for Disease Control and Prevention*. https://www.cdc.gov/nchs/nhis/documentation/2024-nhis.html
- Row Zero. (2025, March 6). *FIPS codes for all U.S. locations in a spreadsheet* [Data set]. https://rowzero.com/datasets/fips-codes-lookup#zip-code-mappings
- United Health Foundation (2025). America's Health Rankings 2025 annual report [Data set]. *America’s Health Rankings*. https://www.americashealthrankings.org/publications/reports/2025-annual-report
- United Health Foundation. (2025). 2025 Annual Report: Measures table. *America's Health Rankings*. https://assets.americashealthrankings.org/ahr_2025annual_measurestable_final-web.pdf
- U.S. Drought Monitor. (n.d.). Data Tables [Data set]. *U.S. Drought Monitor*. https://droughtmonitor.unl.edu/DmData/DataTables.aspx
- U.S. Energy Information Administration (2025). *EIA Bulk Data* [Data set]. https://www.eia.gov/opendata/

### Other Data Inspected 

- de Benedictis-Kessner, J., Lee, D. D. I., Velez, Y. R., & Warshaw, C. (2023). American local government elections database. *Scientific Data*, *10*(1), 912.
- de Benedictis-Kessner, J., Lee, D., Velez, Y. R., & Warshaw, C. (2023, May 16). *American Local Government Elections Database* [Data set]. Retrieved from osf.io/mv5e6. 

### Background Materials

- CDC. (2024). NCHS Urban-Rural Classification Scheme for Counties. *National Center for Health Statistics*. https://www.cdc.gov/nchs/data-analysis-tools/urban-rural.html
- Federal Communications Commission. (n.d.). *Federal Information Processing System (FIPS) Codes for States and Counties*. https://transition.fcc.gov/oet/info/maps/census/fips/fips.txt 
- Han, Y., Wu, Z., Li, P., Wierman, A., & Ren, S. (2024). *Health-Informed Computing: Estimating and Addressing the Public Health Impact of Data Centers*. https://arxiv.org/abs/2412.06288
- Jones, J.M. (2026, May 13). Americans oppose AI data centers in their area. *Gallup*. https://news.gallup.com/poll/709772/americans-oppose-data-centers-area.aspx
- Malone, K. (2026, February 16). A quick guide to Pennsylvania’s data center debate. *Technical.ly*. https://technical.ly/civics/pennsylvania-data-centers-explained/ 
- National League of Cities & AAAS Center for Scientific Evidence in Public Issues (EPI Center). (n.d.). *Community strategies to address data center development and operation*.
- Pate, C. A., Akinbami, L. J., Johnson, C., Hsu, J., & Zahran, H. S. (2025). Asthma and Allergy Comorbidity Among the US Population Aged 2 Years or Older, National Health Interview Survey, 2021. *Public health reports (Washington, D.C. : 1974)*, *140*(5-6), 540–550. https://doi.org/10.1177/00333549251358658   
- Pavlinich, E. J. (2026). *The Dangers of Data Centers. Environmental Health Project*. Retrieved from https://www.environmentalhealthproject.org/post/the-dangers-of-data-centers 
- Stansbury, M., Marchese, K., Hardin, K., & Amon, C. (2025, June 24). Can US infrastructure keep up with the AI economy? *Deloitte Insights*. 
https://www.deloitte.com/us/en/insights/industry/power-and-utilities/data-center-infrastructure-artificial-intelligence.html
- United States Census Bureau (n.d.). Geographic Levels. *Guidance for Economic Census Geography Users*. https://www.census.gov/programs-surveys/economic-census/guidance-geographies/levels.html 

