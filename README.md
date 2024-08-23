# BLINKIT_SALES_DASHBOARD

### Overview
The Blinkit Sales Analysis Dashboard is designed to analyze and optimize sales performance, customer satisfaction, and inventory management across various outlets. This guide explains the steps to create the dashboard using Power BI, from data preparation to generating actionable insights.

### Project Steps to Create the Blinkit Dashboard

1. **Requirement Gathering**:
   - **Objective**: Understand Blinkit’s business needs and define the KPIs that will drive the analysis.
   - **Actions**:
     - Get the Data From the Kaggle.
     - Identify key metrics such as Total Sales, Average Sales, Number of Items Sold, and Average Rating.
     - Document the requirements for visualizations (e.g., charts, maps).

2. **Data Walkthrough**:
   - **Objective**: Familiarize yourself with the data available for the dashboard.
   - **Actions**:
     - Access the sales, inventory, and customer feedback data.
     - Review the data structure, including tables and relationships.
     - Identify any data gaps or quality issues that need addressing.

3. **Data Connection**:
   - **Objective**: Connect Power BI to the data sources.
   - **Actions**:
     - Import data from various sources such as databases, Excel, or CSV files into Power BI.
     - Ensure all necessary tables are loaded into the Power BI workspace.
     - Verify the integrity of the connections to ensure all data is accessible.

4. **Data Cleaning/Quality Check**:
   - **Objective**: Prepare the data for analysis by cleaning and ensuring data quality.
   - **Actions**:
     - Use Power Query to remove duplicates, handle missing values, and correct any errors.
     - Standardize formats for dates, numbers, and text fields.
     - Filter out any irrelevant data that doesn’t contribute to the analysis.

5. **Data Modeling**:
   - **Objective**: Build a logical data model to support the required analysis.
   - **Actions**:
     - Define relationships between tables (e.g., linking sales data with outlet and product data).
     - Create calculated columns if needed to support the KPIs.
     - Design the data model to be efficient and easy to query.

6. **Data Processing**:
   - **Objective**: Transform and process the data for optimal performance.
   - **Actions**:
     - Apply necessary transformations in Power Query (e.g., unpivoting columns, creating new fields).
     - Aggregate data where needed to improve performance.
     - Ensure data is ready for use in visualizations.

7. **DAX Calculations**:
   - **Objective**: Develop the necessary DAX measures to calculate KPIs.
   - **Actions**:
     - Create DAX measures for Total Sales, Average Sales, Number of Items Sold, and Average Rating.
     - Example DAX Queries:
       - **Total Sales**: `Total Sales = SUM(Sales[Revenue])`
       - **Average Sales**: `Average Sales = DIVIDE([Total Sales], COUNT(Sales[TransactionID]))`
       - **Number of Items Sold**: `Number of Items Sold = SUM(Sales[Quantity])`
       - **Average Rating**: `Average Rating = AVERAGE(Sales[CustomerRating])`

8. **Dashboard Layouting**:
   - **Objective**: Design the visual layout of the dashboard.
   - **Actions**:
     - Sketch a layout that highlights key insights (e.g., placing Total Sales prominently).
     - Plan the flow of information from general (e.g., total sales) to specific (e.g., sales by outlet).
     - Ensure the layout is intuitive and user-friendly.

9. **Charts Development and Formatting**:
   - **Objective**: Create and format visualizations to represent the data effectively.
   - **Actions**:
     - Develop the required charts, such as donut charts, bar charts, stacked column charts, and funnel maps.
     - Format the visuals for clarity (e.g., choosing appropriate colors, adding labels and tooltips).
     - Ensure that charts are aligned and consistent in style.

10. **Dashboard/Report Development**:
    - **Objective**: Assemble the dashboard by combining all visual elements.
    - **Actions**:
      - Place all visuals on the Power BI canvas according to the layout plan.
      - Add slicers and filters to allow users to interact with the data (e.g., filter by outlet or date range).
      - Test the dashboard to ensure all interactions work as intended.

11. **Insights Generation**:
    - **Objective**: Analyze the completed dashboard to generate actionable insights.
    - **Actions**:
      - Review the visualizations to identify trends and patterns (e.g., which outlets have the highest sales?).
      - Summarize key findings that can inform business strategies (e.g., identifying top-performing products).
      - Share insights with stakeholders to guide decision-making.

### Project Requirements

- **Data Sources**: Sales data, customer feedback, and inventory data.
- **Key Metrics**:
  - **Total Sales**: Overall revenue generated.
  - **Average Sales**: Revenue per transaction.
  - **Number of Items Sold**: Total quantity of items sold.
  - **Average Rating**: Customer satisfaction scores.
  
- **Visualizations**:
  - **Sales by Fat Content**: Donut chart to analyze sales impact by fat content.
  - **Sales by Item Type**: Bar chart to compare item performance.
  - **Sales by Outlet**: Stacked column chart to compare outlets by fat content.
  - **Sales by Outlet Size**: Pie chart to explore sales by outlet size.
  - **Sales by Location**: Funnel map for geographic distribution of sales.

### Key DAX Queries

- **Total Sales**:
  ```DAX
  Total Sales = SUM(Sales[Revenue])
  ```

- **Average Sales**:
  ```DAX
  Average Sales = DIVIDE([Total Sales], COUNT(Sales[TransactionID]))
  ```

- **Number of Items Sold**:
  ```DAX
  Number of Items Sold = SUM(Sales[Quantity])
  ```

- **Average Rating**:
  ```DAX
  Average Rating = AVERAGE(Sales[CustomerRating])
  ```

### Insights
By following these steps, the Blinkit Sales Analysis Dashboard will provide valuable insights into sales trends, customer preferences, and inventory management. This tool is essential for making data-driven decisions to optimize performance across Blinkit’s operations.
