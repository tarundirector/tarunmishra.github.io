
# 🛒E-commerce Sales Analysis and Customer Segmentation Report📦

![Image Alt Text](https://www.providencejournal.com/gcdn/authoring/2020/02/21/NPRJ/ghows-PJ-a02463cb-0970-4047-98b5-2cf730e90980-908abb7d.jpeg?width=660&height=348&fit=crop&format=pjpg&auto=webp)

In the dynamic world of e-commerce, understanding customer behavior and sales trends is pivotal for success. This report aims to analyze sales data to identify customer segments and provide actionable insights to optimize sales and improve profitability for an e-commerce company.

---

## **🎯 Problem Statement**

Analyze sales data to identify customer segments and provide actionable insights to optimize sales and improve profitability for an e-commerce company.

---

## **📊 Objectives**

- Identification of distinct customer segments based on purchasing behavior.
- Insights into sales trends, product performance, and customer preferences.
- Actionable recommendations to improve sales strategies and profitability.

---

## 💡**Dataset Description**

#### 1. **Row ID**: Unique identifier for each row.
#### 2. **Order ID**: Unique Order ID for each Customer.
#### 3. **Order Date**: Order Date of the product.
#### 4. **Ship Date**: Shipping Date of the Product.
#### 5. **Ship Mode**: Shipping Mode specified by the Customer.
#### 6. **Customer ID**: Unique ID to identify each Customer.
#### 7. **Customer Name**: Name of the Customer.
#### 8. **Segment**: The segment where the Customer belongs.
#### 9. **Country**: Country of residence of the Customer.
#### 10. **City**: City of residence of the Customer.
#### 11. **State**: State of residence of the Customer.
#### 12. **Postal Code**: Postal Code of every Customer.
#### 13. **Region**: Region where the Customer belongs.
#### 14. **Product ID**: Unique ID of the Product.
#### 15. **Category**: Category of the product ordered.
#### 16. **Sub-Category**: Sub-Category of the product ordered.
#### 17. **Product Name**: Name of the Product
#### 18. **Sales**: Sales of the Product.
#### 19. **Quantity**: Quantity of the Product.
#### 20. **Discount**: Discount provided.
#### 21. **Profit**: Profit/Loss incurred.

### **🔍 Dataset Overview: Key Statistics and Shape**

- **Missing Values:** The dataset does not have any missing values in the provided columns.

#### **Summary Statistics:**

- **Sales:** The mean sales is $229.86, ranging from $0.44 to $22,638.48.
- **Quantity:** The mean quantity is 3.79, ranging from 1 to 14.
- **Discount:** The mean discount is 15.62%, ranging from 0% to 80%.
- **Profit:** The mean profit is $28.66, ranging from -$6,599.98 to $8,399.98.

**Date Range:**

- Maximum Order Date: 2017-12-30
- Minimum Order Date: 2014-01-03


#### **Dataset Shape Overview:**

- **Complete Data:** 9994 Rows, 21 Columns

This dataset provides comprehensive information about sales transactions, including customer details, product information, and financial data.

---

## 📊**PowerBI Dashboard**

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/fb4b8b61-7016-4ef0-8a18-3f8be694ba9e)

The PowerBI dashboard provides a comprehensive analysis of sales data to facilitate strategic decision-making for an e-commerce company. Its primary purpose is to optimize sales and improve profitability by identifying customer segments and analyzing sales trends. 

Key features of the dashboard include:
1. **Filters**: Segmentation of products allows users to analyze sales data based on different product categories, providing insights into the performance of each segment.

2. **KPIs**: Year-to-date (YTD) sales, profit, quantity, and profit margin metrics offer a quick overview of the company's financial performance, aiding in performance evaluation and goal tracking.

3. **Sales by Category Table**: A detailed breakdown of sales by category enables users to understand which product categories are driving revenue and identify trends over time.

4. **Sales by State Map**: Geographic visualization of sales data helps identify regions with high or low sales volumes, allowing for targeted marketing efforts and resource allocation.

5. **Top and Bottom Products Bar Charts**: These charts highlight the best and worst-performing products, helping identify successful products to capitalize on and underperforming products that may require attention.

