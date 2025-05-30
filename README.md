# 🛍️ Market Basket Analysis on Online Retail Data

This project performs Market Basket Analysis on retail transaction data using association rule mining with the **Apriori algorithm**. The aim is to uncover patterns and relationships between items frequently purchased together, which can inform marketing strategies, product placement, and inventory management.

The analysis was conducted using Python and the `mlxtend` library, based on a real-world dataset of over 500,000 transactions from an online retailer.

---

## 📌 Project Summary

This project aims to:
- Understand purchasing patterns using **frequent itemsets**
- Generate association rules (like “if X is purchased, Y is likely to be purchased too”)
- Identify **high-confidence product combinations** to support business decisions like promotions or product bundling

The work was completed as part of a practical data mining assignment and uses classic unsupervised learning methods.

---

## 📂 Dataset Overview

**Source**: UCI Machine Learning Repository – Online Retail Dataset   
**Size**: ~540,000 rows, ~4,000 products  
**Scope**:  
- Time range: 2010–2011  
- Includes `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, and `Country`

---

## 🎯 Objectives

- Clean and preprocess transactional data for basket analysis
- Identify frequent itemsets using **Apriori algorithm**
- Generate association rules based on **support, confidence, and lift**
- Interpret results to make retail strategy suggestions

---

## 🧰 Tools & Libraries

- **Languages**: Python  
- **Libraries**:  
  - `pandas` – data manipulation  
  - `mlxtend` – Apriori algorithm and rule generation  
  - `matplotlib`, `seaborn` – data visualization 

---

## 🧪 Methodology

### 1. Data Preprocessing
- Loaded and cleaned the transaction data.
- Removed invalid or canceled transactions.
- Transformed the data into a one-hot encoded format suitable for the Apriori algorithm.

### 2. Frequent Itemset Mining
- Applied the **Apriori algorithm** to find frequent itemsets.
- Set a minimum support threshold to filter out infrequent combinations.

### 3. Rule Generation
- Generated association rules using the frequent itemsets.
- Filtered rules based on meaningful **confidence** and **lift** thresholds.

### 4. Visualization & Interpretation
- Visualized key rules and metrics.
- Interpreted item relationships and actionable insights.

---

## 📊 Key Findings

- Found strong associations such as:
  > Customers who buy **"ALARM CLOCK BAKELIKE RED"** also tend to buy **"ALARM CLOCK BAKELIKE GREEN"** – with high confidence and lift.
- Identified potential product bundles ideal for promotions.
- Demonstrated how association rule mining can support strategic retail decisions (e.g., cross-selling, store layout planning).
