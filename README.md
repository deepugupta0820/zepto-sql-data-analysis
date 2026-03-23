# 🛒 Zepto SQL Data Analysis Project

## 📌 Project Overview
This project focuses on **data preprocessing and advanced SQL-based analysis** of a product dataset (Zepto Inventory). The goal is to extract meaningful business insights such as pricing patterns, discount effectiveness, inventory distribution, and category-level performance.

---

## 🗂️ Database Schema

### 📦 Table: `zepto`

| Column Name | Data Type | Description |
|------------|----------|-------------|
| sku_id | SERIAL (PK) | Unique product ID |
| category | VARCHAR(120) | Product category |
| name | VARCHAR(150) | Product name |
| mrp | NUMERIC(8,2) | Maximum Retail Price |
| discountPercent | NUMERIC(5,2) | Discount percentage |
| availableQuantity | INTEGER | Available stock |
| discountedSellingPrice | NUMERIC(8,2) | Final selling price |
| weightInGms | INTEGER | Product weight in grams |
| outOfStock | VARCHAR(10) | Stock status |
| quantity | INTEGER | Quantity info |

---

## 📊 Data Analysis Queries

### 🔹 Data Exploration & Preprocessing
- Check for missing (NULL) values in the dataset  
- Identify unique product categories  
- Analyze products in stock vs out of stock  
- Detect duplicate product names (multiple SKUs)  
- Identify products with invalid pricing (MRP = 0)  
- Convert price values from paise to rupees  

---

### 🔹 Business Insights & Analysis

#### 🛍️ Product & Pricing Analysis
- Top 10 products with the highest discount percentage  
- Products with high MRP but currently out of stock  
- Most expensive product in each category  
- Products with high price but low discount  
- Discount effectiveness (customer savings per product)  

---

#### 📦 Inventory & Category Analysis
- Total estimated revenue per category  
- Total inventory weight per category  
- Top 5 most stocked products  
- Categories with highest stock-out percentage  
- Identification of slow-moving products (high stock, low discount)  

---

#### ⚖️ Value-Based Analysis
- Best value products based on price per gram  
- Product segmentation into Low, Medium, and Bulk categories  

---

#### 🔍 Data Quality & Validation
- Duplicate product detection (same name and price)  

---

### 🔹 Advanced SQL Analysis

#### 📊 Statistical Analysis
- Detection of price outliers using standard deviation  
- Categories with highest price variability  

---

#### 🧠 Window Functions
- Ranking products by price and discount (comparison analysis)  
- Dividing products into quartiles based on price distribution  

---

#### 📈 Business Metrics
- Category-wise contribution to total revenue (%)  
- Weighted average price per category  

---

## 🎯 Summary

This project includes:
- Data cleaning and preprocessing  
- Exploratory data analysis  
- Advanced SQL techniques  
- Business-focused insights generation  
