Sales Data Cleaning and Analysis
This Jupyter Notebook (task1.ipynb) performs data cleaning and analysis on a sales dataset. Below is a summary of the steps taken:

Steps Performed
Data Loading:

The dataset is loaded from an Excel file (sales_data.xlsx) into a pandas DataFrame.

Initial Inspection:

The isnull() method is used to check for missing values, revealing that columns Unnamed: 8 to Unnamed: 12 contain only null values.

Data Cleaning:

The null columns (Unnamed: 8 to Unnamed: 12) are dropped from the DataFrame.

The Order Quantity column is converted to integer type.

The Order Date column is converted to datetime format.

Column names are standardized to lowercase with underscores for better readability (e.g., Order Number becomes order_number).

Feature Engineering:

Two new columns are added:

avg_sales_per_day: The average sales quantity per day for each SKU and warehouse combination.

max_sales_per_day: The maximum sales quantity per day for each SKU and warehouse combination.

Data Export:

The cleaned and processed DataFrame is saved to a new Excel file (clean_sales.xlsx).

A download link for the cleaned file is generated for easy access.

Key Observations
The dataset contains 33,919 rows and 8 columns after cleaning.

There are 290 unique SKU IDs in the dataset.

The data spans from January 1, 2021, to July 30, 2023.

Output
The final cleaned dataset includes the following columns:

order_number, order_date, sku_id, warehouse_id, customer_type,

order_quantity, unit_sale_price, revenue, avg_sales_per_day, max_sales_per_day
