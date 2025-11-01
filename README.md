# 🍕 Pizza Sales Data Analysis (SQL + Power BI)

## 📖 Project Overview
This project analyzes pizza sales data to uncover key insights and improve business performance using **SQL** and **Power BI**.  
The goal is to calculate essential **KPIs**, visualize sales trends, and identify best and worst-performing pizzas.

---

## 🎯 Problem Statement
To analyze pizza sales data and gain insights into business performance by calculating the following key indicators:
1. **Total Revenue:** Total price of all pizza orders.  
2. **Average Order Value:** Average spend per order.  
3. **Total Pizzas Sold:** Total number of pizzas sold.  
4. **Total Orders:** Number of unique orders placed.  
5. **Average Pizzas per Order:** Average pizzas sold per order.

---

## 🧮 Tools & Technologies
- **SQL Server** – Data extraction, transformation, and KPI calculations  
- **Power BI** – Dashboard visualization and data storytelling  
- **Excel** – Used for data cleaning and formatting  

---

## 🧠 Key Insights
- Orders are **highest on weekends** — especially **Friday and Saturday evenings**.  
- Maximum orders occur during the months of **July** and **January**.  
- **Classic Category** and **Large Size pizzas** contribute most to total sales.  
- **Thai Chicken Pizza** generates the **maximum revenue**, while **Brie Carre Pizza** shows the **lowest performance**.

---

## 📊 Dashboard Features
### **KPI Cards**
- Total Revenue  
- Average Order Value  
- Total Pizzas Sold  
- Total Orders  
- Average Pizzas per Order  

### **Visualizations**
- **Daily & Monthly Trends** for total orders  
- **Sales Distribution** by pizza category and size  
- **Funnel Chart:** Total pizzas sold by category  
- **Top & Bottom 5 Pizzas** by revenue, quantity, and orders  

---

## 🧾 SQL Queries (Sample)
```sql
-- Total Revenue
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;

-- Average Order Value
SELECT (SUM(total_price) / COUNT(DISTINCT order_id)) AS Avg_Order_Value FROM pizza_sales;

-- Top 5 Pizzas by Revenue
SELECT TOP 5 pizza_name, SUM(total_price) AS Total_Revenue
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Revenue DESC;

📈 Project Structure
Pizza-Sales-Analysis/
│
├── Pizza_Sales_Queries_Of_SQL.docx
├── Pizza_Sales_Dashboard.pbix
├── Dashboard_Screenshots/
├── Screen Recording 2025-11-01 163135.mp4
└── README.md

🚀 Results

✅ Delivered a fully interactive dashboard providing business insights such as:

Top-performing pizza categories and sizes

Peak sales days and months

Customer purchasing trends

Data-driven decisions for product improvement

🧩 Future Enhancements

Automate data refresh using Power BI Gateway

Integrate live database connections

Add DAX-based advanced KPIs for customer segmentation

👨‍💻 Author

Yash Sonwane
🔗 GitHub Profile(https://github.com/YashSonwane11)

💼 LinkedIn Profile(www.linkedin.com/in/yash-sonwane-88a92923a)

🏷️ Tags

#PowerBI #SQL #DataAnalytics #BusinessIntelligence #Dashboard #DataVisualization #PortfolioProject


---

Would you like me to make this **README automatically downloadable** as a `.md` file so you can just drag and drop it into your repo?
