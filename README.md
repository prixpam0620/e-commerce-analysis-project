# e-commerce-analysis-project
Data analysis of e-commerce basket and customer data using Python
# E-commerce Analysis Project

## Overview
This project analyzes an e-commerce dataset consisting of `basket_data` (15,000 rows of purchase transactions) and `customer_data` (20,000 rows of customer demographics). The goal was to explore customer purchasing behavior and build a basic predictive model.

## Dataset
- **Source**: Local files (`basket.csv`, `customer.csv`).
- **Details**: 
  - `basket_data`: Contains `customer_id`, `product_id`, `basket_date`, and `basket_count`.
  - `customer_data`: Contains `customer_id`, `sex`, `customer_age`, and `tenure`.
- **Size**: 15,000 and 20,000 rows respectively, with only 72 rows matching due to sparse `customer_id`s.

## Analysis Performed
- Merged datasets using an inner join to identify 64 unique `customer_id`s with matching data.
- Calculated total `basket_count` by sex: 33 (Female) and 122 (Male), totaling 155.
- Analyzed `basket_count` by age group: 2 (0-18), 52 (19-30), 71 (31-50), 20 (51+), and 10 (outside 0-100), resolving a 155 vs. 145 discrepancy.
- Built customer-level features and attempted a Poisson regression model to predict `basket_count` (MSE = 26.19).

## Skills Demonstrated
- Data cleaning and merging with Pandas.
- Exploratory data analysis and visualization with Matplotlib.
- Basic modeling with scikit-learn.
- Problem-solving (e.g., debugging age group totals).

## Files
- `ecommerce_analysis.py` or `ecommerce_analysis.ipynb`: Contains the full code.
- `basket.csv`, `customer.csv`: Original datasets link (https://www.kaggle.com/datasets/berkayalan/ecommerce-sales-dataset/code).

## Future Work
- Refine the model with more data or features.
- Explore unmatched transactions for additional insights.

## Contact
Priyanka Pandey
yourspm91@gmail.com
linkedin: https://www.linkedin.com/in/prixpam0620 
