# 🛍️ E-Commerce Sales Analysis & Customer Segmentation

## 📊 Overview
This project analyzes over 500,000 online retail transactions to uncover product performance insights and segment customers using RFM (Recency, Frequency, Monetary) analysis. The goal is to help businesses identify their most valuable customers and key revenue-driving products using Python.

---

## 📁 Dataset
- **Source:** [Kaggle – Online Retail Data](https://www.kaggle.com/datasets/carrie1/ecommerce-data)
- **Rows:** 500,000+
- **Timeframe:** Dec 2010 – Dec 2011
- **Features:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## 🧹 Data Cleaning
- Removed cancelled orders (`InvoiceNo` starts with 'C')
- Dropped missing `CustomerID` rows
- Removed negative or zero `Quantity` and `UnitPrice`
- Created `Revenue = Quantity × UnitPrice`
- Converted `InvoiceDate` to datetime format

---

## 📈 Product Sales Analysis
- Total Revenue: **~£8.9 million**
- Identified **Top 10 Products** by revenue
- Analyzed **Monthly Revenue Trends**
- Ranked **Top Countries** by revenue (UK led with ~90%)

---

## 👥 Customer Segmentation (RFM)
Calculated:
- **Recency**: Days since last purchase
- **Frequency**: Number of orders
- **Monetary**: Total spending

Customers were scored on each dimension (1–4 scale) and combined into an `RFM_Score`.

**Segments Identified:**
- 🏆 **Champions** (444 score): most loyal and high-spending customers
- 🧊 **At Risk**: infrequent or inactive customers
- ✨ **New Customers**: recent but low frequency
- 📉 **Loyal Customers**: frequent but not high spenders

---

## 📊 Visualizations
- Top 10 products bar chart
- Monthly revenue trend line plot
- Recency, Frequency, Monetary histograms
- Revenue by country bar chart

---

## 💡 Business Insights
- 20% of products drive most revenue
- UK is the core market (90% of revenue)
- Small % of customers generate most revenue (Pareto principle)
- RFM segmentation provides powerful marketing targeting

---

## 📁 Folder Structure

