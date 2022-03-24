# Purpose

The purpose of this project is to project the next 36 months of weekly sales using historical weekly sales.

I hope these time series models I built will be handy during the valuation stage as the models can quickly provide an overview on whether the sales will be trendy upward or downward in the next few years. The models can also be used during the post-integration stage, to monitor each acquired company's sales. 

# Key Findings

This project was one of the past competitions I found on Kaggle which the instruction is to project sales data for 45 Walmart stores located in different regions. Some of the key findings I found:

- dept, size, month, and week all have a perfect positive relationship with the response variable - Weekly Sales 
- unemployment,  store, CPI all have a perfect negative relationship with the response variable - Weekly Sales 
- temperature and fuel price have no relationship with the response variable - Weekly Sales
![correlation matrix](https://github.com/qinggao68/Project-2-Sales-Forecasting/blob/main/correlation_matrix.PNG)
- in the past three years, the top 10 stores that contributed to the most average weekly sales in Walmart are: stores 4, 20, 13, 2, 14, 10, 27, 39, 1, and 6
  - store #19 dropped in the top ten stores rank in 2011 and 2022 and store #39 climbed up to the top ten stores rank 
![top ten stores in avg wkly sales](https://github.com/qinggao68/Project-2-Sales-Forecasting/blob/main/Top_Ten_Stores_with_Highest_avg_Weekly_Sales_2010_2012.PNG)
- in the past three years, the top 10 departments that contributed to the most average weekly sales in Walmart are: depts 92, 95, 38, 65, 90, 40, 72, 2, 91, 94 
![top ten depts in avg wkly sales](https://github.com/qinggao68/Project-2-Sales-Forecasting/blob/main/Top_Ten_Departs_with_highest_avg_weekly_sales_2010_2012.PNG)
- store type A is the largest, followed by type B, and type C
![stores types proportion](https://github.com/qinggao68/Project-2-Sales-Forecasting/blob/main/types_of_stores_proportion.PNG)
- there is a significant increase in weekly sales in November and December, other months' weekly sales are relatively constant 
![wkly sales in 2010 to 2012](https://github.com/qinggao68/Project-2-Sales-Forecasting/blob/main/total_weekly_sales_in_2010_2012.PNG)
- final model - STL-ARIMA has the lowest WMAE with a score of 1454.388  
![final model - STL ARIMA](https://github.com/qinggao68/Project-2-Sales-Forecasting/blob/main/stl_arima_result.PNG)

# Additional Information 
Please access the R markdown provided below to view the full analysis.   

# Project Scope 
1. Examine the data sets provided and check to see if there are any missing values 
2. Create data visualization for each predictor and compare it to the response variable - weekly sales 
3. Create a correlation matrix 
4. Convert irregular time series to regular time series 
5. Convert to multiple time series 
6. Interpolation 
7. Split data into train and validate 
8. Build a Simple Exponential Smoothing model 
9. Build a Holt's Trend model 
10. Build a Seasonal Naive Forecast model 
11. Build a Linear Model with Time Series Components 
12. Build a TBATS Forecast model 
13. Build a Seasonal & Trend Decomposition - ETS model 
14. Build a Seasonal & Trend Decomposition - ARIMA model 
15. Make holidays adjustment

# Future Work 
I might display the visualization on the Shiny server. 

# Reference
[Caio Avelino's Kaggle Notebook done using Python] https://www.kaggle.com/code/avelinocaio/walmart-store-sales-forecasting
[Yasir Hussain's Kaggle Notebook done using Python] 
https://www.kaggle.com/code/yasirhussain1987/eda-and-store-sales-predictions-using-xgb
