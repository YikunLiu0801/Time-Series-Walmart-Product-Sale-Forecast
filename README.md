# [Time Series] Walmart Product Sale Forecast

This project is to estimate, as precisely as possible, the point forecasts of the 28 days unit sales of various products sold in the USA by Walmart. 

Cost Funtion: Weighted Root Mean Squared Scaled Error (RMSSE) of all 30490 products in the predicted 28 days.

## About the dataset
- The dataset involves the unit sales of various products sold in the USA, organized in the form of grouped time series. More specifically, the dataset involves the unit sales of 3,049 products, classified in 3 product categories (Hobbies, Foods, and Household) and 7 product departments, in which the above-mentioned categories are disaggregated. The products are sold across ten stores, located in three States (CA, TX, and WI). In this respect, the bottom-level of the hierarchy, i.e., product-store unit sales can be mapped across either product categories or geographical regions
- Besides the time series data, it includes explanatory variables such as sell prices, promotions, days of the week, and special events (e.g. Super Bowl, Valentine’s Day, and Orthodox Easter) that typically affect unit sales and could improve forecasting accuracy.

## Two ways to handle the problem
- Start from store-level sales and break down the sales into product level by calculated ratio. Less memory usage; simpler process; more commonly used in industry; less accurate.
- Handle product-level sales directly. More accurate; more complex and memory consuming.
