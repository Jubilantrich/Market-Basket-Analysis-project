# Market Basket Analysis Using Instacart Online Grocery Dataset

### Big Data Processing with PySpark

This project performs large scale market basket analysis using the
Instacart Online Grocery Shopping dataset. The dataset contains millions
of customer transactions collected from Instacart's e commerce platform,
covering details such as order history, products, departments, aisles,
and purchase patterns.

Using PySpark, the project demonstrates end to end data engineering and
analytical workflows on datasets that would be inefficient to process in
conventional environments.

## Project Objectives

1.  Explore and prepare large transactional datasets using PySpark.
2.  Identify the busiest ordering day of the week.
3.  Calculate the hour with the highest order volume.
4.  Determine the most popular products based on prior orders.
5.  Recognize the department with the maximum number of products.
6.  Apply Spark SQL and DataFrame APIs for large scale analytics.
7.  Demonstrate scalable data processing suitable for real world e
    commerce data.

## Dataset Description

The Instacart dataset consists of: - orders.csv - products.csv -
aisles.csv - departments.csv - order_products_prior.csv -
order_products_train.csv

These files include detailed information about user ordering patterns
and product relationships.

## Technologies Used

-   Apache Spark (PySpark)
-   Python 3
-   Spark SQL
-   Jupyter Notebook or VS Code

## Key Tasks Performed

### Task 1: Load and Explore the Orders Dataset

Loaded orders.csv and displayed the first 10 rows.

### Task 2: Handle Missing Values

Replaced null values in days_since_prior_order with 999.

### Task 3: Identify the Busiest Day

Used order_dow to compute total orders for each day.

### Task 4: Find the Busiest Hour

Aggregated orders by order_hour_of_day.

### Task 5: Determine the Most Popular Products

Joined order_products_prior and products to get the top 10 most
purchased items.

### Task 6: Explore Departments Dataset

Loaded departments.csv and displayed the data.

### Task 7: Department with the Maximum Products

Identified the department with the highest number of product listings.

## Sample Insights

-   Sunday is typically the busiest day.
-   Peak ordering occurs between 10 AM and 4 PM.
-   Produce department contains the most products.
-   Bananas and organic items dominate the top product list.

## How to Run Locally

1.  Install PySpark:

        pip install pyspark

2.  Load the dataset into a working directory.

3.  Start a PySpark session:

        from pyspark.sql import SparkSession
        spark = SparkSession.builder.appName("InstacartAnalysis").getOrCreate()

4.  Load CSV files and run the analysis.

## Project Structure

    ├── data/
    ├── notebooks/
    ├── scripts/
    └── README.md

## Skills Demonstrated

-   Spark SQL and PySpark transformations
-   Big data analytics
-   Data cleaning and joins
-   Aggregations on large scale datasets
-   SQL and Python integration

## Conclusion

This project highlights the use of PySpark for processing and analyzing
large e commerce datasets. It extracts valuable insights that support
inventory management, promotions planning, and customer behavior
understanding.
