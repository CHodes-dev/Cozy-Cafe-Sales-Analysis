# Deep Dive Analysis

## Deep Dive Analysis Process

### 1. North Star Metric <br>
- Focus on the 'money' column, and also calculate the AOV (Average Order Value) to determine the average amount customers spend per transaction. <br>
- Total orders are also an important metric for gauging the number of orders placed by customers.

### 2. North Star Dimensions <br>
- The 'Date' dimension is used to identify sales trends, including periods when sales increase or decrease. <br>
- The 'coffee_name' dimension helps determine which products are the best-sellers and contribute the most to total sales. <br>
- The 'Weekday' dimension reveals which days of the week have the strongest sales performance (peak days). <br>
- The 'Time' dimension identifies the hours during which the highest volume of sales occurs (peak hours).

### 3. North Star Goals <br>
This analysis will answer the following question:
- What caused sales to increase drastically in October 2024 and subsequently decline through January 2025? Is it the same factor that led to the increase in February 2025? <br>
- Which products saw an increase in sales in October 2024 and February 2025? <br>
- During days and hours with high foot traffic, which products sell the most?

## Results

### 1. High Level Sales Insights

**Initial insight #1**: Sales began to rise from August and peaked in October 2024, with a total of 429 orders generating monthly revenue of Rp 13.8 million. Following this peak, sales declined steadily from November 2024 to January 2025. This decline amounted to 54%. Sales in January totalled only around 201 orders.

**Initial insight #2**: However, following this decline, there was another surge in sales in February 2025, totalling 423 orders and generating Rp 13.2 million that month. A further decline occurred in March 2025, although it was not as severe as the previous one, amounting to 23%.

**Initial insight #3**: All customers made their transactions using card.

**Deep dive insights**

| Total Sales vs AOV | Total Sales vs Total Orders |
| --- | --- |
| !(total_sales_vs_aov)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/total_sales_vs_aov.png] | !(total_sales_vs_total_orders)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/total_sales_vs_total_orders.png] |

- Looking at the comparison of trends in total sales and AOV, in August 2024, when total sales began to rise by 10% from the previous month, the AOV actually reached its lowest point at Rp 27,992. Meanwhile, the total number of orders increased by 15% from the previous month. <br>
There was a decrease in the average order value per customer. However, this did not affect total sales; in fact, total sales increased due to the rise in the total number of orders.

- In the following months, September–October 2024, total sales, AOV and total orders all increased. Total sales rose by 39%, driven by a 12% increase in the average order value and a 24% rise in the total number of orders. <br>
Although the initial rise in total sales was driven solely by the increase in the total number of orders, once the average order value also began to rise, total sales reached their highest level yet. 

- A significant drop in total sales of up to 54% occurred between November 2024 and January 2025. This initial decline in November 2024 resulted in the café experiencing a drop in revenue of up to Rp 5.3 million. Although there was a 2%  increase in AOV, this was insufficient to offset the reduction in the number of orders. The same trend applied to December 2024 and January 2026. <br>
In December 2024, the number of orders was exactly the same as in November 2024, namely 259 orders. Coupled with a decrease in AOV to Rp 1,362, this further reduced total sales for that month by Rp 352,800. <br>
In January 2025, total sales fell by Rp 1,838,880 due to a significant drop in the total number of orders to 58. <br>
The reduction in the number of orders had a significant impact on the decline in total sales during this period.

- As it is known that the patterns of increase and decrease in total sales observed in previous months were driven by total orders, the second surge in total sales, which occurred in February 2025, rising by 107% or the equivalent of Rp 6,816,620, was also caused by a surge in total orders, which increased by 110%. Although the AOV fell by 2%, or Rp 593, this did not have a significant impact.

- Similarly, regarding the decline in total sales in March 2025, total orders fell again by 25%, equivalent to a reduction of 104 orders. This led to a 24% drop in total sales, equivalent to Rp 3,229,040.

### 2. Product Performance Insights

**Initial insight #1**: As much as 62% of revenue comes from just three products: Americano with Milk, Latte and Cappuccino. These three products have contributed approximately Rp 69 million in revenue over the past year.

**Initial insight #2**: Espresso, as a high-concentration coffee drink, has performed less than satisfactorily, contributing just 2% to the café’s total revenue, despite being the cheapest option compared to other products.

