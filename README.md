# 🛒 Retail Sales Analysis — SQL Project

## 📌 Project Overview

This project analyzes retail sales data using **SQL** to uncover meaningful business insights such as customer behavior, product performance, and sales trends.  
The dataset was **self-created** and exported for practice purposes, making this project a complete end-to-end SQL case study.

---

## 🧰 Tools & Technologies

- **Database:** MySQL  
- **Language:** SQL  
- **Techniques Used:**
  - Table creation & data insertion  
  - Data cleaning  
  - Aggregations (`SUM`, `AVG`, `COUNT`)  
  - Filtering & sorting  
  - Window functions (`RANK() OVER`)  
  - CTE (Common Table Expressions)  
  - Business insight generation  

---

## 🗃️ Dataset Creation

The dataset used in this project was **created manually** using SQL and then populated with sample retail transaction data for learning and analysis.

### Table Structure

```sql
CREATE TABLE retail_sales (
    transactions_id INT PRIMARY KEY,
    sale_date DATE,
    sale_time TIME,
    customer_id INT,
    gender VARCHAR(15),
    age INT,
    category VARCHAR(15),
    quantiy INT,
    price_per_unit FLOAT,
    cogs FLOAT,
    total_sale FLOAT
);
```

## 🧹 Data Cleaning

Records with missing values in key columns were identified and removed:

- `transactions_id`
- `sale_date`
- `sale_time`
- `customer_id`
- `gender`
- `category`
- `quantiy`
- `price_per_unit`
- `cogs`
- `total_sale`

This ensured consistency and accuracy in the analysis.

---

## 🔍 Data Exploration

Key questions explored:

- Total number of sales  
- Total number of unique customers  
- List of product categories  

---

## 📊 Business Questions & SQL Analysis

### 1️⃣ Sales on a Specific Day  
Sales that occurred on **2022-11-05**

### 2️⃣ High-Volume Clothing Sales (Nov 2022)
Transactions where:
- Category = `Clothing`
- Quantity ≥ 4  
- Month = **November 2022**

### 3️⃣ Total Sales & Orders by Category  
Calculated revenue and order volume per category.

### 4️⃣ Average Age of Beauty Customers  
Average customer age for the **Beauty** category.

### 5️⃣ High-Value Transactions  
All transactions with `total_sale > 1000`.

### 6️⃣ Transactions by Gender & Category  
Transaction count by gender across product categories.

### 7️⃣ Best-Selling month of Each Year  
Identified using the `RANK()` window function based on average monthly sales.

### 8️⃣ Top 5 Customers by Total Sales

### 9️⃣ Unique Customers by Category

### 🔟 Orders by Sales Shift  
Orders grouped into:
- **Morning** (<12)
- **Afternoon** (12–17)
- **Evening** (>17)

---

## 🚀 Conclusion

This project demonstrates a complete SQL workflow — from dataset creation to business analysis — making it ideal for portfolio presentation and interview discussions.



