# 📋 Financial Dashboard in Excel

## 📌 Problem Statement
Managing finances is a crucial aspect of both personal and business life. However, analyzing hundreds of raw transaction rows in Excel makes it difficult to:

- Track monthly income and expenses
- Identify spending patterns and overspending categories
- Monitor credits, debits, and net balances
- Visualize financial trends over time

The objective of this project is to develop a user-friendly **Excel-based Financial Dashboard** that offers a clean visual representation of all financial activities to help users make informed decisions.

---
![Download Dataset](https://github.com/SRK0724/Financial-Planning/blob/main/Finance%20Expenses%20Data.xlsx)
## 🧐 Project Process

### 1. 📂 Dataset Preparation
- The original dataset contained a mix of:
  - Pre-labeled month names (e.g., "Jan", "Feb")
  - Full date formats (e.g., "01-13-2021")
- To fix inconsistent month labeling, the following Excel formula was used to extract the correct month:
  ```excel
  =IFERROR(TEXT(DATE(MID(A2,7,4), MID(A2,1,2), MID(A2,4,2)), "mmm"), A2)
  ```
- Cleaned and categorized each transaction with:
  - `Amount`
  - `Category`
  - `Sub-category`
  - `Type` → Credit or Debit

### 2. 📊 Data Analysis Using Pivot Tables
- Used pivot tables to summarize:
  - Monthly financial data
  - Category-wise expenses and incomes
  - Sub-category breakdown
- Created calculated fields to separate **Credit** and **Debit** totals

### 3. 🎨 Dashboard Design in Excel
#### 🔹 Components:
- **Header Summary Cards** showing:
  - Total Amount
  - Total Credit
  - Total Debit
- **Amount by Description**: Vertical bar chart
- **Debit by Category**: Line chart with value labels
- **Amount by Category Type**: Donut chart for Income vs Expenses
- **Credit by Sub-Category**: Horizontal bar chart
- **Credit by Category Type**: Pie chart
- **Month-wise Filter**: Interactive slicer for Jan, Feb, Mar

#### 🔺 Formatting:
- Color-coded charts for better differentiation
- Centered text, rounded corners, and background gradients
- Interactive and dynamic filters using slicers

---

## 🖼️ Dashboard Preview

![Dashboard Preview](https://github.com/SRK0724/Financial-Planning/blob/main/Financial%20Planning%20Dashboard.png)

---

## 💻 Tools Used
- Microsoft Excel
- Excel Formulas (`TEXT`, `DATE`, `IFERROR`)
- Pivot Tables
- Pivot Charts (Bar, Line, Pie, Donut)
- Excel Slicers

---

## 🚀 Future Enhancements
- Add Year filter and multi-year comparison
- Connect live data via Power Query
- Integrate with Power BI for advanced analytics
- Automate monthly financial reporting

---

## 🙌 Author
**Likitha**  
B.Tech CSE Graduate | Excel & Data Analytics Enthusiast  
[LinkedIn](https://www.linkedin.com/in/sivaramakrishnacareergpt) | [Email](mailto:sivaramakrishnabandla970@gmail.com)

---

## 📨 Feedback & Contributions
Feel free to open issues, suggest improvements, or contribute to this project. Your input is always welcome!
