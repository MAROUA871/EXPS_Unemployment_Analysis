# Unemployment Analysis with Python

## Internship Project — EXPERT PETROLEUM SERVICES

This project was completed as part of my internship at **EXPERT PETROLEUM SERVICES**.

The objective of this project is to analyze unemployment trends across U.S. states and selected geographic areas using Python. The analysis covers data cleaning, validation, exploratory data analysis (EDA), historical trends, geographic differences, seasonal patterns, and the impact of the COVID-19 pandemic.

---

## Project Objectives

* Clean and validate a real-world unemployment dataset.
* Explore the distribution and variation of unemployment rates.
* Analyze historical unemployment trends over time.
* Investigate the impact of the COVID-19 pandemic.
* Compare unemployment rates across geographic entities.
* Identify seasonal patterns in unemployment.
* Examine the relationship between labor-force participation and unemployment.
* Identify major historical periods of unemployment increases and recovery.
* Present findings through tables, visualizations, and written analysis.

---

## Dataset

The dataset used in this project is:

**Unemployment in America Per US State.csv**

The dataset contains monthly unemployment data covering:

* **53 geographic entities**
* **1976–2025**
* **31,747 observations**
* U.S. states and selected local geographic areas

The dataset includes information such as:

* State/Area
* Year
* Month
* Civilian non-institutional population
* Civilian labor force
* Employment
* Unemployment
* Unemployment rate
* Labor-force participation-related measures

The raw dataset is located in:

```text
data/
└── raw/
    └── Unemployment in America Per US State.csv
```

---

## Data Cleaning and Validation

The dataset was systematically inspected and cleaned before analysis.

The cleaning and validation process included:

* Checking the dataset structure and dimensions.
* Standardizing column names.
* Inspecting and correcting data types.
* Converting numeric columns stored as strings into numeric values.
* Removing commas from numeric values.
* Detecting special missing-value codes.
* Replacing the special `–` values with `NaN`.
* Checking for missing values.
* Checking for duplicate observations.
* Validating categorical values.
* Validating year and month information.
* Converting relevant variables to appropriate numeric formats.

The final dataset contains **31,747 observations and 11 columns**.

The cleaned dataset is located in:

```text
data/
└── processed/
    └── unemployment_cleaned.csv
```

---

## Exploratory Data Analysis

### Historical Trends

The analysis examines unemployment trends from **1976 to 2025**, identifying:

* Long-term unemployment trends.
* Major periods of increasing unemployment.
* Periods of economic recovery.
* Differences between monthly and annual unemployment patterns.

### COVID-19 Impact

A specific part of the analysis focuses on the **COVID-19 pandemic**.

The analysis examines the sharp increase in unemployment during 2020 and compares unemployment levels before, during, and after the pandemic.

### Geographic Analysis

Unemployment rates are compared across the **53 geographic entities** included in the dataset.

This analysis identifies:

* Areas with consistently higher unemployment rates.
* Areas with lower unemployment rates.
* Differences in unemployment behavior between geographic entities.
* Geographic variation during major economic periods.

### Seasonal Analysis

Monthly unemployment rates are analyzed to identify recurring seasonal patterns.

The analysis examines:

* Average unemployment by month.
* Months with relatively higher unemployment.
* Months with relatively lower unemployment.
* Whether seasonal patterns remain consistent over time.

### Labor Force Analysis

The project also examines the relationship between labor-force participation-related measures and unemployment to provide additional context for changes in unemployment rates.

---

## Visualizations

The project includes visualizations generated during the analysis.

### Time-Series Analysis

```text
outputs/
└── figures/
    └── time_series/
        ├── annual_unemployment_trend.png
        └── monthly_unemployment_trend.png
```

### Seasonal Analysis

```text
outputs/
└── figures/
    └── seasonal_analysis/
        └── monthly_seasonality.png
```

---

## Key Findings

The analysis highlights several important patterns in U.S. unemployment:

* Unemployment varies considerably across different historical periods.
* The **COVID-19 pandemic produced an exceptional increase in unemployment in 2020**.
* Unemployment rates differ substantially between geographic entities.
* Unemployment exhibits recurring monthly and seasonal patterns.
* Major economic downturns can be identified through sharp increases in unemployment.
* Periods of economic recovery are reflected by subsequent decreases in unemployment.

Detailed findings and supporting visualizations are available in the analysis notebook.

---

## Project Structure

```text
EXPS_Unemployment_Analysis/
│
├── data/
│   ├── raw/
│   │   └── Unemployment in America Per US State.csv
│   │
│   └── processed/
│       └── unemployment_cleaned.csv
│
├── notebooks/
│   └── unemployment_analysis.ipynb
│
├── outputs/
│   └── figures/
│       ├── seasonal_analysis/
│       │   └── monthly_seasonality.png
│       │
│       └── time_series/
│           ├── annual_unemployment_trend.png
│           └── monthly_unemployment_trend.png
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## Technologies and Libraries

The project was developed using **Python** and the following tools and libraries:

* **Python** — programming language
* **Pandas** — data manipulation and analysis
* **NumPy** — numerical operations
* **Matplotlib** — data visualization
* **Seaborn** — statistical data visualization
* **Jupyter Notebook** — interactive analysis

---

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/MAROUA871/EXPS_Unemployment_Analysis.git
cd EXPS_Unemployment_Analysis
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the virtual environment

On Windows:

```bash
.venv\Scripts\activate
```

### 4. Install the required libraries

```bash
pip install -r requirements.txt
```

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```text
notebooks/unemployment_analysis.ipynb
```

---

## Internship

**Organization:** EXPERT PETROLEUM SERVICES

**Project:** Unemployment Analysis with Python

**Focus:** Data Cleaning, Data Validation, Exploratory Data Analysis, Data Visualization, Time-Series Analysis, Seasonal Analysis, and Economic Trend Analysis.
