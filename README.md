### Sales Data Analysis

This project involves the analysis of sales data from multiple CSV files located in the Sales directory. The goal is to perform various data cleaning and visualization tasks to gain insights into the sales performance.

## Libraries Used

- `numpy`
- `pandas`
- `matplotlib`
- `os`

## Steps Performed

### - Data Import and Concatenation

- **Import Libraries** : We start by importing necessary libraries such as pandas, numpy, matplotlib, and os.
- **Read Files** : All CSV files in the ./Sales directory are read and concatenated into a single DataFrame called all_data.
- **Save Combined Data** : The combined data is saved into a new CSV file named all_data.csv.

### - Data Cleaning

- **Remove Empty Rows** : Rows with all NaN values are removed.
- **Filter Valid Order Dates** : Rows with invalid Order Date formats are filtered out.
- **Convert Data Types** : The Order Date column is converted to datetime format, and Quantity Ordered and Price Each columns are converted to numeric types.
- **Calculate Sales** : A new column Sales is created by multiplying Quantity Ordered and Price Each.

### - Data Analysis

- **Monthly Sales** : The data is grouped by month to calculate the total quantity ordered, price each, and sales for each month.
- **City and State Sales** : The data is grouped by city and state to calculate the total sales for each location.
- **Hourly Orders** : The data is grouped by the hour of the day to analyze the number of orders placed each hour.
- **Product Sales** : The top 10 best-selling products are identified.
- **Product Combinations** : Products that are frequently bought together in the same order are identified.

### - Data Visualization

- **Monthly Sales Plot** : A bar plot is created to visualize the monthly sales.
- **City Sales Plot** : A bar plot is created to visualize the total sales by city.
- **State Sales Plot** : A bar plot is created to visualize the total sales by state.
- **Hourly Orders Plot** : A line plot is created to visualize the number of orders per hour.
- **Top 10 Products Plot** : A bar plot is created to visualize the top 10 best-selling products.
- **Product Combinations Plot** : A horizontal bar plot is created to visualize the products frequently bought together.
