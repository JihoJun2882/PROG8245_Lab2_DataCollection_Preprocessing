# Lab 2 – Data Collection & Pre-Processing

This project implements an end-to-end data pipeline on an e-commerce sample.
Data are loaded into pandas, validated, and cleaned (including de-duplication and field normalization).
Used small Class and Method for implement functions. New features are engineered and derived columns are added.
A secondary CSV is joined to append shipping_city from Country.
City-level total revenue is computed via groupby with Data Wrangler.
This notebook demonstrates reproducible data handling, cleaning, transformation, and aggregation.

## Quick‑start

 Python 3.11 or 3.12

 0) Open new terminal

 1) Virtual environment
  python -m venv venv

 - Activate virtual environment
 > Windows
 - venv\Scripts\activate
 > macOS/Linux
 - source venv/bin/activate

 2) Install packages
 - pip install -r requirements.txt

 3) Launch the notebook
 - Run All

## Repository layout (example)

```
.
├─ Lab2_DataCollection_PreProcessing.ipynb   # main notebook
├─ requirements.txt
├─ data/
│  ├─ 1000 Sales Records.csv                 # Primary (use first 500 rows)
│  ├─ concap.csv                             # Secondary (CountryName, CapitalName)
│  ├─ cleaned_data.csv / cleaned_data.json               # Step 11 outputs
│  └─ city_aggregate.csv / city_aggregate.json           # Step 10 outputs
└─ README.md
```

## Data sources (attribution)

- **Primary**: *1000 Sales Records* (ExcelBIAnalytics)  
  https://excelbianalytics.com/wp/downloads-18-sample-csv-files-data-sets-for-testing-sales/
- **Secondary**: *World capitals gps* (`concap.csv`) — `CountryName`, `CapitalName`  
  https://www.kaggle.com/datasets/nikitagrec/world-capitals-gps   - (Kaggle)

# Simple correction for items with different country names (6 countries)

## Outputs

- Cleaned transactions (`cleaned.csv` / `cleaned.json`)  
- City‑level aggregation (`city_agg.csv` / `city_agg.json`)  
- Data Dictionary: Markdown table

## List of other projects (links)

- Example • LinearRegressionArchitecture_Workshop — https://github.com/JihoJun2882/LinearRegressionArchitecture_Workshop.git
- Example • CSCN8010_LAB_1 - https://github.com/JihoJun2882/CSCN8010_LAB_1.git
- Example • PROG8431_week4 - https://github.com/JihoJun2882/PROG8431_week4.git