**Initial insight #3**: Whenever there is an increase in sales, the product types that contribute the most are not always the same. In October 2024, Latte (contributing 31%), Americano with Milk (contributing 18%) and Hot Chocolate (contributing 15%). Meanwhile, in February 2025, Americano (contributing 23%), Americano with Milk (contributing 20%) and Cocoa (contributing 15%).

**Deep dive insights**

!(sales_mix_by_product)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/sales_mix_by_product.png]

- There are several product categories with the best sales performance based on their time period.
    1. The products with the best sales performance from March 2024 to March 2025 were: Latte (Rp 26,875,300), Americano with Milk (Rp 24,751,120) and Cappuccino (Rp 17,439,140).
    2. The products that contributed to the surge in revenue in October 2024 were: Latte contributing 31%,  Americano with Milk contributing 18%, and Hot Chocolate contributing 15%. These three products accounted for at least 64% of that month’s total revenue, equivalent to Rp 4,995,360 out of Rp 13,891,160.
    3. The products that contributed to the surge in revenue in February 2024 were Americano which contributed 23%,  Americano with Milk  which contributed 20%, and Cocoa which contributed 15%. The combined contribution of these three reached 58%, equivalent to Rp 7,662,980 out of Rp 13,215,380.
 
!(sales_table)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/sales_table.png]

| !(table_total_sales_by_product)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/table_total_orders_by_product.png] | !(table_aov_by_product)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/table_aov_by_product.png] |
| --- | --- |

- Based on this trend, Latte and Americano with Milk have shown consistent sales performance, accounting for 46% of annual revenue. The high total sales of these two products are due to the high proportion of orders they generate, which account for 44% of all orders received by the café. Furthermore, both feature in the Top 3 during sales spikes. <br>
However, as almost half of the café’s revenue relies on these products, any decline in their performance due to a drop in the number of orders will have a significant impact on overall revenue performance.

- Meanwhile, Cappuccino, as one of the best-performing products throughout the year and accounting for 16% of the café’s total revenue, has shown a fairly stable trend without ever entering the Top 3 products during sales spikes. This is due to the high average order value for this product, which stands at Rp 35,883, customers purchasing Cappuccino have a higher average spend than those buying other top-selling products such as Latte and Americano with Milk.

- The two chocolate-based products, Hot Chocolate and Cocoa, consistently rank in the Top 3 whenever sales spikes occur, indicating that there is a customer segment that consistently seeks out these products. This customer niche tends to spend more to purchase these products, as evidenced by their average order values ranking amongst the top three. Hot Chocolate even takes first place with the highest AOV, reaching Rp 35,991, whilst Cocoa ranks third with an AOV of Rp 35,653.

- Americano, as the best-selling product during the spike in February 2025, had shown a fairly stable pattern in the preceding months with reasonably good sales performance, contributing 16% to the total number of orders and thus ranking third in terms of the number of orders received. <br>
The high sales recorded in February 2025 were due to a more than four-fold increase in the number of orders. This may have been caused by external trends or a shift in customer preferences towards a stronger coffee flavour.

- Espresso, as a brewed coffee product without any added water or milk, has a very strong coffee flavour. For the majority of customers, who are predominantly students and young adults, this product is not the first choice. The combination of a low average transaction value for this product, just Rp 20,885, and an order volume of only 129 cups per year means its performance is not as strong as that of other products.

### 3. Day and Time Performance Insights

**Initial insight #1**: On average, a café sells 39 cups a day and generates Rp 1.2 millions. On the busiest day, Tuesday, cafés sell an average of up to 44 cups, with total sales reaching Rp 1.3 millions. This figure differs by only Rp 371,000 from total sales on Saturday, the day with the lowest sales, which averages just 32 cups.

**Initial insight #2**: The busiest times are at 10 am and 4 pm. On average over the course of a week, 47 cups are sold at 10 am. Meanwhile, sales pick up again at 4 pm, with an average of 40 cups sold.

**Initial insight #3**: Meanwhile, the period between 6 am and 7 am sees the lowest sales, with an average of just 8 cups sold during that time.

**Deep dive insights**

!(total_sales_by_mon_tue)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/total_sales_by_mon_tue.png]

| !(top_product_mon)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/top_prodct_mon.png] | !(top_product_tue)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/top_product_tue.png] |
| --- | --- |

