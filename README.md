# Sales_Analytics_DataModel.xlsx

## 📌 Project Overview

This project demonstrates an end-to-end data cleaning and data modeling workflow using Microsoft Excel, Power Query, and Power Pivot.

The raw sales dataset contained duplicate records, inconsistent text values, invalid dates, formatting issues, and missing values. Using Power Query, the data was cleaned, standardized, and transformed into an analytics-ready dataset. A star schema data model was then built using Power Pivot for reporting and dashboard creation.

---

## 🛠 Tools & Technologies

- Microsoft Excel
- Power Query
- Power Pivot
- Data Model
- Data Cleaning
- Data Transformation
- Data Modeling

---

## 🔄 Data Cleaning Steps

### Data Preparation
- Promoted first row as headers
- Removed unnecessary columns
- Trimmed extra spaces
- Cleaned hidden characters

### Data Standardization
- Standardized Category values
- Standardized Order Status values
- Standardized Payment Mode values
- Standardized State names

### Data Validation
- Removed duplicate records
- Removed blank rows
- Removed error rows
- Fixed invalid date formats

### Data Transformation
- Converted Order Date to Date type
- Converted Quantity to Whole Number
- Converted Unit Price to Decimal
- Converted Discount to Decimal
- Converted Shipping Fee to Decimal
- Added +91 country code to mobile numbers

---

## 📈 Calculated Columns

### Gross Sales

```text
Gross Sales = Quantity × Unit Price
```

### Discount Amount

```text
Discount Amount = Gross Sales × Discount
```

### Net Sales

```text
Net Sales = Gross Sales − Discount Amount
```

### Final Sales

```text
Final Sales = Net Sales + Shipping Fee
```

---

## 📅 Time Intelligence

Created the following columns from Order Date:

- Month (Jan-2026)
- Quarter (Q1-2026)
- Year

---

## 🏗 Data Model

### Product Dimension

Created Product Master table using:

- Product
- Category

Removed duplicate records to maintain unique products.

### Calendar Dimension

Created Calendar Table using valid Order Date range.

Included:

- Date
- Month
- Quarter
- Year

---

## ⭐ Star Schema

```text
                DimCalendar
                     |
                     |
                     |
DimProduct ------ FactSales
```

### Relationships

```text
DimCalendar[Date]
        |
        |
FactSales[OrderDate]

DimProduct[Product]
        |
        |
FactSales[Product]
## 🎯 Key Skills Demonstrated

- Data Cleaning
- Data Transformation
- Power Query
- Power Pivot
- Data Modeling
- Star Schema Design
- Data Validation
- Excel Analytics

---

## 🚀 Future Improvements

- Build Interactive Dashboard
- Power BI Integration
- KPI Tracking
- Sales Trend Analysis
- Customer Insights Dashboard

---

## 👨‍💻 Author

**Ravi Kumar**

BCA Student | Aspiring Data Analyst

Skills: Excel • SQL • Power BI • Python • Power Query • Power Pivot
