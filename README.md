# Microsoft Stock Time-Series Analysis

## Overview



## Business Problem

Investors, such as day traders and short-term investors, are actively involved in stock trading. They are interested in making informed trading decisions to capitalize on short-term price movements. Our challenge is to develop a predictive model that can forecast the direction of Microsoft stock prices over the next trading day.

## Data Understanding and Analysis

The dataset was obtained from Yahoo Finance and it consists of the date, opening price, maximum price, minimum price, closing price, adjusted closing price, and volume of the Microsoft stock. The data had been obtained from March 13, 1986 to December 26, 2023. The observations are collected during weekdays and not on weekends in accordance to the opening and closing of the New York Stock Exchange (NYSE). The dataset had 9524 observations.

We were concerned only with the closing stock price. Therefore, the master dataset was a Series that consisted of the date, which was used as index, and the closing price.

![MSFT_stock_price](Images/MSFT_close_price.png)

Looking at MSFT Closing Stock Price vs Date graph, we can see an upward trend in the last 9 years. Through the eye test, we can see that the data is not stationary. This was confirmed with a P-Value of 1.00 when Dickey-Fuller test was done.

![seasonal_decomposition](Images/trend.png)

Looking at these graphs, we can see the upward trend of MSFT stock price in the past 9 years. This year alone, MSFT stock price rose 55% under the leadership of CNN Business' CEO of the year, Satya Nadella.



## Modeling

### Baseline Model: Naive Model

Naive model is done based on our current data shifted by one step. In other words, we used values from last observation to forecast our future predictions.

### ARIMA Model


### Random Walk Model


### LSTM Model

## Recommendations

- **Upward Trend**

Based on our analysis, MSFT stock price has an upward trend since 2016, which 

- **LSTM MOdel Predictions**


## Future Insights

- **External Factors**

- **Real-Time Forecasting**

For day traders, decisions need to be made on site and in real-time. Therefore, further research needs to be done for an application to give them forecasting in real-time to make decisions at the moment.

- **Enhancing Model Robustness**


## Outside Research
- [Microsoft’s Satya Nadella is CNN Business’ CEO of the Year](https://www.cnn.com/2023/12/26/tech/satya-nadella-ceo-of-the-year/index.html)

- 

## Appendix

## Repository Structure

```bash

├── Data                                       <- Folder consisting dataset used in this project

├── Images                                     <- Folder consisting images used in this project

├── .gitignore                                 <- Contains list of files ignored from GitHub

├── Microsoft_Stock_Time_Series_Analysis.pdf   <- Slide Presentation of the project

├── README.md                                  <- Contains README file consisting summary of the project

└── microsoft_stock_analysis.ipynb             <- Jupyter notebook of the project containing codes and analysis