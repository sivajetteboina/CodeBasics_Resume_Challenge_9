# CodeBasics_Resume_Challenge_9
# AtliQ Mart Sales Promotions Analysis
This repository contains the SQL scripts used to analyze the performance of promotional campaigns run by AtliQ Mart during Diwali 2023 and Sankranti 2024. The project addresses various business requests related to identifying high-value discounted products, store distribution, campaign effectiveness, and product performance in terms of incremental sales and revenue.

# Introduction

Promotional campaigns play a crucial role in the retail industry, driving sales and attracting customers during festive seasons. This project aims to analyze the performance of promotional campaigns conducted by AtliQ Mart during Diwali 2023 and Sankranti 2024. By leveraging data analytics, we seek to gain insights into the effectiveness of these campaigns and provide recommendations for optimizing future marketing strategies.

# Data Sources

The analysis is based on data obtained from AtliQ Mart's internal databases. The main datasets used include fact_events, dim_products, dim_stores, and sales_summary. These datasets contain information about product sales, store locations, promotional events, and campaign revenues.

# Project OverView

1. Analyzed data from AtliQ Mart's internal databases.
2. Performed SQL queries to fulfill five business requests.
3. Insights are intended to inform future promotional strategies and resource allocation.

# Business Requests

# High-Value Products in 'BOGOF' Promotion
Objective: Identify high-value products featured in the 'BOGOF' (Buy One Get One Free) promotion.

  SELECT 
     DISTINCT(product_name),
     base_price
     FROM 
     fact_events
     JOIN
     dim_products USING (product_code)
