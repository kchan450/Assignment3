# Nike Sales Data Analysis

## Project Overview

This project integrates multiple aspects of Nike sales data analysis, combining exploratory data analysis, data cleaning, cost analysis, and profit calculations into a comprehensive study. The dataset consists of global sales transactions and unit cost data, enabling a detailed examination of sales trends, cost structures, and profitability across different product lines and regions.

The primary objectives of this project are to:

- Explore sales trends and patterns across various regions and product lines.
- Ensure data accuracy and integrity through rigorous cleaning and validation.
- Merge sales and cost datasets to compute profit margins and assess financial performance.
- Identify and resolve missing or inconsistent cost data for better insights.
- Use Git for version control to track changes, manage branches, and push updates efficiently.

By combining exploratory analysis, data integration, and visualization techniques, this project provides valuable insights into Nike's global sales performance and cost dynamics.

Git was used for version control to track changes, manage branches, and push updates efficiently.

## Project Structure

### **Key Files and Their Purpose**

- **Assignment3.ipynb** – Exploratory analysis, sales trends, and data cleaning.
- **Assignment5.ipynb** – Data merging (sales + cost), profit calculations, and insights.

### **Key Goals**

- **Sales Trend Analysis**: Explore sales trends across regions and product lines (Assignment 3).
- **Profit Calculation**: Merge sales and cost data to calculate profit (Assignment 5).
- **Data Integrity Check**: Identify and resolve inconsistencies (Assignment 5).

## **Dataset Sources**

### **Dataset 1: Nike Sales Dataset (Nike_sales_2024)**

- Sourced from Kaggle ([Nike Global Sales Data 2024](https://www.kaggle.com/datasets/ayushcx/nike-global-sales-data-2024)).

### **Dataset 2: Nike Unit Cost Dataset (Nike_unitcost)**

- Generated from [Mockaroo](https://www.mockaroo.com/), providing unit costs for different Nike products.

## **Dataset Overview**

### **Sales Dataset (nike_sales.csv)**

| Column | Description |
|--------|-------------|
| Month | The month of the sales transaction |
| Region | The geographical region where the sales occurred |
| Main_Category | Broad category of Nike products |
| Sub_Category | More specific category of Nike products |
| Product_Line | The specific line of products sold |
| Price_Tier | The pricing segment of the product (e.g., premium, mid-range) |
| Units_Sold | Number of units sold |
| Revenue_USD | Revenue generated in USD |
| Online_Sales_Percentage | Percentage of sales made online |
| Retail_Price | The listed price of the product |

### **Cost Dataset (nike_unitcost.csv)**

| Column | Description |
|--------|-------------|
| Product_Line | The specific line of products (matching nike_sales.csv) |
| Price_Tier | The pricing segment of the product |
| Unit_Cost | The cost of producing one unit of the product |

## **Data Processing and Cleaning**

### **Assignment 3: Initial Exploration & Cleaning**
- Checked for missing values in **Units_Sold, Revenue_USD, Retail_Price**.
- Standardized product names for consistency.
- Converted numeric fields to the correct data types.
- Generated summary statistics for sales trends.

### **Assignment 5: Data Merging & Profit Calculation**
- Merged sales & cost data using **LEFT JOIN**.
- Calculated profit for financial insights.
- Visualized key insights using **two charts**.
- Identified missing cost data.

## **Data Visualization**
- Created bar charts, line graphs, and scatter plots to illustrate sales trends across different regions and product lines.
- Visualized profitability metrics to better understand cost vs. revenue.
- Used interactive visualizations to make insights more accessible and interpretable.

## **Data Integration Approach**

### **Using LEFT JOIN for Data Merging**
To merge the sales dataset with cost data, a **LEFT JOIN** was used. This approach ensured that all sales records were retained, even if some cost details were missing. The resulting dataset helped identify missing cost values that required further updates.

## **Challenges & Solutions**

### **Choosing the Right SQL Join**

Initially, an INNER JOIN was used to merge the sales and cost datasets. However, this approach excluded sales records that did not have corresponding cost data, leading to an incomplete analysis. To ensure that all sales records were retained, a LEFT JOIN was implemented instead. This allowed for the integration of cost data while keeping all sales records, ensuring a more comprehensive analysis.

Another challenge was considering a RIGHT JOIN, which prioritized cost data over sales records. However, since the focus of the analysis was on sales trends and profitability, this approach was not useful. The LEFT JOIN ultimately provided the best balance, ensuring that all sales data remained while incorporating available cost information.

## **Final Thoughts**
By leveraging exploratory analysis, data cleaning, and proper data integration techniques, this project successfully examined Nike sales trends while ensuring data consistency. The use of **LEFT JOIN** allowed for comprehensive profit analysis without losing critical sales information.


