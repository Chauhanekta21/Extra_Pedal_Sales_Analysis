# Extra Pedal Sales Analysis

<<<<<<< HEAD
## Project Overview

This project focuses on building a professional sales analytics dashboard using Power BI. The workflow covers data preparation, transformation, modeling, visualization, and dashboard storytelling based on raw sales-related datasets.

## Source Files and Columns

The project uses the following raw files from the Data/Raw folder:

### 1. Sales 2015.csv
- Columns:
  - OrderDate
  - StockDate
  - OrderNumber
  - ProductKey
  - CustomerKey
  - TerritoryKey
  - OrderLineItem
  - OrderQuantity

### 2. Sales 2016.csv
- Columns:
  - OrderDate
  - StockDate
  - OrderNumber
  - ProductKey
  - CustomerKey
  - TerritoryKey
  - OrderLineItem
  - OrderQuantity

### 3. Sales 2017.csv
- Columns:
  - OrderDate
  - StockDate
  - OrderNumber
  - ProductKey
  - CustomerKey
  - TerritoryKey
  - OrderLineItem
  - OrderQuantity

### 4. Customers Table.csv
- Columns:
  - CustomerKey
  - Prefix
  - FirstName
  - LastName
  - BirthDate
  - MaritalStatus
  - Gender
  - EmailAddress
  - AnnualIncome
  - TotalChildren
  - EducationLevel
  - Occupation
  - HomeOwner

### 5. Products.csv
- Columns:
  - ProductKey
  - ProductSubcategoryKey
  - ProductSKU
  - ProductName
  - ModelName
  - ProductDescription
  - ProductColor
  - ProductSize
  - ProductStyle
  - ProductCost
  - ProductPrice

### 6. Product Categories.csv
- Columns:
  - ProductCategoryKey
  - CategoryName

### 7. Product Subcategories.csv
- Columns:
  - ProductSubcategoryKey
  - SubcategoryName
  - ProductCategoryKey

### 8. Territories.csv
- Columns:
  - SalesTerritoryKey
  - Region
  - Country
  - Continent

### 9. Returns.csv
- Columns:
  - ReturnDate
  - TerritoryKey
  - ProductKey
  - ReturnQuantity

### 10. Calendar.csv
- Columns:
  - Date

## Dashboard Demo

![Dashboard Demo](Gif/dashboard_demo2.gif)


=======
## 🔹 Project Overview
>>>>>>> 692cf32e64568b934c36889ab60a35973e1d85b6

-  This project is a business intelligence dashboard built in Microsoft Power BI to analyze sales performance, product contribution, regional trends, customer behavior, and return impact. 

-  The objective was to transform raw sales data into a structured, interactive dashboard that can support business decision-making and present insights clearly.

-  The project follows a complete analytics workflow starting from raw CSV files and ending with a professional dashboard presentation.

---

## 🔹 Business Problem

Raw sales data alone does not provide immediate business value unless it is cleaned, modeled, and visualized properly. This project addresses that gap by helping answer key questions such as:

- Which products are driving the highest sales?
- Which regions and territories are performing best?
- How do returns affect overall sales performance?
- Which product categories are contributing most to revenue?
- How can sales trends be interpreted across multiple years?

---

## 🔹 Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Data Modeling
- Data Cleaning and Transformation
- Dashboard Design

---

## 🔹 Dataset Overview

The project uses multiple raw CSV files stored in the data folder. The data covers sales transactions, customer information, product details, territories, product hierarchy, and return records

### Source Files Used

- Sales 2015.csv             
- Sales 2016.csv               
- Sales 2017.csv             
- Customers Table.csv        
- Products.csv               
- Product Categories.csv     
- Product Subcategories.csv  
- Territories.csv            
- Returns.csv                
- Calendar.csv


### Dataset Link :- https://github.com/Chauhanekta21/Extra_Pedal_Sales_Analysis/tree/main/Data/Raw


---

## 🔹 Analytics Workflow

```text
Raw Data
    ↓
Data Import
    ↓
Data Cleaning
    ↓
Data Transformation
    ↓
Data Modeling
    ↓
DAX Measures
    ↓
Charts & Visuals
    ↓
Interactive Dashboard
```

---

## 🔹 Data Preparation and ETL Process

### 1. Data Import
- Imported raw CSV files into Power BI from the data folder.
- Loaded sales data from multiple yearly files.
- Added supporting tables for products, customers, territories, calendar, and returns.

### 2. Data Cleaning
- Promoted the first row to column headers across all tables.
- Removed unnecessary rows from the raw datasets.
- Standardized date formats across transaction and return files.
- Checked and corrected data types for quantity, cost, and price-related fields.

### 3. Data Transformation
- Appended the yearly sales datasets (2015, 2016, and 2017) into a single **Final Sales** table.
- Organized product information into category and subcategory hierarchies.

### 4. Data Loading
- Loaded the transformed tables into the Power BI data model.
- Established relationships between fact and dimension tables to create a star schema.
- Validated the model before creating DAX measures and dashboard visualizations.

---

## 🔹 Data Model

The project uses a relational data model where sales transactions are linked to product, customer, territory, and time-related data. This makes the dashboard more scalable and allows multiple perspectives of the same business dataset.

![Data Model](Images/data_model.png)

---


