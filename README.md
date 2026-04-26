# E-Commerce Sales Analysis

This project analyzes an e-commerce sales dataset using Python, Pandas, and Plotly. The analysis is built in a Jupyter Notebook and explores sales, profit, customer segments, product categories, and monthly performance trends.

## Project Files

- `e commerce sales.ipynb` - Main Jupyter Notebook containing the complete analysis and visualizations.
- `Sample - Superstore.csv` - Source dataset used for the analysis.

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

Make sure `Sample - Superstore.csv` stays in the same folder as the notebook, because the notebook loads it using this relative path:

```python
pd.read_csv("Sample - Superstore.csv", encoding="latin-1")
```

## Output

The notebook produces interactive Plotly charts for sales and profit trends. These visualizations help identify high-performing categories, profitable sub-categories, and customer segments with stronger business performance.
