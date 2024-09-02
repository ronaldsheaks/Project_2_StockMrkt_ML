# Project_2_StockMrkt_ML
OSU AI Bootcamp - Stock Market - ML - Ryan and Ronald


# Project Overview

The goal of this project is to develop a machine learning model that analyzes stock market data to uncover trends and insights. This project leverages historical data from 2020-2024 to better understand market behavior during significant periods, such as the COVID-19 pandemic and the subsequent recovery.

# Questions/Topic

1. Which machine learning algorithms are best suited for predicting stock price movements based on historical data?

2. How can we use feature engineering to enhance the predictive power of our model?

3. What is the most effective way to handle missing or noisy data in our dataset?

4. How can we evaluate the performance of our model, and which metrics should we use?

5. Can the model generalize well to unseen data, and how can we prevent overfitting?

# data sources

[Alpha Vantage API](https://www.alphavantage.co/support/#api-key)

# files
[IT_SECTOR_2020_24](https://github.com/ronaldsheaks/Project_2_StockMrkt_ML/tree/main/ALL_STOCKMARKET_DATA_2020_24/IT_SECTOR_2020_24)



# notes 
**Wednesday, August 28th - Post Class

Added stockapi.env to the repo with the associated Alpha Vantage API Key as ALPHA_VANTAGE_API_KEY=

Created AlphaVantage_Historical_StockData_APIcall_2020_24.ipynb which calls the AlphaVantage API for Historical Stock Data

Used AlphaVantage_Historical_StockData_APIcall_2020_24.ipynb notebook to output the AAPL_2020_2024.csv, AMZN_2020_2024.csv, and GOOGL_2020_2024.csv, respectively, and output to the the "Historical Stock Data CSV" folder

Pushed changes

**Thursday, August 29th

Created Preliminary Folder Structure for Stock Market Data by Sub-Sector and Year(Covid/Post-Covid), for the Yearspan of 2020-2024

Developed an Idea for a Stock Data API Call Workflow, using a Pipeline

Created a Stock Market Alpha Vantage API Call Pipeline for Downloading Stock Market Data/Symbols by Stock Market Sub-Sector as .csv extensions in the "ALL_STOCKMARKET_DATA_2020_24" Folder

Pushed changes

Next Steps: SWOT, AI Risk Analysis, PMP: Workflow, Assignments

Concatenated IT_SECTOR Data, with Ticker Symbols, did SWOT

**Friday, August 29th

Calculated Moving, Added Column with Stats

Scaled Data with Standard Scaler

Added PROJECT_MANAGEMENT to root

Added SWOT, PMP, and INSTRUCTOR_NOTES .txt





