# 🛍️ Market Basket Analysis on Online Retail Data

This project applies **association rule mining** to online retail transaction data to uncover patterns in customer purchasing behavior. It uses **Apriori-based market basket analysis** to identify frequently co-purchased items and generate actionable insights about product affinity.

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

- **Python**
- `pandas`, `numpy`
- `mlxtend` for association rules
- `matplotlib`, `seaborn` for plotting
- `openpyxl` for Excel import

---

## 🔍 Methodology

1. **Data Preprocessing**
   - Removed cancelled orders and negative quantities
   - Filtered transactions to UK-based customers
   - Created a **binary basket matrix** using pivoting

2. **Frequent Itemset Mining**
   - Used **Apriori algorithm** to extract itemsets above minimum support threshold

3. **Association Rules Generation**
   - Derived rules using `mlxtend.frequent_patterns.association_rules()`
   - Evaluated rules based on confidence and lift
   - Sorted and visualised top rules for business interpretation

---

## 📊 Key Findings

- Items like **“white hanging heart”**, **“regency cake stand”**, and **“jam making sets”** were frequently purchased together
- High-confidence rules (above 80%) were found in home décor and kitchen accessories
- Lift values > 3 indicate strong product affinity, useful for upselling or cross-promotion strategies
