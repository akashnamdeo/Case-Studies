# Walmart Case Study

## Description

Walmart, a leading multinational retail corporation based in the United States, operates a wide range of retail formats including supercenters, discount department stores, and grocery stores. Serving over 100 million customers globally, Walmart is focused on optimizing its customer insights to drive business decisions. This case study explores customer purchase behavior to understand how spending patterns differ between male and female customers, especially during high-traffic periods such as Black Friday.

## Business Problem

The management team at Walmart Inc. is keen to analyze customer spending behavior to make informed strategic decisions. Specifically, they want to understand if there are significant differences in purchase amounts between male and female customers. This analysis aims to determine if women spend more than men during key shopping events like Black Friday. The dataset under analysis includes 50 million male customers and 50 million female customers.

### Dataset Overview
Dataset:
![alt text](image.png)

The dataset comprises various attributes and contains the following details:

- **Total Records:** 5,891
  - **Male Customers:** 414,259 rows (4,225 unique users)
  - **Female Customers:** 135,809 rows (1,666 unique users)
- **Product IDs:** 3,631 unique products
- **Age Groups:** Divided into 7 categories (0 to 55+)
- **Occupations:** 21 unique values
- **City Categories:** 3 values (A, B, C)
- **Stay in Current City Years:** 5 values (0 to 4 years)
- **Marital Status:** 2 values (0 for married, 1 for unmarried)
- **Product Categories:** 20 unique values
- **Purchase Amount:** Continuous variable representing the amount spent

## Variable Distributions and Relationships

### Purchase Statistics

- **Count:** 5,891 records
- **Mean Purchase Amount:** $865,016.60
- **Standard Deviation:** $943,644.50
- **Minimum Purchase Amount:** $46,681.00
- **25th Percentile:** $237,678.00
- **Median Purchase Amount:** $521,213.00
- **75th Percentile:** $1,119,250.00
- **Maximum Purchase Amount:** $10,536,910.00

### Observations

- **Distribution Pattern:** The purchase data follows a log-normal distribution, indicating a few high-value purchases skewing the mean to the right of the median.
- **High-Value Purchases:** The dataset includes substantial high-value purchases, which affect the mean significantly compared to the median.

### Key Insights

- **Gender Distribution:** The dataset shows a clear gender imbalance, with male customers significantly outnumbering female customers. Spending patterns are similar across genders, with most purchases occurring below $1,000,000.
- **Age Group Analysis:** The age group 26-35 is identified as having the highest spending. This age group contributes significantly to overall purchase amounts.
- **Marital Status Correlation:** There is a notable correlation between marital status and age, affecting purchase behavior.
- **Product Categories:** There is a strong negative correlation between product categories and purchase amounts, indicating that certain product categories are associated with lower purchase values.
- **Outliers:** Extreme purchase values exist, but they should be considered significant transactions rather than simple outliers.

## Recommendations

1. **Target High-Spending Customers:**
   - Focus on customers in the 26-35 age group as they represent a substantial portion of high-value purchases. Gender and marital status do not significantly alter their high spending behavior.

2. **Gender-Specific Spending Insights:**
   - Men generally spend more than women. With 90% confidence:
     - Men’s spending ranges between $921,110 and $1,098,157.
     - Women’s spending ranges between $607,705 and $875,972.
   - There is no overlap in these confidence intervals, indicating a clear distinction in spending patterns between genders.

3. **Product Preferences:**
   - Product Category 1 is highly popular across both genders. It accounts for 36% of purchases among high-priority customers.
   - Notable product IDs and categories include Product ID P00000142, and categories 1, 5, and 8.

4. **Estimations for a Larger Population:**
   - **For 100 Million Customers:**
     - Estimated total spending by male customers could be approximately $94.6 billion.
     - Estimated total spending by female customers could be around $69.8 billion.
   - **By Age Group:**
     - 0-17: $588,179
     - 18-25: $801,402
     - 26-35: $946,072
     - 36-45: $893,535
     - 46-50: $799,268
     - 51-55: $801,402
     - 55+: $478,919

5. **Product Recommendations:**
   - Recommend high-demand products from the identified categories and product IDs to high-priority customers to maximize sales.

