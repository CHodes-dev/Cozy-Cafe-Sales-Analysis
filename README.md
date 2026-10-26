# Cozy Cafe Sales Analysis

### Project Background

Cozy Cafe is a grab-and-go style café that has been in operation since March 2024. Its menu features eight beverage options, ranging from coffee-based to chocolate-based drinks. Located near several campuses, the café has become a popular choice for students looking for quick and affordable drinks.

The owner wants to analyze sales data from the first year of operation to evaluate performance and identify areas for improvement. Insights and recommendations are provided on the following key areas: <br>
- Sales Trends Analysis: analyzing historical data to identify sales patterns that have occurred. <br>
- Product Performance: analyzing product performance in relation to its impact on sales. <br>
- Day and Time Performance: analyzing the time periods with the best or worst performance during the cafe's operation.

⚠️**Disclaimer**: This project does not represent actual events and was created specifically for portfolio purposes.

### Data Structure

The café transaction data is contained in a single table consisting of 11 columns and 3,547 rows, as shown below.

![data_structure](https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/data_structure.png)

Before analysis is conducted, the data must be cleaned and selected based on the requirements of the analysis. The steps for data cleaning and standardization can be viewed [here](https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/project_workflow/02_data_understanding_and_cleaning.md).

### Executive Summary

#### Overview of Findings

The cafe's sales trend over the year shows spikes occurring at two different times. The first increase occurred in October 2024, when the cafe's sales reached IDR 13.8 million, contributing approximately 12.4% to the total sales. The second increase happened in February 2025, when sales reached IDR 13.2 million, equivalent to 11.8% of the total sales. However, afterward, there was also a significant decline.

Here is a preview of the Cozy Cafe sales performance dashboard; to obtain the interactive dashboard, it can be downloaded [here](https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/docs/cozy_cafe_dashboard.pbix).

![prev_dashboard](https://github.com/CHodes-dev/Cozy-Cafe-Sales-Analysis/blob/main/images/prev_dashboard.png)

##### Sales Trends

- Sales began to increase from August and peaked in October 2024 with a total of 429 orders, generating a monthly revenue of Rp 13.8 million. After the highest sales occurred, sales continuously declined from November 2024 to January 2025. This decline reached up to 54%. Sales in January were only around 201 orders.
- However, after the decline, there was another surge in sales in February 2025 with 423 orders, generating Rp 13.2 million that month. A decline occurred again in March 2025, although not as severe as the previous one, which was 23%.
- All customers conduct transactions using cards.

##### Product Performance

- As much as 60% of the orders made come from just three products, Americano with Milk, Latte, and Americano. These three products contributed Rp 66.2 million in revenue over the past year, or 59% of the café's total revenue.
- Espresso, as a high-concentration coffee drink, shows less satisfactory performance, contributing 2% to the total revenue of the café, despite being the cheapest compared to other products.
- Every time there is an increase in sales, the type of product that contributes the most is not always the same. In October 2024, Latte (contributing 30%), Americano with Milk (contributing 18%), and Hot Chocolate (contributing 14%). Meanwhile, in February 2025, Americano (contributing 23%), Americano with Milk (contributing 20%), and Cocoa (contributing 15%).

##### Day and Time Performance

- On average, the café sells 39 cups each day and generates Rp 1.2 million per day. On the busiest day, Tuesday, the café sells an average of 44 cups with total sales reaching Rp 1.3 million. This value differs by only Rp 371,000 from the total sales on Saturday, the day with the least sales, which sells an average of 32 cups.
- The busiest times occur at 10 AM and 4 PM. On average, 47 cups are sold at 10 AM throughout the week. Meanwhile, at 4 PM, sales increase again with an average of 40 cups sold. The 6-7 AM time slot has the lowest sales, averaging only 8 cups sold during that period.
