# Climate-Change-Data-Analysis
Time-series analysis of global land and ocean temperatures using Python
# 🌍 Climate Change - Global Temperature Data Analysis

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-3776AB.svg)](https://seaborn.pydata.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

</div>

---

## 👨‍🎓 Project Information
* **Course:** Programming for Data Science and AI[span_0](start_span)[span_0](end_span)
* **Instructor:** Dr. Belal Alifan[span_1](start_span)[span_1](end_span)
* **Student Name:** Zain Irshedat[span_2](start_span)[span_2](end_span)
* **Project Type:** Climate Change Indicators Analysis[span_3](start_span)[span_3](end_span)

---

## 🎯 Project Objectives
* Analyze real-world climate datasets using Python[span_4](start_span)[span_4](end_span).
* Perform a time-series trend analysis of global land and ocean temperatures (1750–2015)[span_5](start_span)[span_5](end_span).
* Explore geographical patterns, regional variations, and city-level temperature extremes[span_6](start_span)[span_6](end_span).
* Generate rich data visualizations to support climate awareness[span_7](start_span)[span_7](end_span).
* Practice professional data cleaning, feature extraction, and exploratory data analysis (EDA) techniques[span_8](start_span)[span_8](end_span).

---

## 📁 Dataset Description
The analysis is based on the **Kaggle Climate Change Indicators Dataset**[span_9](start_span)[span_9](end_span). The following files were utilized:
* `GlobalTemperatures.csv`[span_10](start_span)[span_10](end_span)
* `GlobalLandTemperaturesByCity.csv`[span_11](start_span)[span_11](end_span)
* `GlobalLandTemperaturesByCountry.csv`[span_12](start_span)[span_12](end_span)
* `GlobalLandTemperaturesByMajorCity.csv`[span_13](start_span)[span_13](end_span)
* `GlobalLandTemperaturesByState.csv`[span_14](start_span)[span_14](end_span)

**Key Columns Analyzed:** `dt` (Date), `AverageTemperature`, `Country`, `City`, `LandMaxTemperature`, `LandMinTemperature`, `LandAndOceanAverageTemperature`.

---

## 🛠️ Tech Stack & Libraries Used
* **`pandas` & `numpy`:** Data cleaning, grouping, statistical calculations, and correlation matrices[span_15](start_span)[span_15](end_span).
* **`matplotlib` & `seaborn`:** Advanced plotting (Line charts, Bar charts, Boxplots, and Correlation Heatmaps)[span_16](start_span)[span_16](end_span).
* **`scipy.stats` (Linear Regression):** Calculating temperature trend slopes over time[span_17](start_span)[span_17](end_span).
* **`plotly`:** Interactive global choropleth heatmaps.

---

## 🧹 Data Cleaning & Preprocessing
* Converted raw date columns (`dt`) into standardized `datetime` objects[span_18](start_span)[span_18](end_span).
* Handled and dropped missing values (`dropna`) and checked for duplicate rows[span_19](start_span)[span_19](end_span).
* Extracted **Year** and **Month** features for temporal grouping.
* Filtered time-series data (focusing from 1900+ and specific historical ranges) and removed anomalies (e.g., Antarctica) for precise global mapping[span_20](start_span)[span_20](end_span).

---

## 📊 Key Findings & Insights
1. **Global Temperature Trends:** Time-series visualization demonstrates a clear, continuous upward trend in global average land temperatures, particularly accelerating from the 1900s to 2015[span_21](start_span)[span_21](end_span).
2. **Correlation Analysis:** Built robust correlation heatmaps across `LandAverage`, `LandMax`, `LandMin`, and `Ocean` variables, revealing extremely high positive correlations ($\ge 0.98$), proving that global warming drives concurrent rises in peak and baseline temperatures[span_22](start_span)[span_22](end_span).
3. **Warming Rates (Slope Analysis):** Applied linear regression per country to find the steepest warming rates (1960–2015), highlighting regions like Mongolia, Kazakhstan, Turkmenistan, and Uzbekistan[span_23](start_span)[span_23](end_span).
4. **Hottest Urban Zones:** Evaluated city-level data post-2000, revealing extreme urban heat concentration in regions across Africa, the Middle East, and the Gulf (e.g., Djibouti, Khartoum, and surrounding areas)[span_24](start_span)[span_24](end_span).
5. **Seasonal Variability:** Monthly distribution boxplots (1900–2000) show that summer months experience significantly wider temperature variances, whereas winter months remain stable[span_25](start_span)[span_25](end_span).

---

## 💡 Recommendations & Future Work
* **Predictive Modeling:** Monitor countries with the steepest warming slopes using advanced machine learning models[span_26](start_span)[span_26](end_span).
* **Policy Integration:** Utilize temperature trend metrics to inform national climate change strategies[span_27](start_span)[span_27](end_span).
* **Scope Expansion:** Integrate external indicators like $\text{CO}_2$ emissions, sea-level changes, and population density[span_28](start_span)[span_28](end_span).

---

## 🚀 Getting Started & Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/Climate-Change-Data-Analysis.git](https://github.com/your-username/Climate-Change-Data-Analysis.git)
