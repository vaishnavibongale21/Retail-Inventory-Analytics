# Retail Inventory Analysis Report

## 1. Introduction
This report summarizes the exploratory data analysis and visualization performed on the Retail Inventory dataset. The primary goal was to understand the dataset's structure, identify key trends, and extract actionable business insights from inventory and sales data.

## 2. Objectives
The main objectives of this project were:
*   To load and understand the structure of the Retail Inventory dataset.
*   To clean the data by handling duplicates and validating stock quantities.
*   To perform Exploratory Data Analysis (EDA) to discover patterns and relationships.
*   To visualize key metrics and distributions using various chart types.
*   To generate business insights regarding product performance, stock levels, and supplier distribution.

## 3. Methodology
The analysis followed these steps:
1.  **Data Loading**: The `01 Retail Inventory.xlsx` file was loaded into a pandas DataFrame.
2.  **Data Inspection**: Initial checks were performed using `df.info()`, `df.dtypes`, `df.isnull().sum()`, and `df.duplicated().sum()` to understand data types, missing values, and duplicate records.
3.  **Data Cleaning**: Duplicate rows were removed, and rows with missing values were dropped. Stock quantities were validated to ensure no negative values were present.
4.  **Exploratory Data Analysis (EDA)**:
    *   Calculated category-wise product counts and units sold.
    *   Identified the top 10 best-selling products.
    *   Identified products with low stock levels.
    *   Analyzed supplier-wise inventory distribution.
5.  **Data Visualization**: Various charts were generated to visually represent the data:
    *   Bar chart for Category-wise Product Count.
    *   Pie chart for Category-wise Units Sold.
    *   Histogram for Distribution of Units Sold.
    *   Line graph for Category-wise Units Sold Over Time.
    *   Correlation heatmap for numerical variables.
6.  **Report Generation**: Summarized findings and insights from the analysis.

## 4. Charts
Below are the visualizations generated during the analysis:

*   **Category-wise Product Count**: `bar_chart.png`
    *   *Description*: This bar chart shows the total number of unique products within each category.

*   **Category-wise Units Sold**: `pie_chart.png`
    *   *Description*: This pie chart illustrates the proportion of units sold across different product categories, highlighting which categories contribute most to overall sales volume.

*   **Distribution of Units Sold**: `histogram.png`
    *   *Description*: A histogram displaying the frequency distribution of units sold, providing insights into common sales volumes.

*   **Category-wise Units Sold Over Time**: `line_graph.png`
    *   *Description*: A line graph depicting the trend of units sold per category over time (if time data was present and utilized, or per category as an aggregated view).

*   **Correlation Heatmap**: `correlation_heatmap.png`
    *   *Description*: A heatmap showing the correlation between numerical variables in the dataset, helping to identify strong relationships.

## 5. Business Insights
Based on the analysis, the following business insights were derived:
*   **Product Performance**: The 'Toys & Games' and 'Home & Kitchen' categories consistently show high unit sales, indicating strong customer demand. Conversely, 'Clothing' shows comparatively lower unit sales.
*   **Low Stock Management**: Several products across different categories are frequently in low stock, as evidenced by the 'Closing Stock' and 'Reorder Point' analysis. Proactive reordering for these items, such as 'Water Bottle' and 'Canned Soup' (top sellers often in low stock), is crucial to prevent stockouts and lost sales.
*   **Supplier Contribution**: The distribution of products among suppliers reveals that some suppliers, like 'National Supply Group' and 'Premier Merchandise', supply a larger portion of the inventory. This could inform supplier relationship management and negotiation strategies.
*   **Sales Distribution**: The distribution of units sold indicates that while many products have moderate sales, a few products are exceptionally high-performing, highlighting the importance of identifying and promoting best-sellers.

## 6. Conclusion
This analysis provided a comprehensive overview of the retail inventory, identifying key areas for potential improvement in inventory management, sales strategy and supplier relations. By monitoring top-selling products and proactively managing low stock levels, businesses can optimize their operations and enhance profitability. Further analysis could include predictive modeling for demand forecasting and more detailed profitability analysis per product or category.