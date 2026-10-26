# Toy Store KPI Report

An interactive Power BI dashboard designed to analyze the key performance indicators of a toy store.

## Project Overview

The **Toy Store KPI Report** provides an overview of sales performance across products, store locations, categories, and time.

The project was built using multiple related tables and a structured data model to transform raw sales data into clear and actionable business insights.

## Business Questions

This report helps answer questions such as:

- How many orders were placed?
- What are the total revenue and profit figures?
- How does revenue change over time?
- Which product categories generate the most orders?
- How does performance vary by store location?
- What are the monthly sales and profit trends?

## Data Sources and Tables

The data model consists of the following tables:

- **Sales**: The main fact table containing sales transactions.
- **Products**: Product details, including product names, categories, costs, and prices.
- **Stores**: Store information, including store names, locations, cities, and opening dates.
- **Calendar**: A dedicated date table used for time-based analysis.

## Data Modeling

The model follows a star schema structure:

- `Sales` is the fact table.
- `Products`, `Stores`, and `Calendar` are dimension tables.
- Relationships were created between the tables using the appropriate keys, including Product ID, Store ID, and Date.

This structure helps organize the data and enables consistent filtering and analysis across products, stores, and time periods.

## Data Preparation and Transformation

The data was prepared and enhanced before creating the dashboard. The main improvements included:

- Adding a calculated **Revenue** column.
- Adding a calculated **Profit** column.
- Creating and organizing a dedicated Calendar table.
- Creating date hierarchies for time-based analysis.
- Adding **Start of Month** and **Start of Week** fields.
- Preparing the data model for monthly and weekly trend analysis.

## Dashboard KPIs and Analysis

The dashboard presents the following key insights:

- Total Orders
- Total Revenue
- Total Profit
- Orders by Product Category
- Monthly Revenue Trends
- Monthly Profit Trends
- Store Performance by Location
- Time-based performance analysis

## Dashboard Preview

![Toy Store KPI Dashboard](screenshots/dashboard.png)

## Data Model

![Toy Store Data Model](screenshots/data-model.png)

## Tools and Skills Used

- Microsoft Power BI
- Power Query
- DAX
- Data Cleaning and Transformation
- Data Modeling
- Star Schema Design
- Calendar and Time-Based Analysis
- KPI Development
- Data Visualization
- Dashboard Design

## Project Structure

```text
toy-store-kpi-report/
│
├── README.md
├── dashboard/
│   └── Toy_Store_KPI_Report.pbix
├── data/
│   ├── sales.csv
│   ├── products.csv
│   ├── stores.csv
│   └── calendar.csv
├── screenshots/
│   ├── dashboard.png
│   └── data-model.png
└── documentation/
    └── project-notes.md
```

> Update the filenames and folder structure if your actual files have different names.

## How to View the Project

1. Download or clone this repository.
2. Open the `.pbix` file using Microsoft Power BI Desktop.
3. If the data source paths are different, update the data source connections in Power Query.
4. Refresh the data if required.

## Notes

The dashboard was created for learning, portfolio, and analytical demonstration purposes. If the original dataset is not included in the repository, a sample or anonymized version can be provided instead.

## Author

Created as a Power BI data analysis project focused on retail sales performance and KPI reporting.