6. **YTD Sales by Region Donut Chart**: Visualization of sales distribution across different regions provides insights into regional performance and helps identify areas for growth or improvement.

7. **YTD Sales by Shipping Type Donut Chart**: Analysis of sales by shipping type allows users to assess the effectiveness of different shipping methods and their impact on sales.

Overall, the PowerBI dashboard serves as a powerful tool for sales analysis and strategic planning, empowering stakeholders to make informed decisions to optimize sales and improve profitability.

![Untitled design](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/62e6e9be-0945-4b6a-9102-f2da9b21043a)
_(Dashboard in Action)_

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/ca99403f-7a8a-4e45-a656-555808e1e701)
_(Model View for Dashboard)_

---

## **🧠Findings and Insights**

For a more detailed analysis visit the [Kaggle Notebook](https://www.kaggle.com/code/tarundirector/sales-analysis-and-customer-segmentation-eda#%5B2%5D-%F0%9F%94%8D-Dataset-Overview)

### **[1] 🌐Customer Segmentation:**

![Image Alt Text](https://www.mediaheroes.com.au/wp-content/uploads/2023/09/market-segmentation-media-heroes-banner.webp)

Understanding customer segments is crucial for tailoring marketing strategies and providing personalized experiences. Through cluster analysis, distinct customer segments based on purchasing behavior were identified.

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/9af87c5a-ad8b-46c2-8e60-27fa124de971)

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/67953744-00b1-4688-904f-ee64f233fde2)


#### 💡 **Cluster 0: Regular Shoppers**
- **Shipping Preferences:** They mostly prefer "Standard Class" shipping.
- **Order Frequency:** Regular shopping behavior with a high count of orders.
- **Segment Composition:** Primarily consumers.
- **Geographical Distribution:** Spread across various regions, significant presence in West and East regions.
- **Sales and Profit:** Moderate values, focusing on small to medium-sized orders.
- **Top Cities:** New York City, Los Angeles, Philadelphia.
- **Top States:** California, New York, Texas.
- **Discounts:** Moderate discounts offered, with a tendency towards higher rates.
- **Product Preferences:** Varied, purchasing across different product categories.

#### 💡 **Cluster 1: Premium Shoppers**
- **Shipping Preferences:** Prefer "First Class" or "Second Class" for faster delivery.
- **Order Frequency:** Moderate, emphasizing quality over quantity.
- **Segment Composition:** Predominantly corporate customers.
- **Geographical Distribution:** Concentrated in East and West regions.
- **Sales and Profit:** Higher compared to other clusters, indicating higher value purchases.
- **Top Cities:** New York City, Los Angeles, Seattle.
- **Top States:** California, New York, Texas.
- **Discounts:** Moderate, but tend to purchase even without discounts.
- **Product Preferences:** High-quality products and luxury items are favored.

#### 💡 **Cluster 2: Bulk Buyers**
- **Shipping Preferences:** Prefer "Standard Class" for cost-effectiveness.
- **Order Frequency:** Moderate, but tend to purchase in larger quantities.
- **Segment Composition:** Diverse mix of consumers, corporate, and home office customers.
- **Geographical Distribution:** Spread across different regions, significant presence in West and East regions.
- **Sales and Profit:** Highest among clusters, focusing on bulk orders.
- **Top Cities:** New York City, Los Angeles, San Francisco.
- **Top States:** California, New York, Texas.
- **Discounts:** Preferential towards lower or no discounts, focusing on bulk purchases.
- **Product Preferences:** Bulk purchases across various product categories, often for resale or distribution purposes.

---

### **[2] 💰Sales & Profitability Analysis:**

![Image Alt Text](https://wp-bn.salesforce.com/blog/wp-content/uploads/sites/2/2023/10/Sales_Quotas.jpg)

The analysis of sales and profitability trends over time provides valuable insights into the performance of the e-commerce company across different years, months, and days of the week.

#### **➡️Yearly Trends:**

The yearly analysis reveals a consistent growth trend in both sales and profitability over the years 2014 to 2017. Sales increased steadily from 2014 to 2017, with the highest recorded sales in 2017, reaching $733,215.25. Similarly, profitability showed a positive trajectory over the same period, with the highest profit recorded in 2017, totaling $93,439.26.

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/757c6ac9-4755-4f3a-87df-5a7eff222d2f)

