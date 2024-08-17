# Aerofit Case-Study

## Description
The market research team at AeroFit is focusing on enhancing their product recommendation system for treadmills. They aim to understand the distinct characteristics of their target audience for each type of treadmill offered. By identifying these characteristics, AeroFit intends to tailor their recommendations to new customers more effectively, ensuring that they match the right treadmill with the right customer profile. This analysis investigates whether there are significant differences in customer attributes across the different treadmill models and aims to provide insights that can guide more personalized marketing and sales strategies.

## Business Problem
The market research team at AeroFit seeks to refine their product recommendation strategy by identifying and understanding the characteristics of the target audience for each type of treadmill. The objective is to analyze whether distinct customer profiles exist for different treadmill models and how these profiles can be leveraged to improve the accuracy of product recommendations. By differentiating customer characteristics associated with each treadmill type, AeroFit aims to enhance customer satisfaction and optimize their marketing efforts to align with customer preferences and needs.

This analysis will explore the variations in customer attributes, such as demographics and purchasing behavior, across various treadmill models to develop targeted recommendations for new customers and support strategic business decisions.

# Business Insights

## Attribute Ranges
- **Product**: Three unique treadmill models: `KP281`, `KP481`, and `KP781`.
- **Age**: Ranges from 18 to 50 years.
- **Gender**: Two unique values: `Male` and `Female`.
- **Education**: Ranges from 14 to 21 years.
- **Marital Status**: Two unique values: `Single` and `Partnered`.
- **Usage**: Six unique values: `3`, `2`, `4`, `5`, `6`, `7`.
- **Usage Fitness**: Five unique values: `4`, `3`, `2`, `1`, `5`.
- **Income**: Ranges from 29,562 to 104,581.
- **Miles**: Ranges from 21 to 360 miles.

## Variable Distributions and Relationships
- **Age and Income**: Positive correlation; as age increases, income tends to increase.
- **Product Usage**: Right-skewed; most customers use the treadmill less frequently.
- **Education**: Spread across all age groups; neither normally distributed nor skewed.
- **Usage**: Right-skewed; lower usage frequencies are more common.
- **Fitness**: Normally distributed for `KP281` and `KP481`.
- **Income**: Normally distributed for `KP281` and `KP481`.
- **Miles**: Normally distributed for `KP781`.

# Recommendations
- **Age-Based Recommendation**: Customers over 40 years old prefer the `KP281` model. Recommend `KP281` to customers aged 40 and above.
- **Education-Based Recommendation**: Customers with 12 to 18 years of education are the most frequent buyers. Recommend products based on this education range and consider `KP281` for customers with very low or very high education levels.
- **Usage-Based Recommendation**: Customers who use the treadmill 3 days a week mostly prefer `KP281`. Recommend `KP281` to customers with a target usage of 3 days per week.
- **Fitness-Based Recommendation**: Customers with an average fitness score of 3 prefer `KP281`. Recommend `KP281` to customers with an average fitness score.
- **Income-Based Recommendation**: High-income customers prefer `KP781`, while those with mid-range income prefer both `KP281` and `KP481`. Recommend products based on income brackets:
  - High income: `KP781`
  - Mid-range income: `KP281` and `KP481`
- **Mileage-Based Recommendation**: Customers with high mileage targets prefer `KP781`. Recommend `KP781` to customers with high mileage goals.
- **Overall Preference**: `KP281` is the most preferred model overall. Recommend `KP281` to customers with no specific information available.
- **Gender and Marital Status**: Male customers who are partnered have a higher probability of purchasing products. Consider this when recommending products to male, partnered customers.

