 E-Commerce Sales Data Analysis

##  Project Overview
This project focuses on analyzing e-commerce retail transaction data using Python. The goal is to explore sales trends, identify top-performing products, and understand revenue patterns through data analysis and visualization.

##  Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

##  Dataset Information
The dataset contains retail transaction records with the following columns:

- `InvoiceNo` – Invoice number for each transaction
- `StockCode` – Product code
- `Description` – Product description
- `Quantity` – Number of items purchased
- `InvoiceDate` – Date and time of the transaction
- `UnitPrice` – Price per unit
- `CustomerID` – Customer identifier
- `Country` – Customer's country

## Data Cleaning & Preparation
The following steps were performed:

- Loaded the dataset using Pandas.
- Cleaned column names.
- Removed duplicate records.
- Converted `InvoiceDate` into datetime format.
- Checked missing values.
- Created a new `Revenue` column.

##  Revenue Calculation

Revenue was calculated using Quantity multiplied by Unit Price.

```python
data['Revenue'] = data['Quantity'] * data['UnitPrice']

total_revenue = data['Revenue'].sum()

print(f"Total Revenue: {total_revenue:,.2f}")
```

**Note:** Revenue is not the same as profit. The calculation does not include business costs, and negative quantities may represent returns or cancellations.

## Data Visualization
The project includes the following visualizations:

- Monthly Revenue Trend — Line Chart
- Top Products by Revenue — Horizontal Bar Chart
- Quantity Distribution — Histogram
- Correlation Heatmap
- Additional sales and transaction visualizations

## Business Questions
This analysis explores the following questions:

1. How does revenue change over time?
2. Which products generate the highest recorded revenue?
3. Which countries contribute the most revenue?
4. What patterns can be observed in product quantities?
5. What relationships exist between quantity, unit price, and revenue?

##  Key Learnings
Through this project, I practiced:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature creation using Pandas
- Grouping and aggregating data
- Data visualization
- Interpreting business data

## Future Improvements
- Perform customer segmentation using RFM analysis.
- Analyze repeat purchases and customer behavior.
- Build an interactive Power BI dashboard.
- Develop additional business insights and recommendations.

## 👨‍💻 Author
Rehan Muzammal

Aspiring Data Analyst | Python | Pandas | NumPy | SQL | Power BI

---
This project is part of my continuous learning journey in Data Analytics.