#### **➡️Monthly Trends:**
Analyzing sales and profitability on a monthly basis reveals fluctuations and patterns throughout the year. Profits were highest in December across all years, indicating increased sales during the holiday season. Moreover, the months of September and October also showed notable profitability figures, suggesting potential seasonal trends or promotional activities during these months.

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/d0aa9e59-09bf-4daa-a462-0586de9f5708)

#### **➡️Daily Trends:**
Examining sales trends by day of the week provides insights into consumer behavior and purchasing patterns. Sundays consistently showed the highest average sales across all years, followed by Saturdays and Wednesdays. This suggests that weekends may be peak periods for customer purchases, while mid-week days also exhibit significant sales activity.

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/a4927d6c-65ca-4fcb-87a8-bf672b1bb067)


#### 🚀🔄Insights and Recommendations:

- The overall upward trend in sales and profitability indicates the company's growth and success over the years.
- Seasonal trends, particularly during the holiday season, suggest opportunities for targeted marketing campaigns and promotions to capitalize on increased consumer spending.

---

#### **➡️Regional Performance Overview:**

The sales and profitability of the e-commerce company vary significantly across different regions. Here's a summary of the performance of each region:

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/df970e09-d31c-4cb8-a63d-d2a1a0521432)

#### 1. **Central Region:**
   - **Sales:** The Central region contributes a substantial amount to the company's total sales, with a total sales figure of $501,239.89.
   - **Profitability:** Despite the high sales volume, the profitability in the Central region is comparatively lower, standing at $39,706.36.
   - **Insights:** While the Central region generates significant revenue, efforts are needed to improve profitability, possibly through cost optimization or pricing strategies.

#### 2. **East Region:**
   - **Sales:** The East region leads in terms of sales, accounting for the highest total sales of $678,781.24.
   - **Profitability:** Alongside high sales, the East region also demonstrates strong profitability, with total profits reaching $91,522.78.
   - **Insights:** The East region is a key driver of both sales and profitability, indicating strong market demand and effective operational performance.

#### 3. **South Region:**
   - **Sales:** With total sales amounting to $391,721.91, the South region contributes significantly to the company's revenue.
   - **Profitability:** Profitability in the South region is respectable, standing at $46,749.43.
   - **Insights:** The South region shows promising sales figures, and efforts to maintain profitability should be continued to ensure sustainable growth.

#### 4. **West Region:**
   - **Sales:** The West region demonstrates robust sales performance, with total sales reaching $725,457.82.
   - **Profitability:** Profitability in the West region is the highest among all regions, totaling $108,418.45.
   - **Insights:** The West region is a standout performer in both sales and profitability, indicating strong market presence and effective business strategies.

#### **➡️Top Cities and States**:

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/6b531418-907f-4097-b80b-b1188f83145b)


- **Top Cities:** New York City, Los Angeles, and Seattle emerge as the top-performing cities in terms of sales revenue. These cities significantly contribute to the company's overall sales performance.
- **Top States:** California and New York lead in terms of total sales revenue, highlighting the importance of these states in driving overall sales growth.

#### 🚀🔄Insights and Recommendations:

- The East and West regions emerge as the primary drivers of sales and profitability, showcasing strong market demand and effective business operations.
- Efforts to improve profitability should be prioritized in regions with lower profitability, such as the Central region, to ensure sustainable growth.
- Focus on top-performing cities and states, such as New York City and California, to capitalize on high-demand markets and further enhance sales performance.

---

#### **➡️Least Profitable by Year (Sub-Category-wise):**
- Tables and Bookcases emerge as consistently unprofitable sub-categories across multiple years, with notable losses recorded in 2014, 2015, 2016, and 2017.
- Fasteners and Supplies show mixed performance, with both profitable and unprofitable years.

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/d4a043e8-99a8-4711-8657-eefc0760dd88)

