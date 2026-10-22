## E-Commerce Sales Analytics

## 1. Project Overview

The **E-Commerce Sales Analytics** project focuses on analysing e-commerce sales data to identify sales trends, evaluate product and regional performance, understand customer ratings, and generate actionable business insights.

The project uses Python for data cleaning, exploratory data analysis (EDA), and visualisation, along with Microsoft Power BI to develop an interactive dashboard. The findings support data-driven decision-making by highlighting revenue patterns, profitability, and opportunities for business improvement.

## 2. Problem Statement

E-commerce businesses generate large amounts of transactional data, but raw data alone does not provide sufficient information for effective decision-making.

The objective of this project is to transform raw sales data into meaningful insights by addressing the following questions:

- Which product categories and individual products generate the highest sales?
- Which regions contribute the most to sales and profit?
- What patterns exist in sales, profit, discounts, and customer ratings?
- How can data quality issues affect the reliability of business analysis?
- What strategies can improve profitability and overall business performance?

## 3. Dataset Description

The project uses the `ecommerce_sales_week4.csv` dataset, containing 107 records and 11 columns before data cleaning.

| Column | Description |
|---|---|
| `Order_ID` | Unique identifier for an order |
| `Product` | Name of the product sold |
| `Category` | Product category |
| `Region` | Geographical sales region |
| `Quantity` | Number of units sold |
| `Unit_Price` | Price per unit |
| `Sales` | Recorded sales amount |
| `Profit` | Profit generated from the transaction |
| `Discount_Percent` | Discount percentage applied |
| `Customer_Age` | Customer age |
| `Customer_Rating` | Customer rating for the purchase or experience |

The dataset contains numerical and categorical variables, making it suitable for descriptive statistics, comparative analysis, correlation analysis, and visualisation.

**Data source:** `ecommerce_sales_week4.csv`, provided for the project assignment.

## 4. Tools and Technologies Used

- **Python:** Data analysis and processing.
- **Pandas:** Data manipulation and cleaning.
- **NumPy:** Numerical operations.
- **Matplotlib:** Data visualisation.
- **Seaborn:** Statistical visualisation, where applicable.
- **Jupyter Notebook:** Interactive analysis and documentation.
- **Microsoft Power BI:** Interactive dashboard development.
- **Git and GitHub:** Version control and project repository management.

## 5. Data Cleaning Process

Data cleaning was performed to improve the consistency and reliability of the dataset before analysis.

The main steps included:

1. **Data inspection:** Examined the dataset structure, column names, data types, and summary statistics.
2. **Missing-value detection:** Identified missing values in `Quantity`, `Sales`, and `Customer_Rating`.
3. **Missing-value treatment:** Used median imputation for missing `Quantity` and `Customer_Rating` values. Missing `Sales` was calculated using `Quantity × Unit_Price`, where appropriate.
4. **Duplicate removal:** Identified and removed one duplicate record.
5. **Data validation:** Examined numerical values and potential anomalies, including negative unit prices and implausible customer ages, for further verification.
6. **Cleaned dataset export:** Saved the processed dataset as `ecommerce_sales_cleaned.csv`.

After removing the duplicate record, the cleaned dataset contained 106 records.

**Note:** Potential anomalies should be validated against the original data source before being corrected or excluded.

## 6. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was conducted to understand the dataset's characteristics and uncover patterns relevant to business performance.

The analysis included:

- Reviewing descriptive statistics and frequency distributions.
- Examining sales and profit across product categories.
- Comparing regional sales and profitability.
- Identifying leading products by sales and profit.
- Analysing the distribution of sales and customer ratings.
- Investigating the relationship between sales and profit.
- Examining discount-related patterns and potential outliers.

EDA provided the foundation for selecting meaningful visualisations and identifying areas requiring further business investigation.

## 7. Data Visualisations

The project includes the following charts:

| Visualisation | Purpose |
|---|---|
| Sales by Category | Compares sales contributions across product categories |
| Profit by Region | Evaluates regional profitability |
| Distribution of Sales | Examines the spread and concentration of transaction values |
| Discount Percentage vs. Sales | Investigates the relationship between discounts and sales |
| Distribution of Customer Ratings | Understands customer-rating patterns |
| Profit by Product | Identifies products contributing most to profit |

The chart images are included in the repository as PNG files. These visualisations make patterns, differences, and potential anomalies easier to interpret.

## 8. Power BI Dashboard

An interactive dashboard was developed in Microsoft Power BI to present key business performance indicators and enable users to explore the dataset.

### Key Performance Indicators (KPIs)

- **Total Sales:** Sum of recorded sales.
- **Total Profit:** Sum of recorded profit.
- **Average Customer Rating:** Mean customer rating.

### Dashboard Visuals

