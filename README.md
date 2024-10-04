# Bike-Share

# Objective

The objective of this project is to analyze and create a dashboard for Toman Bike Share that highlights key performance metrics to support informed decision-making on a potential 25% increase in bike shares for 2023.

## User story

We can recall that our bike-share company increased the price of our rental bikes by 25% in 2022, and is considering another 25% increase for 2023. We need your expertise to analyze and create a dashboard for Toman Bike Share that highlights key performance metrics, helping us make an informed decision on moving forward.

Insights and recommendations should be provided on the following key areas: 
- Daily Revenue Analysis
- Yearly and monthly Profit and Revenue Trends for 2021 and 2022
- Quarterly Revenue
- Rider Demographics

This will help the company make informed decisions on whether to proceed with a 25% price increase.

# Data source 

- What data is needed to achieve our objective?

We need data on Toman Bike Share for 2021 and 2022 that includes their 
- Number of Riders
- Rider type
- Date
- Price
- Cost of goods
- Revenue
- Profit


Where is the data coming from? 

The data is sourced from Kaggle (contains 3 CSV files), [see here to find it.](https://www.kaggle.com/datasets/walmalki/toman-bike-share-dataset)

## Tools 



| Tool | Purpose |
| --- | --- |
| Excel | Exploring the data and cleaning |
| SQL Server | Cleaning, Testing, and Analyzing the data |
| Power BI | Visualizing the data via interactive dashboards |
| GitHub | Hosting the project documentation and version control |

# Data Cleaning, Structure & Testing
The companies main database structure consists of 3 tables: Bike Share 2021 table, Bike Share 2022 table, and Cost table, with combined total of 33 columns and row count of 34,761 records.

The data met the following criteria and constraints after cleaning:

- Only relevant columns were retained.
- All data types were appropriate for the contents of each column.
- No column contained null values, indicating complete data for all records.

Below is a table outlining the constraints on our cleaned dataset:

| Property | Description |
| --- | --- |
| Number of Rows | 34,758 |
| Number of Columns | 7 |

And here is a tabular representation of schema for our cleaned dataset:

| Column Name | Data Type | Nullable |
| --- | --- | --- |
| Date | date | NO |
| Rider_Type | varchar | NO |
| Riders | int | NO |
| Price | float | NO |
| Cost_of_Goods | Float | NO |
| Revenue | float | NO |
| Profit | float | NO |

Data Cleaning Steps:

1. Changed the data type of "riders" column from text to whole number.
2. Changed data type of "date" column from text to date, but it returned over 1,000,000 rows of errors. I fixed it by setting the date column format as "mm-dd-yyyy".
3. Checked for duplicate records. The duplicates in columns like "date", "rider_type" were excepted were perfectly fine for the analysis.
4. Checked for null values.
5. Created a Revenue column by calculating "riders * price".
6. Created a "Profit" column by calculating  "revenue - (Cost_of_goods * riders)".
7. Removed unnecessary columns by only selecting the ones I need and renamed columns using aliases.


# Executive Summary

### Overview of Findings

Toman Bike Share had a fantastic 2022, and numbers show that another price increase could work if we keep delivering good value to our riders. Instead of a 25% price increase for 2023, I suggest a 10% increase first to see how customers respond, and adjust if needed.

# Analysis 

## Findings

- What did we find?

For this analysis, we're going to focus on the key performance metrics below to get the information we need for our company -

Here are the key performance metrics:

1. Year-over-Year Growth (2021 vs. 2022).
2. Monthly Trends (2021 vs. 2022).
3. Quarterly Revenue Comparison.
4. Revenue by Rider Type.
5. Revenue by Day.


### 1. Year-over-Year Growth (2021 vs. 2022):


Total Riders increased from 1,243,103 in 2021 to 2,049,576 in 2022, indicating a significant rise of approximately 65%.
Total Revenue grew from $4,959,981 to $10,227,384, a 106% increase, suggesting strong financial performance.
Total Profit increased from $3,418,533 to $7,030,046, showing an approximate 106% growth in profit.

| Year | Riders          | Revenue         |   Profit  |
|------|-----------------|-----------------|-----------|
| 2021 | 1,243,103       | $4,959,981      | 3,418,533 |
| 2022 | 2,049,576       | $10,227,384     | 7,030,046 |



### 2. Monthly Trends (2021 vs. 2022):



### 3. Quarterly Revenue Comparison (2021 vs 2022):



### 4. Revenue by Rider Type:



### 5. Revenue by Day













