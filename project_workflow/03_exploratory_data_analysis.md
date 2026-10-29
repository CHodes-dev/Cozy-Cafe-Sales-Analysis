# Exploratory Data Analysis

## EDA Process

### 1. Analysis Requirements <br>
The following requirements were obtained for this project: <br>
- Owner's questions:<br>
  a.) How has sales performance been throughout 2024–2025? <br>
  b.) Which products are the best-sellers? <br>
  c.) On which days are the most orders placed? <br>
  d.) During which hours is the highest sales generated? <br>
  e.) Which payment methods do customers use most frequently for their transactions? <br>
- Metric: money.
- Dimensions: Date, Time, Weekday, coffee_name, cash_type.
- Outcomes: The results will be used by the owner to consider ways to improve sales performance.

### 2. Stakeholder Goals <br>
- No decisions have been made at this time based on the observed sales trends and patterns. <br>
- KPIs: Total Sales, AOV, Total orders.
- Dimensions: Date, Time, Weekday, coffee_name, cash_type.

### 3. Column and Coverage <br>
Using the columns money, Date, Time, Weekday, coffee_name, and Time.

### 4. Aggregates and Anomalies <br>
Looking for key metrics, unexpected patterns, and outliers.

### 5. Notable Segments <br>
Conduct a deep dive by breaking down metrics according to the available dimensions.

## Results

Below are some initial findings obtained after conducting an analysis in Excel, utilizing pivot tables, conditional formatting (color scales), and sparklines.

| Metric - Dimension | Insight |
| --- | --- |
| money - Date | Sales began to rise from August and peaked in October 2024, with a total of 429 orders generating monthly revenue of Rp 13.8 million. Following this peak, sales declined steadily from November 2024 to January 2025. This decline amounted to 54%. Sales in January totalled only around 201 orders. |
| money - Date | However, following this decline, there was another surge in sales in February 2025, totalling 423 orders and generating Rp 13.2 million that month. A further decline occurred in March 2025, although it was not as severe as the previous one, amounting to 23%. |
| money - coffee_name | As much as 62% of revenue comes from just three products: Americano with Milk, Latte and Cappuccino. These three products have contributed approximately Rp 69 million in revenue over the past year. | 
| money - coffee_name | Espresso, as a high-concentration coffee drink, has performed less than satisfactorily, contributing just 2% to the café’s total revenue, despite being the cheapest option compared to other products. |
| money - coffee_name | Whenever there is an increase in sales, the product types that contribute the most are not always the same. In October 2024, Latte (contributing 31%), Americano with Milk (contributing 18%) and Hot Chocolate (contributing 15%). Meanwhile, in February 2025, Americano (contributing 23%), Americano with Milk (contributing 20%) and Cocoa (contributing 15%). |
| money - Weekday | Monday and Tuesday were the days with the best sales performance. |
| money - Weekday | The weekend, Saturday and Sunday, are the days with the worst sales performance. |
| money - Time | On average, a café sells 39 cups a day and generates Rp 1.2 millions. On the busiest day, Tuesday, cafés sell an average of up to 44 cups, with total sales reaching Rp 1.3 millions. This figure differs by only Rp 371,000 from total sales on Saturday, the day with the lowest sales, which averages just 32 cups. |
| money - Time | The busiest times are at 10 am and 4 pm. On average over the course of a week, 47 cups are sold at 10 am. Meanwhile, sales pick up again at 4 pm, with an average of 40 cups sold.|
| money - Time | Meanwhile, the period between 6 am and 7 am sees the lowest sales, with an average of just 8 cups sold during that time. |
| money - cash_type | All transactions are carried out using a card-based method. |
