# ecommerce-analysis
Product Sales &amp; Customer Segmentation using Python (RFM Analysis)
# 🛍️ E-Commerce Sales & Customer Segmentation Project

## 📊 Overview
This project analyzes over 500,000 online retail transactions to uncover key product performance insights and segment customers using RFM (Recency, Frequency, Monetary) analysis. The goal is to help businesses better understand their top-performing products and most valuable customers for data-driven marketing and strategy.

---

## 🗂️ Dataset
- **Source:** [Kaggle - Online Retail Dataset](https://www.kaggle.com/datasets/carrie1/ecommerce-data)
- **Rows:** ~500,000
- **Period:** December 2010 to December 2011
- **Columns:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## 🧹 Data Cleaning
- Removed canceled orders (`InvoiceNo` starting with 'C')
- Dropped rows with missing `CustomerID`
- Filtered out invalid quantities and unit prices (≤ 0)
- Converted `InvoiceDate` to datetime format
- Created new column: `Revenue = Quantity × UnitPrice`

---

## 📈 Product Sales Analysis
- **Total revenue** calculated from cleaned data
- **Top 10 products** by revenue visualized using bar chart
- **Monthly revenue trends** analyzed with line plot
- **Revenue by country** identified key markets (UK led with ~90% share)

---

## 👥 Customer Segmentation (RFM Analysis)
- **Recency**: Days since last purchase
- **Frequency**: Number of purchases
- **Monetary**: Total spending
- Customers were scored on each metric (1–4) and grouped into segments:
  - 🏆 **Champions**: Recent, frequent, high spenders
  - ⚠️ **At Risk**: Haven't purchased recently, low frequency
  - 🆕 **New Customers**: Recent but low frequency

---

## 🧠 Key Insights
- A small % of products generate the majority of revenue.
- The UK dominates as the primary market (~90%+ revenue).
- A small segment of “Champions” accounts for significant revenue.
- There's potential to reactivate “At-Risk” customers with personalized offers.

---

## 💡 Recommendations
- Focus loyalty campaigns on Champions.
- Offer discounts or follow-ups to At-Risk customers.
- Invest more in top products and drop underperforming items.
- Consider expanding into other countries with high-potential customer bases.

---

## 🛠️ Tools Used
- Python (pandas, matplotlib, seaborn)
- Jupyter Notebook
- Excel (optional)
- Git & GitHub

---

## 📁 Project Structure
