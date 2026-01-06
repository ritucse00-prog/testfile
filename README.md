# Inventory KPI Analysis using Power BI

## Problem Statement

Efficient inventory management requires a clear understanding of **product demand**, **availability**, **supply shortages**, and **financial impact**.
Organizations often face losses due to:

- Mismatch between demand and availability

- Unidentified supply shortages

- Lack of visibility into profit and loss trends

This project aims to solve these issues by creating **key inventory KPIs** using Power BI and DAX to support **data-driven decision-making**.

## Column Review

The dataset consists of multiple columns that describe product demand, availability, and financial impact. The **order_date** column is stored in **DD-MM-YYYY** format and represents the date on which product demand was recorded. **Product_Id** uniquely identifies each product, while **Product Name** stores the descriptive name of the product. The **Availability** column indicates the quantity of stock available for a product, and **Demand** represents the number of units requested by customers. **Unit Price** captures the price per unit of each product and is used to calculate financial metrics. Finally, the **Profit / Loss** column reflects the monetary outcome resulting from the difference between demand and availability.

| ***Column Name*** | ***Data Type*** | ***Description*** |
|------------|----------|------------|
| **order_date** | Date(DD-MM-YYYY) |Date on which demand was recorded |
| **Product_Id** | Text / Integer | Unique product identifier |
| **Product Name** | Text | Name of the product |
| **Availability** | Integer | Available product quantity |
| **Demand** | Integer | Customer demand quantity |
| **Unit Price** | Decimal | Price per unit of the product |
| **Profit / Loss** | Decimal | Financial outcome based on supply-demand gap |

## DAX Performed & Newly Created Columns

- DAX measures were created directly in Power BI

- These measures help calculate:

  - Daily averages

  - Supply shortages

  - Profit and loss values

- Additional calculated columns/measures were used to:

  - Identify demand exceeding availability

  - Compute financial impact using unit price

## KPI Details & Explanation

### 1. Average Demand per Day
- Calculates the **average customer demand per day**
- Helps in understanding consumption patterns
- Useful for demand forecasting

### 2. Average Availability per Day
- Shows **average stock availability per day**
- Used to compare against daily demand
- Helps detect under-stocking or over-stocking

### 3. Total Supply Shortage
- Measures total quantity where **demand exceeds availability**
- Highlights inventory gaps
- Critical for supply chain planning

### 4. Total Profit
- Calculates total revenue generated from fulfilled demand
- Indicates inventory efficiency and performance

### 5. Total Loss 
- Represents financial loss due to insufficient stock
- Helps identify costly shortages

### 6. Average Daily Loss
- Calculates **average loss per day**
- Useful for monitoring long-term inventory risk

## Report Description

The Power BI report is designed to provide a **clear and intuitive KPI-based view** of inventory performance.
It focuses on:

  - Demand vs availability comparison

  - Supply shortage identification

  - Profit and loss analysis

The visuals enable **quick decision-making** for inventory optimization. The report also includes interactive filters that allow users to analyze KPIs based on 
Product Name and Order Date, enabling flexible and focused inventory analysis.

### Page 1: Inventory Demand & Supply Analysis

This page focuses on operational KPIs:

- Average Demand per Day

- Average Availability per Day

- Total Supply Shortage

### Page 2: Financial Impact Analysis
This page highlights financial KPIs:
- **Total Profit**

- **Total Loss**

- **Average Daily Loss**

## Conclusion
This project demonstrates how Power BI and DAX can be used to convert raw inventory data into meaningful **KPIs** and **business insights**.

