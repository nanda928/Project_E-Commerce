# E-Commerce Data Analysis using BigQuery

## 📌 Description

This project contains SQL-based data analysis on E-Commerce transactional data using Google BigQuery. The analysis explores customer behavior, transaction trends, product performance, reseller identification, dropshipper detection, and payment processing time.

---

# 📊 E-Commerce Data Analysis Project

## 📖 Overview

This project analyzes E-Commerce transaction data using SQL queries in Google BigQuery. The goal is to gain business insights from transactional activities, customer purchasing behavior, and product sales performance.

The dataset includes:

* Orders
* Users
* Order Details
* Products

---

## ⚙️ Tools & Technologies

* Google BigQuery
* SQL
* Google Cloud Platform (GCP)

---

## 📂 Analysis Included

### 1. Top Transactions by User

Identify the largest transactions made by a specific user.

### 2. Monthly Transaction Analysis

Analyze monthly transaction volume and total revenue.

### 3. Highest Average Transaction Users

Find users with the highest average transaction value.

### 4. High Value Transactions

Detect transactions with large purchase values.

### 5. Best Selling Product Categories

Analyze top-selling product categories based on quantity sold.

### 6. High Value Buyers

Identify customers with consistently high transaction values.

### 7. Dropshipper Detection

Detect users potentially acting as dropshippers based on shipping behavior.

### 8. Offline Reseller Identification

Identify reseller-type customers with large quantity purchases and matching postal codes.

### 9. Buyer & Seller Analysis

Find users who act as both buyers and sellers.

### 10. Payment Processing Analysis

Analyze the average time required for transactions to be paid.

---

## 🗂 Dataset Structure

### orders

Contains transaction information:

* order_id
* buyer_id
* seller_id
* total
* created_at
* paid_at
* delivery_at

### users

Contains user information:

* user_id
* nama_user
* kodepos

### order_details

Contains product transaction details:

* order_id
* product_id
* quantity
* price

### product

Contains product category information:

* product_id
* category

---

## 🚀 Example Query

```sql
SELECT seller_id,
       buyer_id,
       total AS nilai_transaksi,
       created_at AS tanggal_transaksi
FROM project.orders
WHERE buyer_id = 12476
ORDER BY 3 DESC
LIMIT 10;
```

---

## 📈 Key Insights

* Customer purchasing behavior patterns
* Monthly revenue trends
* Product category performance
* Potential reseller and dropshipper identification
* Transaction payment efficiency

---

## 👨‍💻 Author

Ananda Pradewa Dyah Kurniawan Putra
