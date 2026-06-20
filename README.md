# Sales_Analytics_DataModel.xlsx
End-to-end Sales Data Cleaning and Data Modeling project using Excel, Power Query, and Power Pivot. Includes data transformation, standardization, calculated metrics, calendar table creation, and star schema modeling.
📊 Sales Data Cleaning & Data Modeling Project
📌 Project Overview

This project focuses on cleaning, transforming, and modeling raw sales data using Microsoft Excel, Power Query, and Power Pivot. The dataset contained inconsistent values, duplicate records, formatting issues, and missing data. The objective was to prepare an analytics-ready dataset and build a structured data model for reporting and dashboard creation.

🎯 Objectives
Clean and standardize raw sales data
Remove duplicates and invalid records
Convert data into proper formats
Create calculated business metrics
Build dimension tables
Create a Calendar table
Establish relationships using a star schema data model
🛠️ Tools Used
Microsoft Excel
Power Query
Power Pivot
Data Model
🔄 Data Cleaning Process
1. Header Preparation
Promoted first row as headers
Verified column names
2. Text Cleaning
Applied Trim and Clean functions
Removed extra spaces and hidden characters
3. Data Standardization

Standardized inconsistent values such as:

Raw Value	Standard Value
electronics	Electronics
ELECTRONICS	Electronics
delivered	Delivered
DELIVERED	Delivered
4. Duplicate Removal
Removed duplicate records using Order ID
5. Data Type Conversion
Column	Data Type
Order Date	Date
Quantity	Whole Number
Unit Price	Decimal Number
Discount	Decimal Number
Shipping Fee	Decimal Number
6. Error Handling
Removed invalid rows
Fixed date and numeric conversion issues
7. Mobile Number Formatting
Added country code (+91) to customer phone numbers
📈 Calculated Columns Created
Gross Sales
Quantity × Unit Price
Discount Amount
Gross Sales × Discount
Net Sales
Gross Sales − Discount Amount
Final Sales
Net Sales + Shipping Fee
📅 Time Intelligence Columns
Month
Jan-2026
Feb-2026
Mar-2026

Created using Order Date.

Quarter
Q1-2026
Q2-2026
Q3-2026

Created using Order Date.

🏗️ Data Modeling
Product Master Table

Created a Product Dimension table using:

Product
Category

Removed duplicate records to maintain unique products.

Calendar Table

Created a Date Dimension table based on the valid Order Date range.

Included:

Date
Year
Month
Quarter
Relationships
DimCalendar
     |
     |
FactSales
     |
     |
DimProduct

Implemented a Star Schema model using Power Pivot.

📊 Key Learning Outcomes
Data Cleaning using Power Query
Data Transformation Techniques
Handling Missing and Duplicate Data
Data Standardization
Data Modeling using Power Pivot
Creating Dimension Tables
Building Star Schema Relationships
Preparing Data for BI Reporting
🚀 Future Scope
Create interactive Excel Dashboard
Build Power BI Dashboard
Add KPI Cards and Visualizations
Perform Sales Trend Analysis
Develop Business Performance Reports
👨‍💻 Author

Ravi Kumar

BCA Student | Data Analytics Enthusiast

Skills: Excel, Power Query, Power Pivot, SQL, Power BI, Python
