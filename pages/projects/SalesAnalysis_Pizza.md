---
layout: default
title: "📊 Analytics & Revenue Insights for Pizza Sales using Tableau 🍕💡"
---

[Live Interactive Dashboard](https://public.tableau.com/app/profile/tarun.mishra7740/viz/PizzaSalesDashboard_17070774157650/Home)

![App Screenshot](https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/448b794e-dea6-41ae-bcfa-72ec64c56b17)

![App Screenshot](https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/8e8c76a2-164b-483e-b5b8-c30649272ac9)

## **Problem Statement**:

In this project, I aim to leverage the data from a pizza outlet's sales records to gain valuable insights and present them through an interactive dashboard created using Tableau. The dataset encompasses various features that provide a comprehensive view of the pizza sales dynamics.

The dataset contains the following features:

##### 1. **pizza_id** 🍕: Unique identifier for each pizza.

##### 2. **order_id** 📋: Unique identifier for each order.

##### 3. **pizza_name_id** 🍽️: Identifier for each pizza name.

##### 4. **quantity** 📦: The number of pizzas ordered in a specific transaction.

##### 5. **order_date** 📅: Date when the order was placed.

##### 6. **order_time** ⌚: Time when the order was placed.

##### 7. **unit_price** 💰: Price per unit pizza.

##### 8. **total_price** 💵: Total price for the quantity ordered.

##### 9. **pizza_size** 📏: Size of the pizza.

##### 10. **pizza_category** 🍽️: Category of the pizza.

##### 11. **pizza_ingredients** 🥦: List of ingredients in the pizza.

##### 12. **pizza_name** 🏷️: Name of the pizza.





## **Understanding Client Requirements and Practical Significance 🤝📊**

In this section, I bridge the gap between client aspirations and tangible operational insights. By dissecting each requirement laid out by the client and elucidating its practical significance, we aim to provide a comprehensive understanding that goes beyond meeting expectations. 


### KPIs Requirement:

#### 1. Total Revenue 💰:

The sum of the total price of all pizza orders.

*Practical Significance:* Helps the outlet owner understand the overall financial performance of the business. Enables tracking of revenue growth and identifying peak periods for strategic planning, such as promotions or inventory management.

#### 2. Average Order Value 💳:

The average amount spent per order, calculated by dividing the total

*Practical Significance:* Provides insights into customer spending behavior. A higher average order value may indicate successful upselling strategies or the popularity of premium pizza options.

#### 3. Total Pizzas Sold 🍕:

The sum of the quantities of all pizzas sold.

*Practical Significance:* Indicates the overall demand for pizzas. Helps in inventory management, ensuring popular pizzas are well-stocked, and identifying opportunities for introducing new varieties.

#### 4. Total Orders 📦:

The total number of orders placed.

*Practical Significance:* Offers a clear picture of customer transaction volume. Enables the outlet owner to assess staffing needs during peak hours, improving operational efficiency.

#### 5. Average Pizzas Per Order 📊:

The average number of pizzas sold per order, calculated by dividing the total number of pizzas sold by the total number of orders.

*Practical Significance:* Highlights customer ordering habits. Valuable for tailoring promotional strategies or creating bundled offers to encourage higher quantities per order.

---

### Charts Requirement:

#### 1. Hourly Trend for Total Pizzas Sold 🕒🍕:

Created a stacked bar chart that displays the hourly trend of total orders over a specific time period. This chart will help us identify any patterns or fluctuations in order volumes on a hourly basis.

*Practical Significance:* Allows the outlet owner to identify peak hours of demand, optimizing staff schedules and resource allocation for efficient service during busy periods.

#### 2. Weekly Trend for Total Orders 📅📊:

Created a line chart that illustrates the weekly trend of total orders throughout the year. This chart will allow us to identify peak weeks or periods of high order activity.

*Practical Significance:* Aids in long-term planning by identifying recurring patterns. Enables the owner to anticipate high-demand weeks and prepare accordingly, optimizing inventory and staff levels.

#### 3. Percentage of Sales by Pizza Category 🍕📈:

Created a pie chart that shows the distribution of sales across different pizza categories. This chart will provide insights into the popularity of various pizza categories and their contribution to overall sales.

*Practical Significance:* Guides menu optimization by showcasing popular pizza categories. Helps the owner focus on marketing or refining less popular categories for better profitability.

#### 4. Percentage of Sales by Pizza Size 🍕📊:

Generated a pie chart that represents the percentage of sales attributed to different pizza sizes. This chart will help us understand customer preferences for pizza sizes and their impact on sales.

*Practical Significance:* Informs inventory decisions by highlighting preferred pizza sizes. Useful for adjusting stock levels and pricing strategies to align with customer preferences.

#### 5. Total Pizzas Sold by Pizza Category 🍕📉:

Created a funnel chart that presents the total number of pizzas sold for each pizza category. This chart will allow us to compare the sales performance of different pizza categories.

*Practical Significance:* Identifies top-performing pizza categories, aiding in menu refinement. Enables the outlet owner to focus on promoting and improving the offerings within high-demand categories.

#### 6. Top 5 Best Sellers by Revenue, Total Quantity, and Total Orders 💰🔝:

Created a bar chart highlighting the top 5 best-selling pizzas based on the Revenue, Total Quantity, Total Orders. This chart will help us identify the most popular pizza options.

*Practical Significance:* Essential for strategic menu planning. Helps the owner understand customer favorites and adjust marketing efforts, pricing, or promotions for maximum impact.

#### 7. Bottom 5 Best Sellers by Revenue, Total Quantity, and Total Orders 💰📉:

Created a bar chart showcasing the bottom 5 worst-selling pizzas based on the Revenue, Total Quantity, Total Orders. This chart will enable us to identify underperforming or less popular pizza options.

*Practical Significance:* Indicates underperforming items. Enables the outlet owner to assess whether marketing efforts, pricing adjustments, or menu changes are needed to boost sales or phase out less popular options.


## **SQL Queries for Data Validation 🛠️🔍**

To ensure the accuracy and reliability of the data presented in the dashboard, SQL queries play a pivotal role in validating the underlying dataset. However, it's important to note that SQL queries are not inherently dynamic and might require manual entry for varied results. Below are some essential SQL queries tailored for data validation:

### A. KPI’s

#### 1. Total Revenue:
```
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;
```

<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/134bf323-38e7-4b43-bdf8-bc94da2bd1ac" width="150">


#### 2. Average Order Value
```
SELECT (SUM(total_price) / COUNT(DISTINCT order_id)) AS Avg_order_Value FROM pizza_sales
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/5f71b079-804d-454a-a382-89d8a4460041" width="150">

#### 3. Total Pizzas Sold
```
SELECT SUM(quantity) AS Total_pizza_sold FROM pizza_sales
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/2dfa9525-0b6b-45ce-be87-503aaa31b863" width="150">


#### 4. Total Orders
```
SELECT COUNT(DISTINCT order_id) AS Total_Orders FROM pizza_sales
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/d944d758-c714-4ba4-9da8-8df530a60727" width="150">

#### 5. Average Pizzas Per Order
```
SELECT CAST(CAST(SUM(quantity) AS DECIMAL(10,2)) / 
CAST(COUNT(DISTINCT order_id) AS DECIMAL(10,2)) AS DECIMAL(10,2))
AS Avg_Pizzas_per_order
FROM pizza_sales
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/84138b38-260a-437f-a8fb-d0625b7c04f0" width="150">


### B. Charts 

#### 1. Hourly Trend for Total Pizzas Sold
```
SELECT DATEPART(HOUR, order_time) as order_hours, SUM(quantity) as total_pizzas_sold
from pizza_sales
group by DATEPART(HOUR, order_time)
order by DATEPART(HOUR, order_time)
```

<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/b9e263d1-01c8-4503-a551-c1052f34de05" width="200">


#### 2. Weekly Trend for Orders
```
SELECT 
    DATEPART(ISO_WEEK, order_date) AS WeekNumber,
    YEAR(order_date) AS Year,
    COUNT(DISTINCT order_id) AS Total_orders
FROM 
    pizza_sales
GROUP BY 
    DATEPART(ISO_WEEK, order_date),
    YEAR(order_date)
ORDER BY 
    Year, WeekNumber;
```

<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/c74df234-c054-4be2-abff-27a770f09211" width="420">

#### 3. % of Sales by Pizza Category
```
SELECT pizza_category, CAST(SUM(total_price) AS DECIMAL(10,2)) as total_revenue,
CAST(SUM(total_price) * 100 / (SELECT SUM(total_price) from pizza_sales) AS DECIMAL(10,2)) AS PCT
FROM pizza_sales
GROUP BY pizza_category
```

<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/7c512d27-3e19-4d5b-ba37-216254810e68" width="200">

#### 4. % of Sales by Pizza Size
```
SELECT pizza_size, CAST(SUM(total_price) AS DECIMAL(10,2)) as total_revenue,
CAST(SUM(total_price) * 100 / (SELECT SUM(total_price) from pizza_sales) AS DECIMAL(10,2)) AS PCT
FROM pizza_sales
GROUP BY pizza_size
ORDER BY pizza_size
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/28d326d0-f76e-407f-9efe-e380596081a8" width="200">

#### 5. Total Pizzas Sold by Pizza Category
```
SELECT pizza_category, SUM(quantity) as Total_Quantity_Sold
FROM pizza_sales
WHERE MONTH(order_date) = 2
GROUP BY pizza_category
ORDER BY Total_Quantity_Sold DESC
```

<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/89568b7b-6788-420d-af51-fbbd234acf24" width="200">

#### 6. Top 5 Pizzas by Revenue
```
SELECT Top 5 pizza_name, SUM(total_price) AS Total_Revenue
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Revenue DESC
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/01dbfbdf-6bf0-471f-bd8e-4bd5d9c40b39" width="200">

#### 7. Bottom 5 Pizzas by Revenue
```
SELECT Top 5 pizza_name, SUM(total_price) AS Total_Revenue
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Revenue ASC
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/e8bf8ceb-f6a2-46c2-bcc9-7e4d1d3121cd" width="200">

#### 8. Top 5 Pizzas by Quantity
```
SELECT Top 5 pizza_name, SUM(quantity) AS Total_Pizza_Sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Pizza_Sold DESC
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/a575406b-24fd-4424-a993-54fdf45e6675" width="200">

#### 9. Bottom 5 Pizzas by Quantity
```
SELECT TOP 5 pizza_name, SUM(quantity) AS Total_Pizza_Sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Pizza_Sold ASC
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/88a31c40-ec1e-461a-85e9-3210f397588e" width="200">

#### 10. Top 5 Pizzas by Total Orders
```
SELECT Top 5 pizza_name, COUNT(DISTINCT order_id) AS Total_Orders
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Orders DESC
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/bb7cb65f-0318-4b6d-9958-36a1c4911571" width="200">

#### 11. Bottom 5 Pizzas by Total Orders
```
SELECT Top 5 pizza_name, COUNT(DISTINCT order_id) AS Total_Orders
FROM pizza_sales
GROUP BY pizza_name
ORDER BY Total_Orders ASC
```
<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/5e5496f9-2e43-480c-b960-df9970c0d87a" width="200">

#### ***Note: If we want to apply the pizza_category or pizza_size filters to the above queries we can use WHERE clause. Follow some of below examples***
```
SELECT Top 5 pizza_name, COUNT(DISTINCT order_id) AS Total_Orders
FROM pizza_sales
WHERE pizza_category = 'Classic'
GROUP BY pizza_name
ORDER BY Total_Orders ASC
```


## **Designing a PowerBI Dashboard: My Approach 📊💡**

In crafting a comprehensive dashboard in Power BI, I followed a systematic approach to ensure accurate representation and insightful analysis. Here's an overview of the steps I took:

![App Screenshot](https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/448b794e-dea6-41ae-bcfa-72ec64c56b17)

### 1. Measures Addition:

My initial step involved the addition of key measures that serve as the foundation for insightful KPIs and charts. Some examples include:
- `COUNTD([Order Id])` for tracking Total Orders.
- `SUM([Quantity])` to quantify Total Pizzas Sold.
- `SUM([Total Price])` to calculate the Total Revenue.
- `([TotalPizzasSold]/[TotalOrders])` for Avg Pizzas Per Order.
- `([TotalRevenue]/[TotalOrders])` for Avg Order Value.

### 2. KPI Creation:

With measures in place, I crafted essential Key Performance Indicators (KPIs) to gauge critical aspects of the business, such as Total Orders, Total Pizzas Sold, and Total Revenue. These KPIs provide a quick and comprehensive overview of the outlet's performance.

![App Screenshot](https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/224aed93-db36-48ac-bb80-e917311c6799)


### 3. Chart Development:

Following KPIs, my focus shifted to the creation of diverse charts, aligning with the specified requirements. Stacked bar charts for hourly trends, line charts for weekly trends, pie charts depicting sales distribution, funnel charts for category-specific sales, and bar charts spotlighting top and bottom performers were meticulously designed to provide a visually engaging representation of the data.

<img src="https://github.com/tarundirector/HR-Analytics-using-PowerBI/assets/85684655/0daaf316-e597-4091-a3c2-abc85860caa0" width="400">



### 4. Validation and Cross-Verification:

Ensuring the accuracy of the presented data was paramount. To achieve this, I cross-verified the dashboard values with SQL queries as given above.

By verifying dashboard outputs against SQL-calculated values, I instilled confidence in the reliability of the presented insights.




## 🚀 Conclusion

In conclusion, this Tableau-driven Pizza Sales Analytics Dashboard not only meets the client's requirements but goes beyond, offering a comprehensive view of the business dynamics. From key performance indicators to visually compelling charts, each element is meticulously crafted to provide actionable insights for the outlet owner. The integration of SQL queries ensures data accuracy, validating the dashboard's reliability. This analytics tool stands as a valuable asset for strategic decision-making and operational optimization in the dynamic realm of pizza sales.
