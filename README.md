## 📊 Extra Pedal Sales Analysis 
  
## 🔹 Project Overview

This project is an interactive **Microsoft Power BI** dashboard built using the **Extra Pedal Sales** dataset.

The dashboard provides a comprehensive analysis of **sales performance** and the key factors influencing it, including **products, customers, regions, and returns**, through interactive visualizations and KPIs.

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

## 🔹 Date Table Creation

- Replaced the static **Calendar** table with a dynamic **Date** table created using DAX.
- Included key date fields: **Date**, **Month**, and **Year**.
- Marked it as the official **Date Table** and related it to the **Final Sales** table for time-based analysis.

![Data Model](Images/calendar_date_table.png)

---

## 🔹 Data Model

The project uses a relational data model where sales transactions are linked to product, customer, territory, and time-related data. This makes the dashboard more scalable and allows multiple perspectives of the same business dataset.

![Data Model](Images/data_model.png)

---

## 🔹 Calculated Columns

1.  Customers Table
-   IncomeStatus: Used to classify customers into Low Income, Medium Income, and High Income for sales analysis by income group.
-   ParentStatus: Used to identify whether a customer is a parent or not parent, mainly for the product details drill-through report.

2.  Date Table
-   Month: Extracts the month from the date field for monthly trend analysis.
-   Year: Extracts the year for year-wise comparison.
-   MonthYear: Combines Month and Year into a single label, used as the trend axis for Sales KPI and Order KPI.

3.  Final Sales Table
-   Product Price: Used as part of the sales calculation logic.
-   Sales: Represents the final sales value used for KPI reporting and dashboard visuals.

![Data Model](Images/calculated_columns.png)

