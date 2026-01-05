# Project name: Complete Data Analysis Project 

# Overview

This project provides a complete data analysis pipeline for sales data stored in a CSV file. The pipeline includes:

Loading and validating data

Cleaning and preprocessing

Analyzing sales trends by product, region, and time

Visualizing insights through charts

Generating meaningful business insights

The analysis is automated, professional, and robust with error handling and data validation.

## Features

### Data Loading

Reads a CSV file with columns:
Date, Product, Quantity, Price, Customer_ID, Region, Total_Sales

Checks for file existence and proper formatting

### Data Cleaning

Handles missing and invalid values

Corrects data types (e.g., Date, numeric columns)

Removes duplicates

Optionally computes missing Total_Sales as Quantity * Price

### Data Analysis

Aggregates total sales per product

Aggregates total sales per region

Computes monthly sales trends

Generates summary statistics for key metrics

## Visualizations

Bar chart: Total sales per product

Line chart: Monthly sales trend

Pie chart: Regional sales distribution

Charts are saved to disk in high-resolution (PNG)

## Insights

Identifies top-selling and lowest-selling products

Highlights the best-performing region

Tracks peak and lowest sales months

Error Handling & Validation

Handles missing files, invalid formats, and missing critical values

Provides informative messages for easy debugging

# Installation

Clone the repository or download the project files.

Ensure Python 3.8+ is installed.

Install required libraries:

`pip install pandas matplotlib seaborn`


Run the script:

You can use jupyter extension on vs code to run the `sales_analysis.ipynb` file


The script will:

`Clean and analyze the data

Generate charts in the visualisation/ folder

Print meaningful insights in the console

Output

Charts saved in visualisation/ folder:

top_products_sales.png

monthly_sales_trend.png

regional_sales_distribution.png`

Insights printed in console:

`1. The top-selling product is 'Product A' with total sales of 15,000.
2. The lowest-selling product is 'Product X' with total sales of 500.
3. The region with the highest sales is 'North' contributing 20,000 in sales.
4. The month with the highest sales is 2026-03 (5,000), and the lowest is 2026-01 (1,200).`

# Customization

You can change the output folder for charts by passing a different path to the visualize_data() function:

visualize_data(sales_per_product, sales_per_region, monthly_sales, output_dir="my_charts")


You can add more visualizations or analysis as needed.



# License

This project is open-source and free to use for educational and professional purposes.