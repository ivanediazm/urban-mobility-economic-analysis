# Urban Mobility & Economic Analysis

## Project Overview

This project analyzes the relationship between **urban mobility and economic productivity** across major Latin American cities.

The main objective is to evaluate whether higher traffic congestion and travel delays are associated with higher or lower levels of economic productivity.

For this analysis:

* `jams_delay` is used as an indicator of traffic congestion and mobility delays.
* `city_gdp_capita` represents GDP per capita.
* `unemployment_pct` is included as an additional economic indicator.

The analysis focuses on identifying patterns, comparing cities, detecting potential outliers, and generating insights that could support infrastructure and urban mobility decisions.

---

## Business Question

**Is there a relationship between urban congestion, travel delays, and economic productivity measured through GDP per capita?**

Understanding this relationship can help identify cities where mobility problems may represent a greater economic challenge and where infrastructure investment could have a stronger potential impact.

---

## Data Coverage

The analysis focuses on **2024** and includes:

* **15 cities**
* **7 Latin American countries**

Countries included:

* Argentina
* Brazil
* Chile
* Colombia
* Mexico
* Peru
* Uruguay

This regional coverage allows for comparisons between cities with different economic and mobility conditions.

---

## Methodology

The project followed a structured data analysis process:

### 1. Data Cleaning

The datasets were reviewed and standardized to ensure consistency across variables.

Main transformations included:

* Standardizing column names
* Converting date fields into datetime format
* Cleaning percentage values
* Converting economic and traffic indicators into numeric formats
* Reviewing missing values
* Identifying duplicated records

### 2. Data Transformation

Traffic and economic datasets were aggregated at the **city-year level**.

A common year field was created to ensure both datasets could be compared consistently.

### 3. Dataset Integration

Traffic and economic datasets were combined using an **INNER JOIN**, keeping only cities available in both sources.

This ensured that all cities included in the final analysis contained both mobility and economic information.

### 4. Exploratory Data Analysis

Visualizations and descriptive statistics were used to:

* Analyze variable distributions
* Identify potential outliers
* Compare congestion levels across cities
* Compare GDP per capita across cities
* Explore the relationship between congestion and economic productivity
* Evaluate unemployment as an additional economic factor

---

## Key Findings

The analysis identified a **positive but weak relationship between traffic congestion and GDP per capita**.

This suggests that cities with higher economic productivity do not necessarily experience higher or lower levels of congestion.

Some important observations include:

### Mexico City

Mexico City shows the **highest traffic delay among the cities analyzed**, while also maintaining a relatively high GDP per capita.

This combination suggests that strong economic activity can coexist with significant mobility challenges.

### Montevideo

Montevideo presents the **highest GDP per capita in the dataset** while maintaining one of the lowest congestion levels.

This indicates that higher economic productivity does not necessarily imply greater traffic congestion.

### Santiago

Santiago appears as a potential **outlier**, combining relatively high congestion with a considerably lower GDP per capita compared with other cities in the analysis.

Before drawing conclusions from this result, the economic indicator should be validated to confirm that currency, units, and calculation methodology are consistent with the rest of the dataset.

---

## Investment Prioritization Insight

Among **Bogotá, Lima, and Buenos Aires**, Bogotá emerges as the strongest candidate for transportation infrastructure investment.

Bogotá combines:

* Higher traffic congestion
* Lower GDP per capita
* Higher unemployment

This combination suggests that mobility improvements could potentially contribute to better accessibility and economic conditions.

Santiago could represent an even higher priority, but its economic data should first be validated before making investment recommendations.

---

## Recommendations

To strengthen future analyses and improve infrastructure investment decisions, additional variables should be incorporated, including:

* Population
* Population density
* Vehicle ownership
* Public transportation coverage
* Average commuting time
* Urban area size
* Transportation infrastructure investment

Including multiple years of data would also make it possible to evaluate trends over time instead of relying on a single-year snapshot.

---

## Tools & Technologies

* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Skills Demonstrated

This project demonstrates practical experience in:

* Data cleaning
* Data transformation
* Data aggregation
* Dataset merging
* Exploratory Data Analysis
* Data visualization
* Outlier detection
* Business-oriented data interpretation
* Insight generation
* Data-driven recommendations

---

## Repository Structure

```text
urban-mobility-economic-analysis/
│
├── README.md
├── urban_mobility_analysis.ipynb
├── oecd_city_economy.csv
└── traffic_sample.csv
```

> The complete traffic dataset is not included in this repository due to file size limitations. A sample dataset can be included to demonstrate the structure of the original data.

---

## Conclusion

The analysis does not provide strong evidence that cities with higher GDP per capita systematically experience higher or lower traffic congestion.

Instead, urban mobility appears to depend on multiple factors beyond economic productivity alone.

The results highlight the importance of combining mobility indicators with socioeconomic variables when evaluating transportation infrastructure priorities.

Future analyses incorporating additional variables and multiple years of data could provide a more robust understanding of how urban mobility influences economic performance.
