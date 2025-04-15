Dataset from: https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting

This project focuses on analyzing Walmart sales data to identify the top-performing branches and products, examine sales trends across various items, and gain insights into customer behavior. The goal is to explore opportunities for enhancing and optimizing sales strategies based on data-driven findings. The primary objective of this project is to analyze Walmart's sales data to uncover the various factors influencing sales performance across different branches.

What needed to be analyzed:
1. Product
   Perform an analysis of the data to gain insights into the various product lines, identify those that are performing the best, and highlight the ones that require improvement.

  question:
  1. How many unique product lines does the data have?
  2. What is the most common payment method?
  3. What is the most selling product line?
  4. What is the total revenue by month?
  5. What month had the largest COGS?
  6. What product line had the largest revenue?
  7. What is the city with the largest revenue?
  8. What product line had the largest VAT?
  9. Fetch each product line and add a column to those product lines showing "Good", "Bad". Good if it is greater than average sales
  10. Which branch sold more products than the average product sold?
  11. What is the most common product line by gender?
  12. What is the average rating of each product line?
    
2. Sales
   This analysis seeks to uncover the sales trends of different products. The findings can help evaluate the effectiveness of current sales strategies and identify any necessary adjustments to boost overall sales performance.

  question:
  1. What is the number of sales made each time of the day per weekday?
  2. Which of the customer types brings the most revenue?
  3. Which city has the largest tax percentage/ VAT (Value Added Tax)?
  4. Which customer type pays the most in VAT?

3. Customer
  This analysis seeks to identify distinct customer segments, examine their purchasing patterns, and evaluate the profitability associated with each segment.

  question:
  1. How many unique customer types does the data have?
  2. How many unique payment methods does the data have?
  3. What is the most common customer type?
  4. Which customer type buys the most?
  5. What is the gender of most of the customers?
  6. What is the gender distribution per branch?
  7. Which time of the day do customers give the most ratings?
  8. Which time of the day do customers give the most ratings per branch?
  9. Which day of the week has the best average ratings?
  10. Which day of the week has the best average ratings per branch?

Steps in this analysis:

1. Data cleaning
   - make sure NULL values and missing values are detected and data replacement methods are used to replace missing or NULL values.

2. Feature engineering:
   - Add a new column named time_of_day to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.
   - Add a new column named day_name that contains the extracted days of the week on which the given transaction took place (Mon, Tue, Wed, Thur, Fri). This will help answer the question on which week of the day each branch is busiest.
   - Add a new column named month_name that contains the extracted months of the year on which the given transaction took place (Jan, Feb, Mar). Help determine which month of the year has the most sales and profit.
