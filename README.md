# coffee-shop-sales-dashboard
 Coffee Shop Sales Analysis and Dashboard using MySQL and Power BI 

---

## 📌 Project Objective
To analyze and visualize coffee shop sales data using **MySQL** for data preparation and **Power BI** for creating an interactive dashboard that helps identify product trends, store performance, and customer behavior across time.

---
## 📁 Dataset Used
[Dataset Link](https://www.kaggle.com/datasets/ahmedmohamedibrahim1/coffee-shop-sales-dataset)

---

## ❓ Key Questions Answered
- What are the total sales, order volume, and quantity sold?
- Which product categories and types are most popular?
- What time of day drives the most sales?
- Which store locations perform best?
- How do weekdays compare with weekends in terms of sales?

---

## ⚙️ Process Overview

### 🔸 Data Preparation in MySQL
- Used `STR_TO_DATE()` to clean and convert date/time columns.
- Created new columns for:
  - **Hour** extracted from `transaction_time`
  - **Day name** and **Day type** (weekday/weekend) derived from `transaction_date`
- Renamed columns with inconsistent encodings using `ALTER TABLE`.
- Created SQL queries and views to calculate:
  - Total sales and quantity
  - Sales by category, location, and time
  - Most sold products and their quantities

### 🔸 Dashboard Design in Power BI
- Imported data and views from MySQL into Power BI.
- Used `CALENDARAUTO()` DAX to generate a date table.
- Built interactive visuals:
  - **KPI cards** for total sales, orders, and quantity
  - **Clustered bar charts** for product categories, product types, locations, and hours
  - **Pie and donut charts** for best-selling products and store distribution
- Implemented **tooltips** in:
  - Calendar chart (to show sales by date)
  - Day & hour chart (to show peak hour details interactively)

---

## 📈 Key Insights

- 📦 **Coffee, Tea, and Bakery** are the **top 3 most sold product categories**.
- 📊 **5 of the top 10 most sold product types** are:
  - **Barista Expresso**
  - **Brewed Chai Tea**
  - **Gourmet Brewed Coffee**
  - **Hot Chocolate**
  - **Brewed Black Tea**
- 🕗 Most sales happen between **8 AM and 10 AM**, aligning with peak coffee hours.
- 🏪 **Downtown and Central** locations consistently generate the highest revenue.
- 📅 **Weekends** outperform weekdays in terms of total sales and quantity.
- 🧠 Tooltip-based visuals enhance analysis of **daily and hourly patterns**.

---

## 🧰 Tools Used
- **MySQL** – Data cleaning, transformation, and aggregation
- **Power BI** – Dashboard creation, slicers, tooltips, and custom visuals
- **DAX** – Used minimally for the `CALENDARAUTO()` function and created multiple measures 

---

## ✅ Conclusion
This dashboard helps stakeholders of a coffee shop chain gain deep insights into their sales patterns, top products, store performance, and customer buying behavior — ultimately supporting smarter marketing, staffing, and inventory decisions.

![dashboard_image](https://github.com/user-attachments/assets/fb8ece37-2808-461c-ab6f-ec90607652d7)


