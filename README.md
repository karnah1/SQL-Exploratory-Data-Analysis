# SQl Exploratory Data Analysis (EDA) 

This project is a hands on SQL case study focused on Exploratory Data Analysis.



## Executive Summary

This project demonstrates a comprehensive Exploratory Data Analysis (EDA) on a retail data warehouse using SQL. The goal is to move beyond simple queries to uncover actionable business insights by analyzing customer behavior, product performance, and sales trends.

**Business Problem** : The business needs to understand its core metrics, identify top-performing products/customers, and uncover geographical sales distributions to optimize marketing and inventory.

**Solution** : Developed a series of SQL scripts to profile data, calculate key performance indicators (KPIs), and perform magnitude and ranking analysis.

**Steps Involved** : Database Schema Exploration → Dimension Profiling → Date/Time Span Analysis → Measure Aggregation → Magnitude Analysis → Ranking & Filtering.

**Numbers Impact** : Identified a total revenue of ~$30M across ~60k items sold, with the "Bikes" category driving the vast majority of income.

## Business Problem

The stakeholders require a deep dive into the "Data Warehouse Analytics" database to answer:

What is the actual time span of our historical data?

Who are our most valuable customers (top spenders)?

Which product categories are underperforming or have data quality issues (nulls)?

How is the customer base distributed globally?

## Methodology

The project follows a structured 6-step framework:

**Database Exploration** : Mapping tables, schemas, and columns using INFORMATION_SCHEMA.

**Dimension Exploration**: Identifying unique values in categorical data (Country, Category, Gender).

**Date Exploration**: Determining the data boundaries (First/Last order) and calculating customer age demographics.

**Measure Exploration** : Calculating high-level KPIs (Total Sales, Quantity, Average Price, Count of unique orders).

**Magnitude Analysis** : Comparing measures across dimensions (e.g., Total Revenue by Category).

**Ranking Analysis** : Using TOP and Window Functions (ROW_NUMBER) to find best and worst performers.

## Skills

**SQL Fundamentals**: SELECT, FROM, WHERE, GROUP BY, ORDER BY, DISTINCT.

**Joins**: LEFT JOIN to combine Fact and Dimension tables without data loss.

**Aggregations** : SUM(), AVG(), COUNT(), MIN(), MAX().

**Advanced SQL** : Window Functions (ROW_NUMBER() OVER()), Subqueries (CTEs), UNION ALL.

**Metadata Querying** : INFORMATION_SCHEMA.TABLES, INFORMATION_SCHEMA.COLUMNS.

**Date Functions** : DATEDIFF(), GETDATE().

## Results and Recommendations

**Top Category** : Bikes generate the highest revenue (~$28M), significantly outpacing Accessories and Clothing.

**Customer Insights** : The customer base is evenly split by gender, but concentrated in the US and Australia.

**Data Quality** : Found 7 products missing category assignments; recommended a data cleansing step for the product catalog.

**Product Performance** : Identified the top 5 revenue-generating products (all Mountain/Road bikes) and recommended focusing marketing efforts on these high-ticket items.

## Next Steps

**Advanced Analytics** : Implement "Moving Averages" and "Year-over-Year (YoY) Growth" analysis.

**Data Visualization** : Connect this SQL database to Power BI or Tableau to create an interactive dashboard for stakeholders.

**Customer Segmentation** : Perform RFM (Recency, Frequency, Monetary) analysis to group customers into tiers.

