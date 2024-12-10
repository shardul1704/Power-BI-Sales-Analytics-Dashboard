# Power-BI-Sales-Analytics-Dashboard
Power BI Sales Analytics Dashboard

Project Overview

The goal of this project was to create a one-page, interactive dashboard showcasing key sales metrics using diverse Power BI visuals. The solution supports automatic data refresh, dynamic data modeling, and advanced calculations using DAX.


Data Sources

The following data sources were integrated:

    Sales Data: Yearly sales files (CSV) from a folder.
    Product Data: Product details (CSV/Database).
    Categories & Subcategories: Excel files containing product hierarchy.
    Sales Representatives: Sales team details (Excel).
    Geography: Regional mapping (Excel).


Data Loading & Transformation

    Dynamic File Loading:
        Implemented a dynamic data loading mechanism in Power Query to import multiple yearly sales files from a folder.
        Added error resilience: Removing or adding files does not cause refresh errors.

    Data Transformation Tasks:
        Split the “Location” field into City and Country for geospatial analysis.
        Standardized data types for accurate reporting.
        Created unique GeoKey columns in the Sales and Geography tables.
        Cleaned SalesRep and SubCategory IDs using a reusable custom function in Power Query.


Data Modeling

    Established relationships between the Fact Table (Sales) and Dimension Tables (Product, Categories, Subcategories, SalesRep, Geography).
    Integrated a Calendar Table for time-based calculations.


DAX Calculations

Developed key DAX measures for deep sales analysis:

    Total Revenue: Calculated as Units Sold * Product Retail Price.
    Total Cost: Calculated as Units Sold * Product Standard Cost.
    Gross Profit: Total Revenue - Total Cost.
    Gross Profit MoM Growth %: Monthly growth percentage for trend analysis.
    QoQ Growth: Quarter-over-quarter revenue growth for quarterly reporting.


Technologies Used

    Power BI Desktop (Data Modeling, Dashboard Design)
    Power Query (Data Transformation & Cleaning)
    DAX (Data Analysis Expressions)
    Excel & CSV Files (Data Sources)


![Sales Analytics Example](https://github.com/user-attachments/assets/759d5072-7709-4479-8f32-ff8792d4d28c)
