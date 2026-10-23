# Data Understanding and Cleaning

## Data Understanding

### 1. Data Source and Overview <br>
This section describes the source, scope, and general characteristics of the dataset used for the cafe sales analysis.

- Data Source: [kaggle](https://www.kaggle.com) <br>
- Data Period: March 2024 - March 2025 <br>
- Number of records: 3,547 <br>
- Number of columns: 11 <br>
- Data scope: Transaction, Date and time, Products, and Prices

### 2. Data Structure and Description <br>
This section explains the dataset structure, column definitions, data types, and their relevance to the analysis.

| Column | Data_Type | Description |
| --- | --- | --- |
| hour_of_day | Number | Indicates the hour at which a transaction took place |
| cash_type | String | Shows the payment method used by the customer |
| money | Number | Displays the amount paid by the customer for each product purchased |
| coffee_name | String |Shows the name of the product purchased |
| Time_of_day | String | shows the time-of-day category (morning, afternoon, or night) when the transaction occurred | 
| Weekday | String | Indicates the day of the week (Mon, Tue, etc.) when the transaction took place |
| Month_name | String | Shows the month (Jan, Feb, etc.) when the transaction occurred |
| Weekdaysort | Number | rovides a numerical representation for the day of the week |
| Monthsort | Number | Provides a numerical representation for the month |
| Date | Date | Indicates the specific date on which the transaction took place |
| Time | Time | Shows the time at which the transaction was conducted |

## Data Cleaning

### 1. Data Cleaning Framework <br>
- Conceptualise the data: understand the dataset by examining metrics and dimensions, and crafting a narrative from the recorded data. <br>
- Locate solvable issues: the first stage of data cleaning involves addressing issues that can be resolved immediately. <br>
- Evaluate unsolvable issues: note which issues cannot be resolved and require investigation by another team, or simply leave them as they are. <br>
- Augment the data: add new data to the existing dataset to improve the quality of the analysis. <br>
-Note and document: record all findings and actions taken in the Issue Log.

### 2. Data Cleaning Process

#### Step 1: Conceptualize the data <br>
Before proceed further, we must understand the nature of the data we have. The aim is to identify what needs to be considered and prioritised during the data cleaning process. This can be done as shown below.

1. Create a narrative based on a single existing record <br>
   On a **Weekday**, specifically on **Date** at **Time**, a transaction was made using **cash_type** for **coffee_name** at a price of **money**.

2. Defining the key metrics
   The key metric is **money**

3. Defining the key dimensions
   There are several dimensions in this project, such as **Date**, **Time**, **Weekday**, **coffee_name**, and **cash_type**.

#### Step 2: Locate solvable issues <br>
The next step is to identify where the issues exist and then work out how to resolve them.

- Solvable issues that were identified: <br>
  a. Inconsistent data format in column **money**, no currency symbol.
  b. Inconsistent data format in column **Time**, no time data displayed.

#### Step 3: Evaluate unsolable issue <br>
There are no unsolvable issues in this dataset.

#### Step 4: Augment the data <br>
No further data augmentation is performed because the data already consists of transformed results.

#### Step 5: Note and document <br>
Once the issues in the data have been recorded in the Issue Log, at this stage the entries are filled in by noting down the solution for each problem identified.

| Table | Column | Issue_type | Issue_desc | Row_count | Status | Resolution |
| --- | --- | --- | --- | --- | --- | --- |
| Coffee_sales | money | inconsistency data format | no currency symbol | 3,547 | Solvable | *1,000, change data format into accounting to show the symbol of the currency |
| Coffee_sales | Time | inconsistency data format | no time data displayed | 3,547 | Solvable | Change data format into time |



   
