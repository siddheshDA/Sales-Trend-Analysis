# Sales Trend Analysis - Task 6

## 📌 Objective
Analyze monthly revenue and order volume from the `online_sales_sample` dataset using SQL aggregations in PostgreSQL.

## 🛠 Tools Used
- PostgreSQL
- pgAdmin 4

## 📂 Dataset
`online_sales_sample.csv` — contains order details such as:
- `order_date`
- `order_id`
- `amount`
- `product_id`
- `year` & `month` (present in CSV but not used directly — derived from `order_date`)

## 📊 Queries Performed
1. **Monthly Revenue & Volume**  
   - Extracted year and month from `order_date` using `EXTRACT()`.  
   - Grouped data by year and month.  
   - Calculated monthly revenue using `SUM(amount)`.  
   - Calculated order volume using `COUNT(DISTINCT order_id)`.  
   - Ordered results chronologically.

2. **Filter for a Specific Year**  
   - Applied `WHERE` condition to analyze only 2023 data.  
   - Sorted months by highest revenue.  

3. **Top 3 Months by Revenue**  
   - Grouped by year and month.  
   - Calculated total revenue per month.  
   - Sorted in descending order and limited results to top 3 months.

## 📈 Insights
- Identified month-wise sales performance.
- Pinpointed peak months by revenue.
- Learned use of aggregate functions, grouping, filtering, and ordering.

## 🚀 How to Run
1. Import `online_sales_sample.csv` into PostgreSQL.
2. Open `task6_sales_trend.sql` in pgAdmin or `psql`.
3. Run the queries sequentially.
4. View results to analyze sales trends.

## 📄 Deliverables
- `online_sales_sample.csv` (Dataset)
- `task6_sales_trend.sql` (All SQL queries)
- Output screenshots
- This README
