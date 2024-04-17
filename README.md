# Maven-Roasters-Analysis-SQL-Project

## Introduction
Maven Roasters is a coffee shop with three locations in New York City namely Lower Manhattan, Hell's Kitchen and Astoria. Maven Roasters aims to understand and optimize the performance of the coffee shop by analyzing various aspects of sales data, such as daily and monthly sales trends, popular products, peak hours, customer demographics, and behaviour.
I will be playing the role of a business analyst for Maven Roasters, a bespoke, small batch coffee roasting company.

## About Dataset
The dataset used is fictional and sourced from Maven Analytics. It contains order details of all transactions recorded from January to June 2023 and it also contains 11 columns and 149116 rows.

## Data Wrangling / Approach
The initial step involves performing data cleaning on the dataset. Surprisingly there are no duplicated transaction records in the dataset.

1. Creating a database.
   ```
   CREATE DATABASE IF NOT EXISTS maven_roasters;
   ```
3. Creating a table.

