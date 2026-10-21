# **E-Commerce Sales Analytics**



###### 1\. Project Overview

&#x09;This project analyzes e-commerce sales data using Python, Pandas, Matplotlib, and Power BI. It explores sales performance, profitability, customer ratings, regional differences, and product-category trends.



###### 2\. Problem Statement

&#x09;Businesses need to understand which products and categories generate the most revenue, which regions perform well, and how sales relate to profit and customer satisfaction. This project uses data analysis and visualization to identify patterns and support informed business decisions.



###### 3\. Dataset Description

&#x09;The dataset contains e-commerce order information, including:

&#x09;	- Order ID

&#x09;	- Product and category

&#x09;	- Region

&#x09;	- Quantity and unit price

&#x09;	- Sales and profit

&#x09;	- Discount percentage

&#x09;	- Customer age

&#x09;	- Customer rating



&#x09;The original dataset contains 107 records and 11 columns. A cleaned version was prepared for analysis.



###### 4\. Tools and Technologies

&#x09;- Python: Data analysis and processing

&#x09;- Pandas: Data inspection and cleaning

&#x09;- Matplotlib: Data visualization

&#x09;- Jupyter Notebook: Interactive analysis

&#x09;- Power BI Desktop: Interactive dashboard

&#x09;- Git and GitHub: Version control and project hosting



###### 5\. Data Cleaning Process

&#x09;The dataset was inspected for missing values and duplicate records. Missing quantity and customer-rating values were filled using the respective medians. Missing sales were calculated using quantity multiplied by unit price. Duplicate records were removed, and the cleaned dataset was saved as `ecommerce\_sales\_cleaned.csv`.



&#x09;Potentially invalid values, including a negative unit price and an implausible customer age, were also identified for validation.



###### 6\. Exploratory Data Analysis

&#x09;The analysis included:

&#x09;	- Descriptive statistics

&#x09;	- Data type and missing-value inspection

&#x09;	- Duplicate detection

&#x09;	- Correlation analysis

&#x09;	- Outlier detection using the Interquartile Range method

&#x09;	- Sales and profit comparisons by category, region, and product

&#x09;	- Customer-rating analysis



###### 7\. Data Visualizations

&#x09;Six visualizations were created:

&#x09;	1. Total Sales by Product Category

&#x09;	2. Total Profit by Region

&#x09;	3. Distribution of Sales

&#x09;	4. Discount Percentage vs Sales

&#x09;	5. Distribution of Customer Ratings

&#x09;	6. Total Profit by Product



&#x09;The chart images are included in the repository.



8\. Power BI Dashboard

&#x09;The interactive dashboard includes:

&#x09;	- Total Sales KPI card

&#x09;	- Total Profit KPI card

&#x09;	- Average Customer Rating KPI card

&#x09;	- Sales by Category

&#x09;	- Profit by Region

&#x09;	- Sales by Product

&#x09;	- Order Count by Customer Rating

&#x09;	- Region, Category, and Product slicers



&#x09;The dashboard allows users to filter and explore business metrics across different segments.



9\. Key Business Insights

&#x09;- Electronics is the largest revenue-generating category.

&#x09;- The North region records the highest sales and profit in the dataset.

&#x09;- Laptops generate the highest recorded sales and profit among products, influenced by an unusually large transaction.

&#x09;- The average customer rating is approximately 4.37 out of 5.

&#x09;- Sales and profit have a strong positive correlation.

&#x09;- Outliers and invalid values require verification before business decisions are made.



10\. Business Recommendations

&#x09;1. Study the sales and profitability drivers of Electronics and the North region to identify practices that may benefit weaker-performing segments.

&#x09;2. Investigate unusually large transactions and implement validation checks for negative prices, implausible customer ages, and unusual order quantities.

&#x09;3. Evaluate discounts using both sales and profit metrics before changing pricing strategies.



11\. Project Structure

&#x09;- `README.md` — Project documentation

&#x09;- `.gitignore`

&#x09;- `ecommerce\_sales\_week4.csv` — Original dataset

&#x09;- `ecommerce\_sales\_cleaned.csv` — Cleaned dataset

&#x09;- `task3\_data\_prep.ipynb` — Data preparation

&#x09;- `task4\_EDA.ipynb` — Exploratory data analysis

&#x09;- `task5\_visualization.ipynb` — Data visualizations

&#x09;- `chart1\_sales\_by\_category.png` to `chart6\_profit\_by\_product.png` — Chart images

&#x09;- `Ecommerce\_Sales\_Dashboard.pbix` — Power BI dashboard



12\. Conclusion

&#x09;This project demonstrates a complete data analytics workflow, from dataset preparation and exploratory analysis to visualization, dashboard development, and business recommendations. The results provide a foundation for understanding e-commerce performance and identifying areas for further investigation.





