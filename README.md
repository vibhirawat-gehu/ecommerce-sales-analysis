# E-Commerce Sales Analysis

This project analyzes an e-commerce sales dataset using Python, Pandas, Plotly, and Power BI. The analysis is built in a Jupyter Notebook and supported by an interactive sales dashboard that explores sales, profit, customer segments, product categories, and monthly performance trends.

## Project Files

- `e commerce sales.ipynb` - Main Jupyter Notebook containing the complete analysis and visualizations.
- `Sample - Superstore.csv` - Source dataset used for the analysis.
- `Sales Dashboard.pbix` - Power BI dashboard file for interactive sales and profit reporting.

## Dataset Overview

The dataset contains order-level sales records from the Sample Superstore dataset.

- Total rows: `9,994`
- Total columns: `21`
- Unique orders: `5,009`
- Date range: `2014-01-03` to `2017-12-30`
- Total sales: `$2,297,200.86`
- Total profit: `$286,397.02`

Main fields include:

- Order details: `Order ID`, `Order Date`, `Ship Date`, `Ship Mode`
- Customer details: `Customer ID`, `Customer Name`, `Segment`
- Location details: `Country`, `City`, `State`, `Region`, `Postal Code`
- Product details: `Product ID`, `Category`, `Sub-Category`, `Product Name`
- Business metrics: `Sales`, `Quantity`, `Discount`, `Profit`

## Analysis Performed

The notebook covers:

- Loading and previewing the dataset
- Descriptive statistics of numeric columns
- Converting order and shipping dates to datetime format
- Creating date-based columns:
  - `Order Month`
  - `Order Year`
  - `Order Day of Week`
- Monthly sales trend analysis
- Sales analysis by category and sub-category
- Monthly profit trend analysis
- Profit analysis by category and sub-category
- Sales and profit comparison by customer segment
- Sales-to-profit ratio analysis by customer segment

The Power BI dashboard provides an interactive view of key sales metrics, profit performance, product category insights, and business trends from the same dataset.

## Key Insights

- Technology is the highest-performing category by both sales and profit.
- Top sub-categories by sales are Phones, Chairs, and Storage.
- Top sub-categories by profit are Copiers, Phones, and Accessories.
- The project compares sales and profit across customer segments: Consumer, Corporate, and Home Office.

## Tools and Libraries

- Python
- Jupyter Notebook
- Pandas
- Plotly Express
- Plotly Graph Objects
- Microsoft Power BI Desktop

## How to Run

1. Clone or download this project.
2. Install the required Python libraries:

   ```bash
   pip install pandas plotly notebook
   ```

3. Open the notebook:

   ```bash
   jupyter notebook "e commerce sales.ipynb"
   ```

4. Run the cells from top to bottom.

To view the dashboard, open `Sales Dashboard.pbix` in Microsoft Power BI Desktop.

Make sure `Sample - Superstore.csv` stays in the same folder as the notebook, because the notebook loads it using this relative path:

```python
pd.read_csv("Sample - Superstore.csv", encoding="latin-1")
```

## Output

The notebook produces interactive Plotly charts for sales and profit trends. The Power BI dashboard adds a dedicated reporting view for exploring overall sales performance, profit trends, category-level performance, and customer segment insights.
