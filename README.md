#  E-Commerce Sales Analysis & Dashboard

##  Overview

This project presents an end-to-end analysis of real-world e-commerce transaction data, combining data cleaning, exploratory analysis, and interactive visualization.

The workflow begins with processing raw transactional data in Python and culminates in a dynamic Tableau dashboard that enables intuitive exploration of revenue trends, product performance, and pricing behavior.

---

##  Objective

* Clean and preprocess raw transactional data
* Analyze revenue trends over time
* Identify product and regional revenue concentration
* Detect pricing inefficiencies impacting profitability
* Build an interactive dashboard for business insights

---

##  Dataset

* **Source:** Online Retail Dataset (UCI / Kaggle)
* **Size:** ~500,000+ records
* Includes real-world issues such as missing values, returns, and duplicates

---

##  Data Cleaning & Feature Engineering

Performed using Python (Pandas):

* Removed missing `CustomerID` values
* Filtered negative `Quantity` values (returns/cancellations)
* Removed invalid pricing entries (`UnitPrice <= 0`)
* Eliminated duplicate records
* Converted `InvoiceDate` to datetime format
* Created **Revenue = Quantity × UnitPrice**

---

##  Exploratory Data Analysis

Key analyses performed:

*  Monthly revenue trend analysis
*  Product-level revenue concentration (Top products)
*  Country-wise revenue distribution
*  Pricing inefficiency analysis using price quartiles

---

##  Key Insights

* ~15% of total revenue comes from low-price transactions, indicating potential margin inefficiencies
* Revenue is highly concentrated among a small set of products
* A few countries contribute the majority of total revenue
* Monthly trends show variability, suggesting opportunities for demand optimization

---

##  Tableau Dashboard

An interactive dashboard was built to visualize and explore insights:

 **View Dashboard:** [\[Tableau Link\]](https://public.tableau.com/views/Book2_17757665358590/E-CommerceSalesDashboard?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

### Features:

* Interactive filters (Year, Month, Country)
* Cross-sheet filtering (Product & Country interactions)
* KPI indicator for total revenue
* Multiple visualizations:

  * Monthly revenue trend
  * Top products
  * Revenue by country
  * Pricing insight

---

##  Tech Stack

* **Python** (Data processing)
* **Pandas** (Data manipulation)
* **Matplotlib** (Visualization)
* **SQL** (Analytical queries)
* **Tableau** (Interactive dashboard)

---

##  How to Run

1. Install dependencies:

   ```bash
   pip install pandas matplotlib
   ```

2. Open the notebook:

   ```
   notebooks/analysis.ipynb
   ```

3. (Optional) Open Tableau dashboard using exported CSV

---

##  Future Improvements

* Incorporate cost/profit data for accurate margin analysis
* Perform RFM-based customer segmentation
* Build predictive models for demand forecasting
* Enhance dashboard with additional KPIs

---

##  Conclusion

This project demonstrates a complete data analysis pipeline — from cleaning and structuring raw data to deriving actionable business insights and presenting them through an interactive dashboard.

It highlights how data-driven approaches can support better pricing strategies, product focus, and regional decision-making.

---
