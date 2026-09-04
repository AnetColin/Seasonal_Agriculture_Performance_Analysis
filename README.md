# 🌾 Seasonal Agriculture Performance Analysis

## 📌 Project Overview

The **Seasonal Agriculture Performance Analysis** project is a data analytics study designed to understand how agricultural performance varies across different **seasons, crops, geographical regions, and irrigation methods**.

The project analyzes agricultural, environmental, resource, and economic factors such as **crop yield, production, rainfall, temperature, soil moisture, water usage, irrigation method, revenue, cost, and profit**.

Using Python-based data analytics techniques, the project identifies important patterns, relationships, performance differences, and high- and low-performing agricultural combinations.

---

## 🎯 Project Goal

The primary goal of this project is to analyze agricultural performance across different seasons, crops, regions, and irrigation methods and identify patterns that can support **evidence-based agricultural planning and decision-making**.

The analysis focuses on:

- Seasonal agricultural performance
- Crop-wise yield and profitability
- Regional/state-level performance
- Irrigation method effectiveness
- Water usage and water efficiency
- Environmental factors and agricultural outcomes
- Economic performance
- Statistical differences between groups
- High- and low-performing Crop–Season–Irrigation combinations

---

## 📊 Dataset

The project uses the **Seasonal Agriculture Performance Dataset** containing:

- **4,000 agricultural records**
- **28 original attributes**
- An additional calculated `Profit_Margin_pct` feature created during analysis

The dataset contains information related to:

### 🌱 Agricultural Factors
- Crop
- Farm Area
- Yield
- Production
- Seed Quality

### 🌦️ Environmental Factors
- Rainfall
- Average Temperature
- Humidity
- Sunlight Hours
- Soil pH
- Soil Moisture

### 💧 Resource & Farming Factors
- Nitrogen
- Phosphorus
- Potassium
- Fertilizer Usage
- Pesticide Usage
- Irrigation Method
- Water Usage
- Water Efficiency

### 💰 Economic Factors
- Market Price
- Total Cost
- Revenue
- Profit
- Profit Margin

### 🗺️ Geographical Factors
- State
- District
- Season

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| **Python** | Data analysis and processing |
| **Jupyter Notebook** | Development and analysis environment |
| **Pandas** | Data manipulation and aggregation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |
| **SciPy** | Statistical testing |
| **Statsmodels** | Tukey HSD post-hoc analysis |

---

## 🔄 Project Workflow

