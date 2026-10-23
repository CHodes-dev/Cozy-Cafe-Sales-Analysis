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

#### Initial insights <br>
- Total sales from 2024 to 2025 reached IDR 112.2 million, with monthly sales ranging between IDR 5 million and IDR 13 million. <br>
- Sales increased significantly in October 2024 before dropping sharply through January 2025, then rose significantly again in February 2025.
- All transactions are carried out using a card-based method.

#### Deep dive insights

**Point 1** <br>
- In October, the AOV saw a 14% increase, following a 22% decline the previous month. The trends for AOV and sales moved in tandem from August through October, both showing consistent, continuous growth. <br>
- Total orders also saw an increase during that period. <br>
  **Indication** <br>
  - The increase in total sales is primarily driven by an increase in customer spending and a rise in the number of orders placed.
  - Customers are purchasing more products, with the total value of their purchases also increasing.

**Point 2** <br>
- From November 2024 through January 2025, sales experienced a continuous decline; however, the AOV remained relatively stable, showing no significant increase or decrease (i.e., no fluctuations greater than +2% or -4%). <br>
  **Indication** <br>
  - A decline in the number of orders placed by customers has resulted in a decrease in revenue.

**Point 3** <br>
- In February 2025, there was an increase in the number of customer orders, while their AOV remained relatively stable (a 2% decrease from the previous month). <br>
  **Indication** <br>
  - There has been an increase in the number of customer orders, even though their spending amounts remain roughly the same as in previous months.

### 2. Product Insights

#### Initial insights <br>
- Most products showed an increase in sales in October 2024 and February 2025. <br>
- Latte was the best-selling product, reaching IDR 26.8 million, while Espresso was the worst-selling product, at approximately IDR 2.6 million, between 2024 and 2025. <br>
- Latte, Americano with Milk, and Cappuccino are the best-performing products, with sales exceeding IDR 17 million. <br>

#### Deep dive insights

**Point 1** <br>
- In October 2024, three products were the primary drivers of the increase in sales: the Latte, which accounted for 30%; the Americano with Milk, which accounted for 18%; and the Hot Chocolate, which accounted for 14%.

**Point 2** <br>
- In February 2025, Espresso accounted for the largest share at 23%, followed by Americano with Milk at 20% and Cocoa at 15%.

  **Indication** <br>
  - There are several product categories with the best performance, based on their respective timeframes.
  - Products with the best sales performance in 2024–2025: Latte, Americano with Milk, and Cappucono.
  - Products that saw an increase in sales in October 2024: Latte, Americano with Milk, and Hot Chocolate.
  - Products that saw an increase in sales in February 2025: Espresso, Americano with Milk, and Cocoa.

  Based on this, it follows that:
  - Latte and Americano with Milk show consistent sales performance.
  - Although cappuccino sales have not seen a surge, total sales have remained relatively stable, averaging IDR 1.3 million per month.
  - Throughout 2024 and up to January 2025, espresso remained the product with the lowest sales; however, it managed to reach the highest sales in February 2025.
  - Chocolate-based products (Hot Chocolate and Cocoa) consistently rank among the items in high demand whenever a sales surge occurs.

### 3. Day and Time Insights

#### Initial insights <br>
- Monday and Tuesday were the days with the best sales performance. <br>
- The weekend, Saturday and Sunday, are the days with the worst sales performance. <br>
- 10 a.m. and 4 p.m. are the times with the best performance. <br>
- 6 a.m. is the time with the worst performance. <br>

#### Deep dive insights <br>

**Point 1** <br>
Busiest times and the products ordered most frequently.
| Day | Time | Product |
| --- | --- | --- |
| Monday | 10 a.m. | Americano with Milk |
| | 4 p.m. | Latte |
| Tuesday | 11 a.m. | Americano with Milk |
| | 7 p.m. | Latte |

**Point 2** <br>
The quietest day, including its busiest hour and the best-selling product during that time.
| Day | Time | Product |
| --- | --- | --- |
| Saturday | 11 a.m. | Americano |
| Sunday | 10 a.m. | Latte |

**Point 3** <br>
- 6 a.m. is the time with the poorest performance, and there are only three products that customers purchase most frequently during this time: Americano with Milk, Americano, and Cappuccino.

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
