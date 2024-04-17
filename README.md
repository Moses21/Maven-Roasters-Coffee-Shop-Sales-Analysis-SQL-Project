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
   ```
   CREATE TABLE IF NOT EXISTS sales(
    transaction_id INT NOT NULL,
    transaction_date DATE NOT NULL,
    transaction_time TIME NOT NULL,
    store_id INT NOT NULL,
    store_location VARCHAR(20) NOT NULL,
    product_id INT NOT NULL,
    transaction_qty INT NOT NULL,
    unit_price FLOAT NOT NULL,
    product_category VARCHAR(20) NOT NULL,
    product_type VARCHAR(50) NOT NULL,
    product_detail VARCHAR(50) NOT NULL
   )
   ```
3. Data Importation from CSV
   After creating a database and table, now it’s time to import data from a CSV file. For this select and right-click on the table sales and a new window open then I select the path from 
   the local machine where I stored the dataset

