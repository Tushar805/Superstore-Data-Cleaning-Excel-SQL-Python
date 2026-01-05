# 🧹 Superstore Data Cleaning – Excel | SQL | Python

## 📌 Project Overview
This project demonstrates a **complete real-world data cleaning workflow** using the **same dataset** across **three different tools**:  
**Excel (Power Query), SQL Server, and Python (Pandas)**.

The goal is to show how data cleaning techniques vary across tools while achieving a **clean, consistent, and analysis-ready dataset**.

Dataset used: **Superstore dataset from Kaggle**.

---

## 🗂️ Dataset Details
- **Source**: Kaggle – Superstore Dataset  
- **Original Size**: 9,994 rows × 21 columns  
- **Final Clean Size**:  
  - Excel / Python → **9,986 rows**  
  - SQL → **9,993 rows**  
- **Data Type**: Orders, Customers, Products, Sales, Profit, Shipping  

---

## 🛠️ Tools Used
- **Excel** – Power Query  
- **SQL Server** – Data Cleaning & Schema Optimization  
- **Python** – Pandas (Jupyter Notebook)

---

## 🔁 Cleaning Approaches Covered

### 1️⃣ Excel (Power Query)
- Removed non-analytical columns (Row ID)
- Verified and corrected data types
- Trimmed and cleaned all text columns
- Validated column quality and distribution
- Removed true duplicates using Order ID + Product ID
- Created derived column **Delivery Days**
- Standardized categorical values
- Renamed columns for better readability

📌 **Result**: Clean, structured, and business-ready Excel dataset.

---

### 2️⃣ SQL Server
- Imported CSV using Flat File Wizard
- Verified schema and row counts
- Assigned **Primary Key (Row_ID)**
- Created derived column **DaysToShip**
- Trimmed and standardized text fields
- Identified and removed duplicates using `ROW_NUMBER()` and CTEs
- Optimized numeric data types for precision
- Fixed real-world issue of **truncated product names** by:
  - Expanding column size
  - Re-importing original data
  - Restoring values via JOIN
- Performed final validation checks

📌 **Result**: Optimized, reliable, analytics-ready SQL table/CSV file.

---

### 3️⃣ Python (Pandas)
- Imported dataset into DataFrame
- Validated structure and data types
- Standardized column naming conventions
- Cleaned text columns (spaces & hidden characters)
- Ensured numeric columns were correctly typed
- Converted date columns to datetime
- Added analytical features:
  - Days to Ship
  - Profit Margin
  - Order Year & Month
- Applied logical validations (e.g., sales > 0)
- Removed duplicates programmatically
- Performed Unicode normalization
- Revalidated entire dataset

📌 **Result**: Fully standardized, scalable, and repeatable cleaning pipeline.

---

## 📂 Repository Structure
- `data/` → Original and cleaned datasets  
- `excel_cleaning/` → Power Query steps & cleaned Excel file  
- `sql_cleaning/` → SQL scripts for cleaning & validation  & cleaned CSV file
- `python_cleaning/` → Jupyter Notebook & cleaned Excel file 
- `README.md` → Project documentation  

---

## ⚡ Key Learnings & Insights
- The **same dataset** can require **different techniques** depending on the tool  
- SQL provides **strong structural control** and schema-level fixes  
- Python enables **scalable and repeatable validation logic**  
- Excel Power Query is excellent for **quick profiling and business users**  
- Real-world issues (like truncated fields) can silently impact data quality  

---

## 🚀 Why This Project Matters
This project highlights:
- Real-world data quality issues  
- Cross-tool cleaning expertise  
- Strong understanding of **data preparation before analysis**  
- Practical, industry-relevant workflows  

It reflects how data cleaning is performed in **actual analytics roles**, not just theory.

---
<img width="386" height="309" alt="Query16" src="https://github.com/user-attachments/assets/2f1190fc-f3c7-45da-aacd-60c576f68405" />

<img width="392" height="340" alt="Query10" src="https://github.com/user-att![Uploading Query16.PNG…]()
achments/assets/ff9d2b50-e128-44dc-8b22-f46728e68867" />

<img width="386" height="311" alt="Query3" src="https://github.com/user-attachments/assets/2492c7dc-1de7-4cfb-b4ac-5806df35c030" />

<img width="664" height="333" alt="Query6" src="https://github.com/user-attachments/assets/4f9dfead-c1ab-4627-949e-80ef2d6c8a07" />
