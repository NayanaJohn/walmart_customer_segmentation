# Walmart Retail Dataset Analysis for Customer Segmentation and Sales Prediction

## Overview

This project analyzes the Walmart retail dataset to uncover valuable insights into customer behavior, segmenting customers based on spending patterns, purchase frequency, and RFM (Recency, Frequency, and Monetary) metrics. The goal is to enable enhanced targeted marketing strategies, improve customer loyalty, and increase revenue for business growth.

## Objective

The main objectives of this project are:

- Segment customers based on purchase patterns.
- Predict sales using various machine learning models.
- Explore factors affecting customer behavior and sales performance.

## Dataset Description

The dataset contains the following columns:

- **city**: Location of the customer.
- **customer_age**: Age of customers.
- **customer_name**: Name of the customer.
- **customer_segment**: Classification of customers into segments.
- **discount**: Discount applied to products in the order.
- **order_date**: Date when the order was placed.
- **order_id**: Unique identifier for each order.
- **order_priority**: Priority level of the order.
- **order_quantity**: Quantity of items ordered.
- **product_base_margin**: Base profit margin for each product.
- **product_category**: Category of the product.
- **product_container**: Type of container for the product.
- **product_name**: Name of the purchased product.
- **product_sub_category**: Categorization within the main product category.
- **profit**: Total profit generated from the order.
- **region**: Geographic region where the sale occurred.
- **sales**: Total sales amount for each order.
- **ship_date**: Date when the order was shipped.
- **ship_mode**: Method of shipping used for the order.
- **shipping_cost**: Cost incurred for shipping the order.
- **state**: State in which the customer is located.
- **unit_price**: Price per unit of product.
- **zip_code**: Postal code for the customer's location.

## Approach

The approach taken in this project includes the following steps:

### 1. EDA (Exploratory Data Analysis)

- **Data cleaning and preprocessing**: Removing missing or duplicate values, handling irrelevant data, and addressing outliers.
- **Univariate and Bivariate Analysis**: Examining individual features and their relationships.
- **Feature Engineering**: Creating new features based on existing data (e.g., extracting year, month, weekday from `order_date`).
- **One-hot Encoding**: Encoding categorical variables like `region`, `product_category`, and `order_priority`.

### 2. Modeling

- **RandomForestRegressor**: Applied to predict sales based on various features .
- **DecisionTreeRegressor**: Used for predicting sales and exploring feature importance.

### 3. Customer Segmentation

- Segmenting customers based on spending patterns, purchase behaviors, and RFM metrics to better target them with marketing campaigns.
- **Pareto Analysis**: Identifying the top 20% of customers contributing to 80% of sales.
- **Anomaly Detection**: Identifying unusual sales patterns or outliers.

### 4. Evaluation

- **Model Evaluation**: Evaluating the performance of the models using metrics such as **MAE** (Mean Absolute Error), **RMSE** (Root Mean Squared Error), and **R-squared**.
- **Feature Importance**: Identifying the most influential features in sales prediction.

## Tools and Libraries

- **Programming Language**: Python
- **Libraries Used**:
  - `pandas`: For data manipulation and preprocessing.
  - `seaborn`: For data visualization.
  - `numpy`: For numerical operations.
  - `matplotlib`: For data visualization.
  - `scikit-learn`: For machine learning models, feature preprocessing, and evaluation.
