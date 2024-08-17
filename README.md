# Yulu Case Study

## Description

Yulu is India’s leading micro-mobility service provider, offering shared electric cycles for daily commutes. Yulu aims to reduce traffic congestion and provide a safe, sustainable, and user-friendly commuting solution through its mobile app. Yulu operates at strategic locations including metro stations, bus stands, office spaces, residential areas, and corporate offices to ensure smooth, affordable, and convenient commuting for its users.

Recently, Yulu has experienced a decline in revenues. To address this issue, they have engaged a consulting firm to analyze the factors affecting the demand for their shared electric cycles in the Indian market.

## Business Problem

Yulu seeks to understand the factors influencing the demand for shared electric cycles. Specifically, they want to identify which variables significantly predict demand and how well these variables describe cycle rental trends. The dataset provided includes information on various factors affecting cycle rentals.

### Dataset Overview
Dataset:
![alt text](image.png)

- **Total Records:** 10,886
- **Columns:** 12
  - **Datetime:** Contains hourly data, 10,886 unique values.
  - **Season:** 4 unique values (1, 2, 3, 4) with equal distribution.
  - **Holiday:** 2 unique values (0 for non-holiday, 1 for holiday).
  - **Working Day:** 2 unique values (0 for non-working day, 1 for working day).
  - **Weather:** 4 unique values (1, 2, 3, 4), with only 1 data point for weather = 4.
  - **Temp, atemp, humidity, windspeed, casual, registered, count:** Numerical variables.
- **Count Column Statistics:**
  - **Count:** 10,886
  - **Mean:** 191.57
  - **Standard Deviation:** 181.14
  - **Minimum:** 1
  - **25th Percentile:** 42
  - **Median:** 145
  - **75th Percentile:** 284
  - **Maximum:** 977
- **Data Quality:** No null values present.

## Business Insights

### Variable Distributions and Relationships

- **Count Distribution:** The distribution of bike rentals is right-skewed.
- **Season Distribution:** Rental data is equally distributed among all four seasons.
- **Holiday Impact:** Only 3% of bike rentals occur on holidays.
- **Working Day Impact:** 69% of bike rentals occur on working days.
- **Weather Impact:**
  - **High Demand:** Clear, Few clouds, Partly cloudy conditions account for 71% of rentals.
  - **Low Demand:** Rentals are extremely low during Snow, Rain, and Thunderstorm conditions.
- **Outlier Detection:** 
  - **Threshold for Outliers:** 647 (calculated using Q3 + 1.5 * (Q3 - Q1))
  - **Occurrences:** Over 300 instances exceed the threshold.
  - **Contribution:** 40% of these high rental counts are from conditions including Light Snow, Light Rain + Thunderstorm, and Scattered Clouds.

### Insights from Statistical Tests

- **Weather Effect:** Demand varies significantly across different weather conditions.
  - **Least Demand:** Heavy Rain + Ice Pellets + Thunderstorm + Mist, Snow + Fog.
  - **Most Demand:** Clear, Few clouds, Partly cloudy conditions.
- **Seasonal Variation:** Rental numbers are not similar across all seasons.

## Recommendations

1. **Stocking Strategy:**
   - **High Demand Weather:** Increase the stock of cycles during Clear, Few clouds, Partly cloudy weather conditions to meet higher demand.
   - **High Demand Locations:** Focus on stocking cycles near corporate offices during workdays.
   - **Low Demand Weather:** Consider alternative strategies for periods with Heavy Rain + Ice Pellets, Thunderstorm, Mist, Snow + Fog, where demand is virtually zero.

2. **Weather-Specific Insights:**
   - **High Demand:** Ensure availability during Clear, Few clouds, and Partly cloudy conditions.
   - **Low Demand:** Avoid excessive stock during weather conditions with Heavy Rain, Ice Pellets, and Snow + Fog, as these conditions result in minimal demand.

3. **Seasonal Insights:**
   - **Adjust Inventory:** Since the demand varies by season, adjust cycle stock based on seasonal patterns to optimize availability and reduce excess inventory.