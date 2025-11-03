# Zepto_data_analysis
A complete SQL data analysis project using Zepto’s e-commerce inventory dataset. Covers data cleaning, exploration, and business insights like best-value products, revenue by category, and stock analysis. Perfect for data analyst portfolios and SQL practice in retail analytics.

Project Overview

This project is a complete, real-world data analytics portfolio case study based on an **e-commerce inventory dataset** scraped from **Zepto**, one of India’s fastest-growing quick-commerce startups. The analysis simulates the end-to-end workflow of a professional data analyst — starting from raw data exploration and cleaning, to deriving actionable business insights using SQL.

The main goal is to understand **product performance, pricing strategy, discount patterns, and inventory health** in an online retail environment.

Objectives

1. Explore and clean raw inventory data for quality and consistency.
2. Identify high-performing product categories and best-value products.
3. Detect stock shortages and revenue potential by category.
4. Analyze discounts, pricing, and product weights to evaluate value per gram.
5. Deliver insights useful for inventory management and marketing strategy.


Tools Used

* PostgreSQL / MySQL / SQL Server (any supported SQL engine)
* VS Code / pgAdmin / DBeaver for SQL query execution and visualization

Database Design

Table Name: zepto
Columns:

* sku_id – unique product identifier
* category – product category
* name – product name
* mrp – maximum retail price (₹)
* discountPercent – discount applied (%)
* availableQuantity – number of units in stock
* discountedSellingPrice – final selling price after discount (₹)
* weightInGms – product weight in grams
* outOfStock – boolean indicating stock status
* quantity – available item count

Workflow and Analysis

1. Data Exploration

* Checked total number of rows and sample records.
* Verified missing (NULL) values across columns.
* Identified distinct product categories.
* Compared **in-stock vs out-of-stock** items.
* Detected duplicate product names and SKUs.

2. Data Cleaning

* Removed invalid products where price or selling price was **zero**.
* Converted price units from **paise to rupees** for consistency.
* Verified data accuracy after transformation.

### 3. Business Analysis (Key SQL Queries)

* **Top 10 Best-Value Products:** Sorted by highest discount percentage.
* **High-MRP Products Out of Stock:** Found premium items frequently unavailable.
* **Estimated Revenue by Category:** Calculated total potential revenue using `discountedSellingPrice * availableQuantity`.
* **High-Value but Low-Discount Products:** Identified high-MRP, low-discount items for potential premium positioning.
* **Top 5 Categories by Average Discount:** Found most competitive product categories.
* **Price per Gram Analysis:** Determined cost-efficiency of products above 100g.
* **Weight-Based Categorization:** Grouped products into “Low,” “Medium,” and “Bulk” based on weight.
* **Total Inventory Weight per Category:** Measured total weight in stock per category for logistics optimization.


Key Insights

* Certain product categories contribute disproportionately to revenue — showing potential for targeted restocking.
* Several **high-MRP products were consistently out of stock**, signaling supply-chain or demand forecasting issues.
* Categories with **high average discounts** attract customers but lower profit margins, indicating need for balanced pricing.
* “Bulk” items dominate total inventory weight, while “Low” weight items drive higher sales volume.
* The best-value products (by discount%) can be used for promotional campaigns to attract price-sensitive customers.


Learning Outcomes

* Hands-on experience in **data exploration, cleaning, and analysis using SQL**.
* Practical understanding of how SQL queries drive **business insights** in retail and e-commerce.
* Ability to communicate data findings in a professional format, making it an excellent addition to a **Data Analyst portfolio**.

Ideal For

*  Data Analyst aspirants building a **portfolio-ready SQL project**.
*  Learners practicing **SQL queries on real-world e-commerce datasets**.
*  Professionals preparing for interviews in **retail, e-commerce, and product analytics** roles.