The dashboard contains:

- Sales by Category
- Profit by Region
- Sales by Product
- Order Count by Customer Rating

### Interactive Filters

The dashboard includes slicers for:

- Region
- Category
- Product

These filters allow users to examine selected business segments and compare performance interactively.

**Dashboard file:** `Ecommerce_sales_dashboard.pbix`

**Template file:** `Ecommerce_sales_dashboard.pbit`

The Power BI report can be opened using Microsoft Power BI Desktop.

## 9. Key Insights

The analysis of the cleaned dataset produced the following findings:

- **Total sales:** 157,971.00
- **Total profit:** 17,247.05
- **Average customer rating:** Approximately 4.37 out of 5
- **Leading category:** Electronics, with sales of 143,928.00
- **Leading region by sales:** North, with sales of 117,753.00
- **Leading region by profit:** North, with profit of 8,957.90
- **Leading product by sales:** Laptop, with sales of 110,790.00
- **Sales-profit correlation:** Approximately 0.988, indicating a strong positive linear relationship in the analysed data.

### Interpretation

Electronics accounts for the largest share of recorded sales, while the North region leads in both sales and profit. Laptop sales make a particularly large contribution to overall revenue.

The strong positive correlation between sales and profit indicates that higher sales values tend to be associated with higher profit values in this dataset. However, correlation does not establish causation.

The dataset also contains an unusually large laptop transaction, which may substantially influence aggregate results. Therefore, the findings should be interpreted alongside transaction-level analysis and data-quality checks.

## 10. Business Recommendations

Based on the analysis, the following recommendations are proposed:

1. **Strengthen high-performing product categories:** Review demand, margins, and stock availability for Electronics while avoiding excessive dependence on a single category.
2. **Optimise regional strategies:** Investigate the factors behind the North region's performance and assess whether successful approaches can be adapted to other regions.
3. **Evaluate product profitability:** Consider both sales volume and profit margin when making pricing, inventory, and promotional decisions.
4. **Assess discount effectiveness:** Measure the impact of discounts on sales volume and profit before expanding promotional campaigns.
5. **Improve customer experience:** Monitor customer ratings alongside complaints, returns, and service feedback to identify opportunities for improvement.
6. **Validate unusual transactions:** Investigate unusually large sales, negative unit prices, and implausible customer ages before using the data for operational decisions.
7. **Monitor KPIs regularly:** Use the Power BI dashboard to track sales, profit, customer ratings, and regional performance over time.

These recommendations should be tested against more detailed transaction records and additional time periods before implementation.

## 11. Conclusion

The E-Commerce Sales Analytics project demonstrates how data analysis and visualisation can transform raw transactional data into actionable business information.

Python and its data-analysis libraries were used to clean, explore, and visualise the dataset, while Power BI provided an interactive dashboard for monitoring key performance indicators and comparing business segments.

The analysis identified Electronics as the leading sales category, the North region as the strongest regional contributor, and Laptops as the leading product by sales. It also highlighted the importance of validating outliers and questionable values before drawing conclusions.

Overall, the project demonstrates the practical application of data cleaning, exploratory data analysis, visualisation, dashboard development, and business interpretation in an e-commerce context.

## 12. Repository Structure

```text
Ecommerce-Sales-Analytics/
│
├── ecommerce_sales_week4.csv
├── ecommerce_sales_cleaned.csv
├── task2_analysis.ipynb
├── task3_data_prep.ipynb
├── task4_EDA.ipynb
├── task5_visualization.ipynb
│
├── chart1_sales_by_category.png
├── chart2_profit_by_region.png
├── chart3_dist_sales.png
├── chart4_discount%_vs_sales.png
├── chart5_dist_customer_rating.png
├── chart6_profit_by_product.png
│
├── Ecommerce_sales_dashboard.pbix
├── Ecommerce_sales_dashboard.pbit
├── E-commerce sales analytics.pptx
├── README.md
└── .gitignore
```

## 13. How to Use the Project

1. Clone or download the repository from GitHub.
2. Install Python and the required libraries.
3. Open the Jupyter notebooks in Jupyter Notebook or VS Code.
4. Run the notebooks in sequence, ensuring that the dataset paths match the local project directory.
5. Open `Ecommerce_sales_dashboard.pbix` using Microsoft Power BI Desktop to explore the dashboard.

Install the main Python libraries using:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## 14. Project Deliverables

- Original and cleaned datasets
- Jupyter notebooks for analysis and visualisation
- Exported chart images
- Interactive Power BI dashboard and template
- Project presentation
- GitHub repository documentation

---

**Project:** E-Commerce Sales Analytics  
**Domain:** Data Analytics and Business Intelligence  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook, Power BI, Git and GitHub