```text
Data Collection
      ↓
Data Inspection
      ↓
Data Cleaning & Preprocessing
      ↓
Exploratory Data Analysis
      ↓
Seasonal Analysis
      ↓
Crop Analysis
      ↓
Regional Analysis
      ↓
Irrigation Analysis
      ↓
Statistical Analysis
      ↓
Correlation Analysis
      ↓
Crop–Season–Irrigation Analysis
      ↓
Key Insights & Recommendations
      ↓
Final Conclusion


## 🔍 Analysis Performed

### 1. Data Cleaning

The dataset was inspected for:

* Missing values
* Duplicate records
* Incorrect data types
* Numerical and categorical variables

Missing numerical values were handled using **median imputation**, and duplicate records were checked and removed where necessary.

---

### 2. Exploratory Data Analysis

Exploratory analysis was performed to understand:

* Dataset distributions
* Crop frequencies
* Seasonal distribution
* Regional distribution
* Yield distribution
* Profit distribution
* Resource usage
* Environmental conditions

Various charts including **histograms, boxplots, and bar charts** were used.

---

### 3. Seasonal Analysis

The dataset contains three major seasons:

* 🌧️ **Kharif**
* ❄️ **Rabi**
* ☀️ **Zaid**

Kharif showed the strongest overall observed economic performance, while Zaid showed the weakest.

Average profit:

| Season | Average Profit |
| ------ | -------------: |
| Kharif |    ₹178,914.65 |
| Rabi   |     ₹87,689.47 |
| Zaid   |    -₹24,804.82 |

Kharif also recorded the highest average yield and water efficiency.

---

### 4. Crop Analysis

Eight crops were analyzed:

* Sugarcane
* Maize
* Rice
* Wheat
* Chilli
* Groundnut
* Cotton
* Pulses

**Sugarcane** recorded the highest average yield and average profit among the analyzed crops.

Average profit of selected top-performing crops:

| Crop      | Average Profit |
| --------- | -------------: |
| Sugarcane |    ₹817,187.99 |
| Chilli    |    ₹750,878.34 |
| Cotton    |    ₹124,546.92 |
| Groundnut |     ₹44,858.12 |

The analysis also demonstrated that **physical yield and profitability do not necessarily follow the same ranking**.

---

### 5. Regional Analysis

Agricultural performance was compared across eight states:

* Punjab
* Maharashtra
* Karnataka
* Tamil Nadu
* Gujarat
* Telangana
* Madhya Pradesh
* Andhra Pradesh

Punjab recorded the highest average yield and production, while Maharashtra recorded the highest average revenue.

---

### 6. Irrigation Analysis

Four irrigation methods were analyzed:

* 💧 Drip
* 💦 Flood
* 🌧️ Rainfed
* 🚿 Sprinkler

Drip irrigation recorded the highest average yield and profitability.

| Irrigation Method | Avg. Yield | Avg. Profit | Avg. Water Efficiency |
| ----------------- | ---------: | ----------: | --------------------: |
| Drip              |       6.58 | ₹219,626.00 |                  6.27 |
| Sprinkler         |       5.16 |  ₹91,121.08 |                  4.67 |
| Rainfed           |       4.60 |  ₹79,050.37 |                  7.56 |
| Flood             |       4.86 |  ₹73,354.02 |                  3.44 |

Rainfed farming showed the highest average water efficiency, while Flood irrigation consumed the most water and had the lowest water efficiency.

---

## 📐 Statistical Analysis

### Seasonal Yield ANOVA

* **F-statistic:** 1.5439
* **p-value:** 0.2137

The difference in mean yield between seasons was **not statistically significant** at the 5% significance level.

### Seasonal Profit ANOVA

* **F-statistic:** 34.2918
* **p-value:** < 0.001

The difference in average profit between seasons was **statistically significant**.

Tukey HSD indicated significant differences between:

* Kharif vs Rabi
* Kharif vs Zaid
* Rabi vs Zaid

---

### Irrigation Yield ANOVA

* **F-statistic:** 4.2455
* **p-value:** 0.0053

The irrigation groups showed a statistically significant difference in average yield.

Tukey HSD indicated that Drip differed significantly from Flood and Rainfed.

---

### Irrigation Profit ANOVA

* **F-statistic:** 15.8873
* **p-value:** < 0.001

Irrigation methods showed statistically significant differences in average profitability.

Drip irrigation had significantly higher average profit compared with the other irrigation groups.

---

## 🔗 Correlation Analysis

Correlation analysis was performed to identify relationships between numerical variables.

Some of the strongest observed correlations were:

| Variable Pair                 | Correlation |
| ----------------------------- | ----------: |
| Water Efficiency ↔ Yield      |    **0.91** |
| Revenue ↔ Profit              |    **0.89** |
| Yield ↔ Production            |    **0.88** |
| Water Efficiency ↔ Production |    **0.81** |
| Production ↔ Revenue          |    **0.56** |

Environmental variables such as rainfall, temperature, humidity, sunlight, and soil moisture showed **very weak linear correlations with yield** in this dataset.

> **Note:** The strong relationship between Water Efficiency and Yield should be interpreted carefully because water efficiency may be calculated from related yield/production and water-use variables.

---

## 🏆 Best Performing Combination

The best observed **Crop–Season–Irrigation** combination was:

### 🌱 Sugarcane + Kharif + Drip

* **Average Yield:** 62.86 tonnes/ha
* **Average Profit:** ₹1,361,630.18
* **Average Water Efficiency:** 39.75
* **Records:** 34

---

## ⚠️ Lowest Performing Combination

The weakest observed combination was:

### 🌾 Wheat + Zaid + Flood

* **Average Yield:** 1.50 tonnes/ha
* **Average Profit:** -₹271,158.52
* **Average Water Efficiency:** 2.27
* **Records:** 25

### Difference between best and worst combinations

* **Profit difference:** ₹1,632,788.70
* **Yield difference:** 61.36 tonnes/ha
* **Water efficiency difference:** 37.48

---

## 💡 Key Insights

1. **Kharif** showed the highest average profitability among the three seasons.
2. **Zaid** showed the weakest average economic performance.
3. **Sugarcane** recorded the highest average crop profitability.
4. **Drip irrigation** showed the strongest overall combination of yield and profitability.
5. **Rainfed** farming showed the highest average water efficiency.
6. **Flood irrigation** had the highest average water usage and lowest water efficiency.
7. Agricultural performance varied significantly across **states, crops, seasons, and irrigation methods**.
8. The best observed combination was **Sugarcane + Kharif + Drip**.
9. The weakest observed combination was **Wheat + Zaid + Flood**.
10. Environmental variables showed weak linear relationships with yield in the available dataset.

---

## 📌 Recommendations

Based on the observed patterns:

* Prioritize **Kharif** when conditions and planning allow.
* Consider economically strong crops such as **Sugarcane and Chilli**.
* Consider **Drip irrigation** where the objective is higher observed yield and profitability.
* Give particular attention to **water efficiency** when evaluating irrigation strategies.
* Evaluate Zaid cultivation carefully because several Crop–Season–Irrigation combinations showed negative profitability.
* Consider **yield, profitability, water efficiency, variability, and sample size together** rather than relying on a single metric.
* Use the findings as decision-support insights rather than direct causal recommendations.

---

## 🔮 Future Scope

The project can be extended by implementing:

* Machine Learning-based crop yield prediction
* Profit prediction models
* Weather forecasting integration
* Smart irrigation recommendations
* GIS-based geographical analysis
* Interactive Power BI or Streamlit dashboard
* Time-series agricultural forecasting
* AI-based agricultural decision support
* Anomaly and risk detection
* Advanced regression and interaction analysis
* Sustainable resource optimization

The project can ultimately evolve from a **descriptive analytics system into a predictive and intelligent agricultural decision-support system**.

---

## 👥 End Users

Potential end users include:

* 👨‍🌾 Farmers
* 🌾 Agricultural planners
* 🏛️ Government agricultural departments
* 💧 Irrigation and water resource managers
* 🔬 Agricultural researchers
* 💼 Agribusinesses
* 🎓 Students and data analysts
* 📊 Agricultural decision-makers

---

## 📂 Project Structure

```text
Seasonal-Agriculture-Performance-Analysis/
│
├── Seasonal_Agriculture_Performance_Analysis.ipynb
├── seasonal_agriculture_performance_dataset.csv
└── README.md
```

---

## 📊 Key Technologies

```text
Python
│
├── Pandas
├── NumPy
├── Matplotlib
├── Seaborn
├── SciPy
└── Statsmodels
```

---

## ⚠️ Important Note

The results presented in this project describe **patterns and associations observed in the available dataset**.

Statistical significance or correlation does not necessarily imply that one agricultural factor directly causes another. In particular, relationships involving irrigation, season, crop selection, and profitability may be affected by other factors such as crop composition, regional conditions, input costs, and dataset characteristics.

Some Crop–Season–Irrigation combinations also have relatively small sample sizes, so those results should be interpreted with caution.

---

## 👨‍💻 Author

**Anet Colin Rockey**

Data Analytics | Python | Machine Learning | Power BI

🔗 LinkedIn: [Anet Colin Rockey](https://www.linkedin.com/in/anetrockey)

🔗 GitHub: [AnetColin](https://github.com/AnetColin)

