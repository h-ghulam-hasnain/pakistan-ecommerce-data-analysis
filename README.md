# 🇵🇰 E-commerce Customer Analytics: Segmentation, Risk, and Forecasting

## Project Overview

This repository contains a comprehensive data analysis project focused on customer behavior, revenue trends, and operational risk using a large transactional dataset from a leading Pakistani e-commerce platform.

The goal is to provide **actionable business intelligence** for marketing strategy, customer retention, and inventory management.

---

## 🔬 Analysis & Methodology

The project follows a structured approach covering three main analytical pillars:

### 1. Customer Segmentation (RFM)
* **Goal:** To group customers based on their purchasing habits for targeted marketing campaigns.
* **Methodology:** Implemented the **RFM (Recency, Frequency, Monetary)** model.
* **Output:** Generated distinct customer segments (e.g., Champions, Loyal Customers, At-Risk) for targeted retention strategies.

### 2. Operational Risk Assessment
* **Goal:** Identify and quantify fulfillment issues across product categories.
* **Methodology:** Calculated **Cancellation Rate** for the top 10 categories to expose high-risk areas contributing to revenue loss.

### 3. Sales Trend & Forecasting
* **Goal:** Understand monthly revenue growth, seasonality, and underlying trends.
* **Methodology:** Time Series analysis, including **Month-over-Month Growth** and **Rolling 3-Month Moving Averages**, to establish a baseline for future sales forecasting models.

---

## ⚙️ Technical Stack

| Tool/Library | Purpose |
| :--- | :--- |
| **Python** | Primary programming language |
| **Pandas** | Data cleaning, wrangling, and RFM calculations |
| **NumPy** | Numerical operations and array handling |
| **Seaborn & Matplotlib** | Professional data visualization (trends, boxplots, segmentation) |
| **Jupyter/Kaggle** | Development and execution environment |

---

## 🧹 Data Cleaning Highlights

* **Handling Missing Data:** Successfully filtered and managed a large volume of missing data (initial dataset contained approximately **464k null rows**).
* **Type Conversion:** Standardized data types, converting key IDs to nullable integers (`Int64`) and categorical features (e.g., `FY`, `category_name_1`) to memory-efficient `category` dtypes.
* **Junk Removal:** Removed irrelevant or junk columns identified during initial exploration (e.g., `BI Status`, `Unnamed: X` columns).

---

## 💾 Project Files

The final, cleaned analytical dataframes are exported to the repository for direct use:

* **`Customer_RFM_Segments_201808.csv`**: The finalized customer-level table with RFM scores and segment labels.
* **`Order_Data_Cleaned_Final_2016_2018.csv`**: The clean, filtered, and feature-engineered order-level transactional data used for all analyses.

---

## 🚀 Getting Started

To run this project locally:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/h-ghulam-hasnain/pakistan-ecommerce-data-analysis.git](https://github.com/h-ghulam-hasnain/pakistan-ecommerce-data-analysis.git)
    ```
2.  **Install Dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```
3.  Open and run the main analysis notebook (e.g., `e-commerce-customer-analytics-segmentation-risk.ipynb` if you downloaded it from Kaggle) in your preferred environment (Jupyter, VS Code, etc.).