#### **Bottom Cities in Terms of Profit:**
- Philadelphia, Houston, and San Antonio are the cities with the lowest profitability, indicating challenges in these markets.
- Lancaster, Chicago, and Burlington also exhibit significant losses, suggesting issues with sales performance or operational efficiency in these areas.

#### **Bottom States in Terms of Profit:**
- Texas, Ohio, and Pennsylvania emerge as the states with the lowest profitability, indicating broader regional challenges.
- Illinois, North Carolina, and Colorado also show substantial losses, pointing towards systemic issues impacting profitability.

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/8f1ccd9d-3cbe-4c42-9b2b-645acb092ff3)

#### 🚀🔄Insights and Recommendations:
- Tables, Bookcases, and certain geographical regions, particularly Philadelphia, Houston, and Texas, consistently demonstrate poor profitability across multiple years.
- The analysis underscores the need for targeted strategies to address the challenges posed by unprofitable products and regions, such as optimizing pricing strategies, refining product offerings, and enhancing operational efficiency in specific markets.
- Conduct a detailed review of pricing strategies and cost structures for unprofitable product categories.
- Explore opportunities for product diversification or SKU rationalization to mitigate losses in underperforming sub-categories.
- Implement targeted marketing and sales initiatives to stimulate demand and improve sales performance in low-profit regions.
- Invest in operational improvements and logistics optimization to reduce costs and enhance profitability in challenging markets.

---

### **[3] 🛍️Customer Behavior Analysis:**

![Image Alt Text](https://www.customerthermometer.com/img/Ways-to-Increase-Customer-Loyalty1-1.jpg)

#### **➡️Impact of Discounting on Sales and Profitability**

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/0ff5278a-0f1d-4900-8ecf-be1bd408314a)

- **Sales Impact**: As expected, higher discounts tend to result in increased sales. We observed a positive correlation between the discount rate and sales revenue. However, it's essential to note that while higher discounts may drive higher sales volumes, they may not always translate to increased profitability.
  
- **Profitability Impact**: Interestingly, our analysis uncovered a nonlinear relationship between discount rates and profitability. While moderate discounts (10% to 20%) were associated with positive profit margins, offering deeper discounts beyond 20% led to diminishing returns and, in some cases, negative profitability. This suggests that while discounts can stimulate sales, they can also erode profit margins if not managed effectively.

#### **➡️Correlation Between Customer Segments and Product Categories**

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/6832d295-9efe-4204-8522-037a3c83a5a2)


- **Furniture**: Consumer segments showed the highest sales performance in the furniture category, followed closely by the Corporate segment. This suggests that furniture products may have higher appeal or demand among individual consumers and corporate buyers.
  
- **Office Supplies**: The Corporate segment exhibited comparable sales performance in the office supplies category, indicating a strong demand for office-related products among corporate buyers. However, there was relatively lower performance in the home office segment.
  
- **Technology**: The technology category demonstrated consistent sales performance across all customer segments, with no significant variations observed. This indicates a universal appeal for technology products among consumers, corporate clients, and home office users.

#### 🚀🔄 Insights and Recommendations

- **Optimize Discount Strategies**: Tailor discounts to specific customer segments and product categories to maximize sales without compromising profitability. Consider dynamic pricing algorithms for optimal discount levels.

- **Focus on Top Categories**: Prioritize product categories with high sales potential among specific customer segments. Invest in marketing efforts to boost sales for top-performing categories.

- **Refine Customer Segmentation**: Continuously refine segmentation strategies to meet the unique needs of different customer segments. Leverage machine learning for identifying hidden patterns and micro-segments.

- **Monitor Profitability**: Implement robust tracking mechanisms to assess the impact of discounts on profitability. Set clear guidelines to maintain a balance between sales growth and profit margins.

---

### **[4] 📦Shipping Analysis:**

![Image Alt Text](https://wl-img-prd.s3-accelerate.amazonaws.com/c1d51abd-29d9-488e-8dd9-a27a6658b17b-h.png)


#### **➡️Shipping Preferences:**

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/56aa862f-b023-4936-bd3a-4ac23ff4a4c2)

