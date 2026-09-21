# Business Performance Intelligence Dashboard

## 📊 Project Overview

This project was developed as part of a Business Intelligence and Data Analytics portfolio project.

The goal was to analyze business performance data and build an interactive Power BI dashboard that helps management understand:

- How the business is performing
- What factors are driving performance
- Which areas require attention
- Where management can focus to improve business results

The project covers data preparation, data modeling, DAX calculations, visualization, and business insights using Microsoft Power BI.

---

## 🎯 Business Problem

Management needs a clear and interactive way to monitor business performance and identify areas that require attention.

The dashboard was designed to answer questions such as:

1. What is the total revenue generated?
2. How many orders were placed?
3. How many unique customers made purchases?
4. What is the average order value?
5. Which states are generating the most revenue?
6. Which product categories perform best?
7. How is revenue changing over time?
8. Which areas are performing above or below expectations?
9. What factors are driving business performance?
10. Where should management focus?

---

## 🛠️ Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Microsoft Excel
- GitHub

---

## 📂 Dataset

The dataset contains information about business sales transactions.

Key fields include:

- Customer
- Product
- Category
- State
- Branch
- Order Date
- Quantity
- Sales
- Cost
- Net Sales

> Note: This dataset is used for educational and portfolio purposes.

---

## 🔄 Data Preparation

The data was prepared using Power Query.

The preparation process included:

- Importing the raw data
- Cleaning missing values
- Removing duplicates
- Correcting data types
- Standardizing text values
- Creating calculated columns where necessary
- Transforming the dataset into a structure suitable for analysis

---

## 🧩 Data Model

The project uses a structured data model consisting of fact and dimension tables.

### Fact Table

**Fact_Sales**

Contains transactional sales information such as:

- Order Date
- Customer ID
- Product ID
- Quantity
- Net Sales
- Cost

### Dimension Tables

- Dim_Customers
- Dim_Products
- Dim_Date
- Dim_Branch

The model was designed to support efficient filtering and analysis across different business dimensions.

---

## 📐 Key DAX Measures

Some of the measures created for the dashboard include:

### Total Revenue

```DAX
Total Revenue =
SUM(Fact_Sales[Net_Sales])
