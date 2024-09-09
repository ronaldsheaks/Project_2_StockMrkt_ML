# Project_2_StockMrkt_ML
OSU AI Bootcamp_Project 2 - Stock Market - ML - Ryan and Ronald


# Project Overview

The goal of this project is to develop a machine learning model that analyzes stock market data to uncover trends and insights. This project leverages historical data of Stock Market Sectors/Sub-Sectors from 2020-2024 to better understand market behavior during significant periods, such as the COVID-19 pandemic and the subsequent recovery.

# Questions/Topic

***1. Which machine learning algorithms are best suited for predicting stock price movements based on historical data?

**Logistic Regression: 

Since we've already calculated the percentage change as a binary (representing if the stock will go up or down), Logistic Regression is a straightforward choice. It's particularly useful for binary classification problems and will help us understand the relationship between our features (e.g., moving averages) and the binary target.

**Support Vector Machines (SVM): 

SVMs are good for classification tasks, especially when the data isn't linearly separable. They can capture more complex relationships in our data, especially if we use kernel tricks (like the RBF kernel). SVMs might give us a more nuanced decision boundary compared to Logistic Regression.

**Random Forest: 

This is an ensemble method that works well for classification tasks and can handle a large number of features. It’s robust to overfitting, especially with a lot of data, and can give us insights into feature importance, which is useful for understanding what drives stock price changes.

**K-Nearest Neighbors (KNN): 

KNN is a non-parametric method that could be useful as a baseline model. It’s simple and effective for small datasets, though it can be computationally expensive with larger ones. It might not perform as well as other models but could provide a good comparison point.

**Gradient Boosting Machines (GBM) or XGBoost: 

These are more advanced ensemble techniques that often perform well in predictive tasks. They build models iteratively, correcting the mistakes of previous models, which can lead to high accuracy.

***2. How can we use feature engineering to enhance the predictive power of our model?

We could add more features. We can also include technical indicators like RSI, Bollinger Bands, or MACD.

***3. What is the most effective way to handle missing or noisy data in our dataset?

So far there are no null values. There are however blank datasets for some stock symbols, for whatever reason, which we can completely omit. This will require manually assessing the data folders and deleting these components. 

***4. How can we evaluate the performance of our model, and which metrics should we use?

After training, we evaluate our models using metrics like accuracy, precision, recall, F1 score, and ROC-AUC, depending on what we find most relevant. Cross-validation can also be a good technique to ensure our model generalizes well.

***5. Can the model generalize well to unseen data, and how can we prevent overfitting?

Hyperparameter Tuning: We can use techniques like Grid Search or Random Search to optimize the hyperparameters of your models, particularly for SVMs, Random Forest, and Gradient Boosting models.(Maybe, not sure about this one, research further)


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

Calculated Moving Average, Added Column with Stats, Percentage Change

Scaled Data with Standard Scaler

Added PROJECT_MANAGEMENT to root

Added SWOT, PMP, and INSTRUCTOR_NOTES .txt

**Sunday, September 1st

Continued downloading stock data via API

**Monday, September 2nd (Labor Day)

Continued downloading stock data via API

Tried to answer proposed Questions/Topic section

Organized Git Repo(Need to add files above)

Moral Support

**Wednesday, September 3rd 

Updated Instructor Notes

Worked in parralel to calculate MA, Percent Change

Created Binaries for Percent Change, Ticker, and Sub-sector, as well as Date Format.

Worked in parralel to analyze Technical Indicators

Graph code is in the Jupyter Notebook folder

Graphical outputs exported to the DATA_OUTPUTS, GRAPHS_CHARTS, TECHNICAL_OUTPUTS Folder





