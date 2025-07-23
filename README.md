# Blinkit Sales & Customer Analysis

# Blinkit Sales & Customer Analysis – Python Project

## Project Overview
This project performs a detailed analysis of Blinkit's sales performance, customer satisfaction, and inventory distribution using Python. By leveraging data analysis and visualization libraries such as Pandas, NumPy, Matplotlib, and Seaborn, it provides actionable insights to help stakeholders make data-driven decisions.

## Business Objective
To analyze Blinkit’s sales, product trends, outlet performance, and customer feedback to identify optimization opportunities and guide business strategy.

## Key KPIs
- **Total Sales**: Overall revenue from products sold.
- **Average Sales**: Average revenue per order.
- **Items Sold**: Total quantity of items sold.
- **Average Rating**: Mean customer rating for products.

##  Workflow Summary

### 1. Requirement Gathering
- Defined the need for comprehensive sales and customer behavior analysis.
- Identified key KPIs to measure performance.

### 2. Data Understanding
- Explored datasets covering sales, products, outlet types, locations, and customer feedback.
- Detected missing values and anomalies.

### 3. Data Import & Integration
- Loaded CSV files using `pandas`.
- Merged data using common keys (`Product ID`, `Outlet ID`, etc.).

### 4. Data Cleaning
- Handled missing values in ratings and prices.
- Removed duplicates and standardized column formats.
- Outliers were managed using IQR-based filtering.

### 5. Data Modeling
- Created a logical star schema:
  - **Fact Table**: Sales data
  - **Dimension Tables**: Product attributes, Outlet details, Feedback

### 6. Feature Engineering
- Calculated new columns such as:
  - `Total Sales = Quantity * Unit Price`
  - `Average Sales = Total Sales / Order Count`

### 7. KPI Calculation (Sample Code)
```python
df['Total_Sales'] = df['Quantity'] * df['Unit_Price']
total_sales = df['Total_Sales'].sum()
average_sales = df['Total_Sales'].mean()
items_sold = df['Quantity'].sum()
average_rating = df['Rating'].mean()
````

### 8. Visualization Highlights

* **Total Sales by Fat Content** – Donut/Bar Chart
* **Sales by Item Type** – Bar Chart
* **Sales by Outlet Size** – Pie Chart
* **Sales by Establishment Year** – Line Chart
* **Urban vs Rural Sales** – Funnel or Bar Chart
* **All Metrics by Outlet Type** – Matrix or Heatmap

### 9. Insights

* Medium-fat products led sales.
* Snacks and dairy were top-selling items.
* Large outlets generated the most revenue.
* Urban outlets outperformed rural locations.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## 📂 Project Structure
```
📦Blinkit-Analysis
 ┣ 📄blinkit_analysis.ipynb
 ┣ 📁data/
 ┃ ┣ 📄sales_data.csv
 ┃ ┣ 📄products.csv
 ┃ ┗ 📄customer_feedback.csv
 ┗ 📄README.md
```

## ▶️ How to Run This Project

1. **Clone the repository**

```bash
git clone https://github.com/your-username/blinkit-sales-analysis.git
cd blinkit-sales-analysis
```

2. **Install dependencies**

```bash
pip install pandas numpy matplotlib seaborn
```

3. **Launch the notebook**

```bash
jupyter notebook blinkit_analysis.ipynb
```

## Outcome

This project provides a complete snapshot of sales trends, customer satisfaction, and product performance. The insights can guide inventory planning, marketing efforts, and operational decisions.

## License

This project is open-source and licensed under the [MIT License](LICENSE).

## Acknowledgments

* Data inspired by Blinkit sales structure.
* Visual inspiration from Power BI implementation, adapted into Python.

---

Let me know if you'd like me to generate the actual files (`LICENSE`, example `.ipynb`, or folder structure) or if you're ready to upload this to GitHub!

```
```
