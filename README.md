### 📌 Project Overview

The **E-commerce Sales Dashboard** project analyzes sales data from an online store to identify trends, top customers, outliers, and business insights.
It uses **Python (Pandas, Matplotlib, Seaborn)** to clean the dataset, perform exploratory data analysis (EDA), and visualize key metrics.

This analysis helps answer questions such as:

* Which months bring the highest sales?
* Which product lines generate the most revenue?
* What percentage of sales comes from returning vs new customers?
* How quickly are orders shipped?
* Who are the top customers by sales volume?

---

### 🛠 **Technologies & Libraries**

* **Python 3.x**
* **Pandas** – data manipulation and aggregation
* **NumPy** – numerical calculations
* **Matplotlib & Seaborn** – data visualization
* **Jupyter Notebook** – interactive analysis

---

### 📂 **Dataset**

The dataset contains sales order information with columns such as:

* `ORDERNUMBER` – unique order ID
* `SALES` – total sale value for the order
* `ORDERDATE` – date of order placement
* `PRODUCTLINE` – category of product sold
* `QTR_ID` – quarter of the year
* `MONTH_ID` – month of the year
* `CONTACTFIRSTNAME`, `CONTACTLASTNAME` – customer details
* `COUNTRY`, `STATE`, `CITY`, `POSTALCODE` – location details

---

### 🔍 **Key Steps in Analysis**

1. **Data Cleaning**

   * Removed rows with missing `POSTALCODE` values.
   * Checked and removed duplicate records.
   * Converted date columns to proper `datetime` format.

2. **Outlier Detection**

   * Used **boxplots** and the **IQR method** to identify high-value orders.
   * Labeled customers responsible for outlier sales.

3. **Customer Segmentation**

   * Created a `CUSTOMERNAME` column.
   * Classified customers into:

     * **Returning customers** (more than 1 order)
     * **New customers** (only 1 order)

4. **Sales Analysis**

   * Calculated total sales from returning vs new customers.
   * Found top-selling product categories.
   * Analyzed monthly and quarterly sales trends.

5. **Visualizations**

   * **Bar plots** for top 10 customers by sales.
   * **Pie chart** for sales distribution between returning and new customers.
   * **Line plots** for monthly trends.
   * **Boxplots** for outlier detection in sales.

---

### 📊 **Example Insights**

* Returning customers generated \~80% of total sales.
* The "Classic Cars" product line contributed the highest revenue.
* Q4 showed the highest average monthly sales.
* Only a small percentage of orders were extreme outliers, but they represented significant revenue.

---

### 📷 **Sample Visualizations**

* **Top 10 Customers by Sales**
* **Sales Distribution: Returning vs New Customers (Pie Chart)**
* **Monthly Sales Trend (Line Plot)**
* **Sales Outliers by Customer (Boxplot)**

---

### 🚀 **How to Run**

1. Clone the repository:

   ```bash
   git clone https://github.com/waniamasood/ecommerce-sales-dashboard.git
   ```
2. Install dependencies:

   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
4. Run the notebook cells in order to reproduce the analysis.

---

### 📌 **Future Improvements**

* Create an **interactive dashboard** using Plotly or Power BI.
* Predict future sales using machine learning.
* Add regional maps for geographic sales visualization.