- Mondays and Tuesdays, specifically between 10 am and 11 am, 4 pm and 7 pm, are the busiest times. These periods account for at least 26%–27% of daily income. <br>
At these times, people whether students or office workers have already begun their respective activities. Customers who visit in the morning are those who need their morning coffee; those who visit in the afternoon are usually relaxing after a day’s work; and those who visit in the evening are typically socialising or working on assignments.

- On the busiest days, Mondays and Tuesdays between 10 am and 11 am, it turns out that the ‘Americano with Milk’ is the most frequently ordered drink, accounting for between 30% and 50% of revenue during those hours. Other popular drinks ordered at this time are the Latte and the Americano, contributing around 25% to 30% of the daily revenue. <br>
On Mondays at 4 pm and 7 pm, customers order more Lattes, which contribute 45% to 48% of revenue; they also order more Cappuccinos at these times than in the morning. <br>
Meanwhile, on Tuesdays at 4 pm, Hot Chocolate and Americano with Milk are the most popular, contributing 22% of revenue. At 7 pm, just as on Monday evenings, Lattes and Cappuccinos are the most popular choices.

!(total_sales_by_sat_sun)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/total_sales_by_sat_sun.png]

!(top_product_sat_sun)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/top_product_sat_sun.png]

- Sales are at their lowest at the weekend, with Saturday contributing 13% and Sunday 12% to total revenue. On both days, the busiest period is only in the morning, specifically between 10 and 11 am. <br>
People typically active at this time are those enjoying their weekend off after exercising or simply taking a morning stroll.

- Although Saturday and Sunday are the days with the lowest sales compared to other days, they also have peak hours that have the potential to boost customer purchases, namely between 10 and 11 am. Customers who make purchases at this time are only interested in three products: Latte, Americano with Milk, and Cappuccino. The percentage of revenue generated during these hours is also roughly the same, ranging from 18% to 38%.

| !(table_sales_6_7)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/table_sales_6_7_am.png] | !(table_sales_by_product_6_7_am)[https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/table_sales_by_product_6_7_am.png] |
| --- | --- |

- Between 6 and 7 am is the least busy time for orders; in fact, orders are only placed at 6 am on two days a week. This may be because not many people are active at that time.

- On Mondays and Fridays between 6 and 7 am, total sales are the highest, at Rp 775,840 and Rp 662,760 respectively, compared to other days at the same time. The best-selling products during this period are Latte contributing 35% of total sales; Cappuccino contributing 25%; and Americano with Milk contributing 20% of total sales between 6 and 7 am over the course of a week.

### Recommendations

Based on these findings, what the cafe owner can do is:

**1. Directional**

Indicates that there are matters that can be explored further, meaning it is not yet possible to draw immediate conclusions regarding what steps should be taken next.

**High Sales Level** <br>
- It is necessary to find out what happened between August and October—for instance, whether any sales strategies, such as product bundling, were implemented that might have increased the amount customers spent. <br>
- Investigating the reasons behind the decline in the number of customers making purchases between November 2024 and December 2025—could it be due to competitors or other factors? <br>
- Investigating the cause of the surge in purchases in February 2025—were there any external factors that influenced it? <br>
- Find out which type of card is most frequently used by customers, so that you can collaborate with the card issuer to offer discounts on purchases made using that card.

**Product** <br>
- Find out the reason behind the increase in sales at Espresso. Was there a specific customer segment that visited in February 2025, leading to this rise in sales?

**2. Actionable**

Clear and realistic insights for taking action.

**Products** <br>
- Lattes and Americano with Milk could serve as key products for a bundling program aimed at increasing AOV.
- To increase the sales volume of Cappuccino, one could focus on promoting this product.
- Focus promotional efforts on both products, Hot Chocolate and Cocoa, to increase interest in them on regular days.

**Day and Time** <br>
- Ensure that Lattes and Americanos with milk remain available on Mondays and Tuesdays at 10–11 a.m., 4 p.m., and 7 p.m, in order to meet customer demand.
- To maximize sales on weekend mornings, you could offer a special promotion during that time, featuring Latte and Americano as the main draws.
- Offer a special early-morning promotion, between 6-7 a.m. on Americano with Milk, Americano, and Cappuccino to increase the number of purchases.
