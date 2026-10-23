# Exploratory Data Analysis

## EDA Process

### 1. Analysis Requirements <br>
The following requirements were obtained for this project: <br>
- Owner's questions:
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
| money - Date | Total sales from 2024 to 2025 reached IDR 112.2 million, with monthly sales ranging between IDR 5 million and IDR 13 million. |
| money - Date | Sales increased significantly in October 2024 before dropping sharply through January 2025, then rose significantly again in February 2025. |
| money - coffee_name | Most products showed an increase in sales in October 2024 and February 2025. | 
| money - coffee_name | Latte was the best-selling product, reaching IDR 26.8 million, while Espresso was the worst-selling product, at approximately IDR 2.6 million, between 2024 and 2025.
| money - coffee_name | Latte, Americano with Milk, and Cappuccino are the best-performing products, with sales exceeding IDR 17 million. |
| money - Weekday | Monday and Tuesday were the days with the best sales performance. |
| money - Weekday | The weekend, Saturday and Sunday, are the days with the worst sales performance. |
| money - Time | 10 a.m. and 4 p.m. are the times with the best performance. |
| money - Time | 6 a.m. is the time with the worst performance. |
| money - cash_type | All transactions are carried out using a card-based method. |