The data revealed that the majority of customers, irrespective of their segment (Consumer, Corporate, Home Office), prefer Standard Class shipping, followed by Second Class and then First Class. Same Day shipping is the least preferred option among customers.

#### **➡️Shipping Time Analysis:**

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/64f8e650-a1e0-4ce4-b4d1-b239a7cb3b3e)


- First Class: Approximately 2.18 days on average.
- Same Day: Very low shipping time, averaging at 0.04 days.
- Second Class: About 3.24 days on average.
- Standard Class: The longest shipping time, averaging at 5.01 days.

These findings suggest that customers prioritize quicker delivery options such as First Class and Same Day when available, although Standard Class remains the most commonly chosen option, possibly due to its lower cost.

**➡️Correlation Analysis for Average Order Value & Shipping Time:**

![image](https://github.com/tarundirector/tarunmishra.github.io/assets/85684655/2b6872ed-dc57-4b14-8229-f1a0e5f41f6e)


To explore the relationship between shipping times and sales, we analyzed the correlation between shipping time and sales value. The analysis did not reveal a significant correlation between faster shipping times and higher order values. Despite some fluctuations, the overall trend suggests that faster shipping times do not consistently lead to higher sales values.


**🚀🔄 Insights and Recommendations:**

- **Customer Preferences:** Customers prioritize cost-efficiency over speed, preferring Standard Class shipping. Offering flexible shipping options, including competitive rates for expedited shipping, can cater to those seeking quicker delivery.
- **Shipping Operations Optimization:** Analyzing shipping times can streamline operations and enhance efficiency. Investing in logistics infrastructure can reduce shipping times, boosting customer satisfaction.
- **Sales Strategy Enhancement:** Although faster shipping may not always increase sales values, it can improve customer experience and loyalty. Implementing transparent tracking and proactive communication can drive repeat purchases.
- **Data-Driven Decision Making:** Continuous monitoring of shipping preferences and their impact on sales is crucial. Leveraging data analytics tools can provide deeper insights into customer behavior for agile decision-making.

---

## **Conclusion**

![Image Alt Text](https://assets.epicurious.com/photos/57eebe2eb382c3c017d3fff0/16:9/w_2560%2Cc_limit/supermarket-shelves.jpg)

The analysis of e-commerce sales data has provided valuable insights into customer behavior, sales trends, and profitability drivers. By leveraging data-driven strategies, businesses can optimize their operations and enhance customer satisfaction, leading to improved sales performance and profitability.

### **🚀Key Takeaways:**

- **Customer Segmentation:** Identify distinct customer segments based on purchasing behavior to tailor marketing strategies and provide personalized experiences.

- **Sales & Profitability Analysis:** Analyze sales trends over time to understand peak seasons and profitability drivers. Focus on top-performing regions and product categories to maximize revenue.

- **Discount Strategy Optimization:** Optimize discount strategies to balance sales growth with profitability. Tailor discounts to specific customer segments and product categories for maximum impact.

- **Shipping Efficiency Enhancement:** Streamline shipping operations to reduce delivery times and improve customer satisfaction. Offer flexible shipping options to cater to diverse customer preferences.

- **Data-Driven Decision Making:** Continuously monitor sales, profitability, and customer behavior metrics to make informed decisions. Leverage data analytics tools to uncover hidden insights and drive business growth.

### **🔄Important Pointers:**

- **Segmentation:** Refine customer segmentation strategies to meet the unique needs of different customer segments.

- **Promotional Campaigns:** Launch targeted marketing campaigns during peak seasons to capitalize on increased consumer spending.

- **Operational Efficiency:** Invest in logistics and fulfillment infrastructure to streamline shipping operations and enhance efficiency.

- **Customer Experience:** Prioritize customer experience initiatives, such as transparent tracking and proactive communication, to improve satisfaction and loyalty.

- **Continuous Improvement:** Implement a culture of continuous improvement, leveraging data analytics to identify areas for optimization and innovation.

By implementing these actionable recommendations, businesses can position themselves for success in the competitive e-commerce landscape, driving sustainable growth and profitability.
