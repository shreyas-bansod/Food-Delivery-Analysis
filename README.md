# Food Delivery Analysis

## Overview

An end-to-end data analytics project investigating food delivery performance and identifying factors associated with longer delivery times and late deliveries. The project combines Python, SQL, statistical analysis, and Power BI to turn raw delivery data into actionable business insights.

**Business Question:** What factors are associated with delivery delays, and how can delivery performance be improved?

## Dataset

* **Dataset:** Food Delivery Dataset by Gaurav Malik
* **Source:** [Kaggle](https://www.kaggle.com/)
* **Records:** 45,593 deliveries
* **Date Range:** February 11, 2022 – April 6, 2022
* **Primary Metric:** Delivery time in minutes

The dataset contains order dates, delivery partner information, weather conditions, road traffic density, vehicle types, geographic coordinates, and delivery duration.

## Tools & Technologies

* **Python:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **SQL:** SQLite
* **Development:** Jupyter Notebook, VS Code
* **Dashboard:** Power BI, DAX
* **Version Control:** Git, GitHub

## Project Workflow

1. **Data Understanding and Cleaning:** Examined data types, missing values, invalid entries, duplicates, and data quality.
2. **Exploratory Data Analysis:** Investigated delivery performance across traffic, weather, distance, vehicle type, city, and multiple deliveries.
3. **SQL Analysis:** Used SQLite queries to calculate summary metrics and investigate operational patterns.
4. **Statistical Analysis:** Applied statistical methods to examine relationships between delivery characteristics and delivery time.
5. **Advanced Analysis:** Investigated combined risk factors and identified high-risk delivery segments.
6. **Business Recommendations:** Translated analytical findings into practical operational recommendations.
7. **Power BI Dashboard:** Built an interactive dashboard for exploring delivery KPIs and performance patterns.

## Key Findings

* **Average delivery time:** 26.29 minutes across 45,593 deliveries.
* **Late deliveries:** 29.84% of deliveries took more than 30 minutes.
* **Traffic impact:** Deliveries during traffic jams averaged 31.18 minutes, compared with 21.27 minutes under low traffic.
* **Weather impact:** Cloudy and foggy conditions had the highest average delivery times, at approximately 28.92 minutes.
* **Combined risk factors:** Orders during fog and traffic jams averaged 36.81 minutes, with 76.08% classified as late.
* **Multiple deliveries:** Orders involving two or three simultaneous deliveries averaged 40.45 and 47.82 minutes, respectively.
* **High-risk segment:** The identified high-risk group contained 843 orders, averaged 42.56 minutes, and had a 100% late-delivery rate.

## Power BI Dashboard

The interactive dashboard includes KPI cards, delivery status distribution, traffic and weather analysis, vehicle comparisons, distance bands, multiple-delivery analysis, city-level distribution, and high-risk delivery indicators.

Interactive slicers allow users to explore performance by order date, city, traffic density, weather conditions, and vehicle type.

![Food Delivery Operations Analytics Dashboard](dashboard/dashboard_screenshot.png)

## Repository Structure

```text
Food-Delivery-Analysis/
├── data/
│   ├── raw/
│   │   └── train.csv
│   ├── cleaned/
│   │   └── food_delivery_cleaned.csv
│   └── food_delivery.db
├── notebook/
│   ├── 01_data_understanding_cleaning.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_sql_analysis.ipynb
│   ├── 04_statistical_analysis.ipynb
│   ├── 05_advanced_analysis.ipynb
│   └── 06_business_recommendations.ipynb
├── dashboard/
│   ├── dashboard_screenshot.png
│   └── food delivery dashboard.pbix
├── sql/
├── docs/
├── .gitignore
├── requirements.txt
└── README.md
```

## How to Run

### Prerequisites

* Python 3
* Jupyter Notebook or VS Code with the Jupyter extension
* Power BI Desktop to open the dashboard

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/shreyas-bansod/Food-Delivery-Analysis.git
   ```

2. Move into the project folder:

   ```bash
   cd Food-Delivery-Analysis
   ```

3. Install the Python dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Open the `notebook/` directory and run the notebooks in numerical order, starting with `01_data_understanding_cleaning.ipynb`.

5. To explore the dashboard, open `dashboard/food delivery dashboard.pbix` in Power BI Desktop.

Keep the folder structure unchanged so relative file paths in the notebooks continue to work.

## Limitations

* The dataset covers a limited period and may not represent delivery patterns across all seasons or current operating conditions.
* The analysis identifies associations and patterns, not necessarily causal relationships.
* Extreme or inaccurate geographic coordinates can affect distance calculations.
* Findings for categories with small sample sizes should be interpreted cautiously.

## Author

**Shreyas Bansod**

* **GitHub Profile:** [shreyas-bansod](https://github.com/shreyas-bansod)
* **Project Repository:** [Food Delivery Analysis](https://github.com/shreyas-bansod/Food-Delivery-Analysis)

---

*This project demonstrates practical data analytics skills in data cleaning, exploratory analysis, SQL, statistical analysis, business recommendations, and Power BI dashboard development.*
