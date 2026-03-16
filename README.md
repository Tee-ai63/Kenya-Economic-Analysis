# 🇰🇪 The Real Cost of Being Kenyan
## An Economic Analysis of Income, Inflation & Purchasing Power | 2018–2024

> *Nominal GDP per capita grew 54.5% between 2018 and 2024.  
> Real GDP per capita grew 8.4%.  
> The difference is the story.*

---

## 📋 Project Overview

This project uses publicly available government and international data 
to answer one central question: **has the average Kenyan's real 
purchasing power actually improved — or has income growth been an 
illusion created by rising prices?**

The analysis covers inflation erosion, real wage decline, CPI category 
breakdowns, fuel price shocks, income inequality in inflation burden, 
and the fiscal policy context behind Kenya's cost of living crisis 
from 2018 to 2024.

**Tools used:** Python · pandas · matplotlib · seaborn · SQLite · 
Power BI · DAX

**Data sources:** World Bank · IMF WEO · KNBS Economic Survey 2024 · 
Central Bank of Kenya

---

## Key Findings

| Finding | Number |
|---------|--------|
| Nominal GDP/capita growth 2018–2024 | +54.5% |
| Real GDP/capita growth 2018–2024 | +8.4% |
| Purchasing power of KES 1,000 by 2024 | KES 701 |
| Real private sector wage change 2019–2023 | -9.2% |
| Food price increase 2019–2023 | +46.8% |
| Transport price increase 2019–2023 | +48.2% |
| Petrol price increase 2019–2023 | +77.4% |
| Peak government debt (2023) | 73.1% of GDP |
| Inflation gap: lower vs upper income (2020) | +3.6pp |
| Household health score 2023 | 1/5 — Critical |

---

## 📁 Project Structure
```
kenya-economic-analysis/
│
├── app.ipynb                 # Data ingestion & cleaning pipeline
├── eda.ipynb                 # Exploratory data analysis & charts
├── sql_analysis.ipynb        # SQLite analysis — 8 queries
│
├── data/
│   └── cleaned/              # 7 cleaned CSV files
│       ├── master_annual.csv         # Master dataset (7 rows × 45 cols)
│       ├── knbs_wages.csv            # Wages by sector & industry
│       ├── knbs_cpi_categories.csv   # CPI by 13 categories
│       ├── knbs_inflation_income.csv # Inflation by income group
│       ├── energy_fuel_prices.csv    # Fuel prices 2019–2023
│       ├── imf_macro.csv             # IMF fiscal indicators
│       └── wb_macro.csv              # World Bank macro indicators
│
└── visuals/
    ├── chart1_nominal_vs_real_growth.png
    ├── chart2_purchasing_power.png
    ├── chart3_cpi_by_category.png
    ├── chart4_nominal_vs_real_wages.png
    ├── chart5_inflation_by_income.png
    └── chart6_fuel_prices.png
```

---

## Charts

### The Illusion of Growth
![Chart 1] :
<img width="1484" height="732" alt="chart1_nominal_vs_real_growth" src="https://github.com/user-attachments/assets/c236c7db-9d17-49ec-afe2-daca442b8983" />


### The Shrinking Shilling : 
<img width="1485" height="732" alt="chart2_purchasing_power" src="https://github.com/user-attachments/assets/517f5fcd-1280-4aae-9bfb-3c007463091b" />


### What Rose Fastest : 
<img width="1785" height="1032" alt="chart3_cpi_by_category" src="https://github.com/user-attachments/assets/303f3311-7cee-4267-b326-4ade78411749" />


### The Pay Rise That Was Not : 
![Chart 4] : 
<img width="1485" height="732" alt="chart4_nominal_vs_real_wages" src="https://github.com/user-attachments/assets/0f473295-cff6-4ee0-af3e-c8d89c070d60" />

### The Poor Pay More
![Chart 5] :
<img width="1484" height="732" alt="chart5_inflation_by_income" src="https://github.com/user-attachments/assets/e99dda54-1a47-4a1d-ab21-1d8e7ad08926" />


### The Fuel Shock
![Chart 6] : 
<img width="1479" height="732" alt="chart6_fuel_prices" src="https://github.com/user-attachments/assets/453cebd2-30d4-4eeb-ba69-a3f43861912f" />


## 🗄️ SQL Analysis

8 queries built against a SQLite database covering:

| Query | Concept | Question |
|-------|---------|----------|
| Q1 | SELECT, ROUND, aliases | Nominal vs real growth gap by year |
| Q2 | WHERE, CASE WHEN | Economic regime classification |
| Q3 | GROUP BY, aggregates | Wage summary by sector |
| Q4 | JOIN, subqueries | Worst real wage declines by industry |
| Q5 | HAVING, nested subquery | CPI categories beating national average |
| Q6 | LAG() window function | Year-on-year debt and savings shifts |
| Q7 | CTE, weighted index | Wage illusion vs household cost burden |
| Q8 | Composite scoring | Executive summary — household health |

---


## 👤 Author

** Tess Kamau **  
Data Analyst · Nairobi, Kenya  
LinkedIn : www.linkedin.com/in/tesskamau-a23708354


*Built as a portfolio project demonstrating end-to-end data analysis 
across Python, SQL, and Power BI using real Kenyan economic data.*
