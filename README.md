# 📊 Swiggy Sales Analytics

A real-world **E-Commerce / Food Delivery Sales Analytics** project using **Python, Pandas, and NumPy**.  
The project focuses on analyzing sales data and performing data-cleaning operations on a Swiggy sales dataset.

---

## 📌 Project Overview

This project demonstrates how Python and Pandas can be used to transform raw transactional data into meaningful business insights.

The analysis includes:

- Product revenue analysis
- Category-wise sales analysis
- Average order value analysis
- Missing-value detection
- Duplicate-record detection
- Data-type correction
- Category standardization
- Abnormal-value detection

---

## 📂 Dataset

The dataset contains one year of Swiggy sales transactions.

### Dataset Columns

| Column | Description |
|---|---|
| `Date` | Date of the order |
| `Order ID` | Unique order identifier |
| `Item Name` | Name of the food item |
| `Category` | Food category |
| `Quantity` | Quantity ordered |
| `Item Price` | Price of the item |
| `Discount` | Discount applied |
| `GST` | GST amount |
| `Delivery Charges` | Delivery charge |
| `Customer Paid Amount` | Amount paid by customer |
| `Net Sales` | Net sales amount |
| `Payment Method` | Payment method used |
| `Order Status` | Status of the order |

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Google Colab**
- **Jupyter Notebook**

---

## 📈 Business Questions

The project analyzes the following questions:

### 1. Which product generates maximum revenue?

Revenue is grouped by `Item Name` and the product with the highest total revenue is identified.

**Result:**

> Chicken Tikka

---

### 2. Which region has declining sales?

The original case study requires a `Region` column.

However, the provided Swiggy dataset does not contain a `Region` column, so this question cannot be calculated from the available dataset.

---

### 3. Who are the top 10 customers?

The original case study requires a `Customer` column.

The provided Swiggy dataset does not contain customer information, so this question cannot be calculated from the available dataset.

---

### 4. Which category has the highest average order value?

The average revenue is calculated for each food category.

```python
df.groupby("Category")["Revenue"].mean().idxmax()
