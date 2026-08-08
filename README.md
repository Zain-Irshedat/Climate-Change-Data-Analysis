# Climate-Change-Data-Analysis
Time-series analysis of global land and ocean temperatures using Python
# 🌍 Climate Change & Global Temperature Data Analysis

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-3776AB.svg)](https://seaborn.pydata.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

</div>

---

## 📌 Project Overview
This project presents a comprehensive time-series and exploratory data analysis (EDA) of global climate indicators. By leveraging Python data science libraries, the project investigates historical land and ocean temperature anomalies, cross-variable correlations, and regional warming trends spanning from 1750 to 2015.

---

## 📊 Datasets & Schema
The analysis utilizes multiple datasets from the Climate Change Indicators repository:
* `GlobalTemperatures.csv` (Global land and ocean temperature records)
* `GlobalLandTemperaturesByCity.csv` & `GlobalLandTemperaturesByMajorCity.csv` (Urban temperature metrics)
* `GlobalLandTemperaturesByCountry.csv` & `GlobalLandTemperaturesByState.csv` (Geographical tracking)

**Primary Features:** `dt` (Timestamp), `AverageTemperature`, `LandMaxTemperature`, `LandMinTemperature`, `LandAndOceanAverageTemperature`, alongside geographical metadata (`Country`, `City`).

---

## 🛠️ Tech Stack & Dependencies
* **Data Processing:** `pandas`, `numpy`
* **Statistical Modeling:** `scipy.stats` (Linear Regression & Trend slopes)
* **Data Visualization:** `matplotlib`, `seaborn`, `plotly`

---

## ⚙️ Data Preprocessing & Pipeline
1. **Type Casting:** Converted raw date strings (`dt`) into standardized `datetime64` structures for precise temporal slicing.
2. **Data Hygiene:** Handled missing values (`dropna`) and validated data uniqueness to prevent analytical skew.
3. **Feature Engineering:** Extracted isolated **Year** and **Month** parameters from timestamps to enable seasonal aggregation.
4. **Filtering & Normalization:** Filtered analytical slices for modern timelines (1900+) and removed geographical anomalies (such as Antarctica) to maintain mapping integrity.

---

## 📈 Key Analytical Findings & Visualizations

### 1. Global Temperature Time-Series Trend
* **Analysis:** Aggregated historical yearly data to trace the global average land temperature trajectory.
* **Insight:** Displays a sharp, continuous upward acceleration in global temperatures, particularly noticeable post-1900 through 2015.

### 2. Cross-Variable Correlation Matrix
* **Analysis:** Constructed Pearson correlation heatmaps mapping relationships between `LandAverage`, `LandMax`, `LandMin`, and `LandAndOcean` temperatures.
* **Insight:** Revealed an extremely strong positive correlation ($\ge 0.98$) across all thermal dimensions, confirming that baseline shifts drive uniform escalations in both peak and minimum boundaries.

### 3. Country-Level Warming Rates (Linear Regression Slope)
* **Analysis:** Applied linear regression per country over the 1960–2015 period to calculate the mathematical rate of change ($\text{°C}$ per year).
* **Insight:** Identified regions experiencing the steepest thermal shifts (e.g., Mongolia, Kazakhstan, Turkmenistan, and Uzbekistan).

### 4. Urban Heat Concentration (Hottest Cities)
* **Analysis:** Evaluated post-2000 city datasets to isolate extreme urban temperature averages.
* **Insight:** Highlighted severe thermal concentration heavily localized in equatorial belts, North/Central Africa, and parts of the Middle East and Gulf region.

### 5. Seasonal Variability & Distribution
* **Analysis:** Mapped monthly boxplot distributions spanning a 100-year window (1900–2000).
* **Insight:** Demonstrated that summer months exhibit significantly higher internal variance and volatility compared to structurally stable winter baselines.

---

## 💡 Strategic Recommendations & Future Work

Based on the insights derived from the data analysis, the following actions and improvements are recommended:
* **Predictive Modeling Implementation:** Deploy advanced machine learning and time-series forecasting models (such as ARIMA or Prophet) specifically targeting countries exhibiting the steepest warming slopes.
* **Targeted Mitigation Policies:** Prioritize climate adaptation and public awareness campaigns in high-risk urban zones and vulnerable equatorial/Gulf regions identified as extreme heat hotspots.
* **Data Integration Expansion:** Expand future iterations of the pipeline to ingest multi-variable indicators, such as atmospheric $\text{CO}_2$ concentration levels, oceanic pH, and population growth data to study direct environmental drivers.
* **Interactive Dashboarding:** Migrate static visual reports into continuous, web-based monitoring dashboards (using Streamlit or Dash) for real-time public reporting and policy decision support.

---

## 🚀 Getting Started & Execution

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/Climate-Change-Data-Analysis.git](https://github.com/your-username/Climate-Change-Data-Analysis.git)
   
