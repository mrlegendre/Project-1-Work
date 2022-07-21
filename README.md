# Group 3

# Profolio Analysis, Major Indices vs High Risk ETFs (Traditional/Crypto)

We will be investigating into 2 Large MarketCap ETF's and benchmark their performance against Nasdaq and SP500.

The choice of ETF's are ARK Innovation ETF (ARKK), 9 Billion MCap, profolio focus is in high potential future looking technologies. Second ETF we will be investigating into is Grayscale Bitcoin Trust (GBTC), 8 Billion Mcap, this is a crypto currencies only investment.

Both of the choosen ETFs are in the higher risk category, it will be very interesting to look at the calculated result between a traditional riskier profolio and a emerging crypto currency profolio compares and obviously summing up with the potential returns comparing to big indices like SP500 and Nasdaq. 

## 1. Introduction
To investigate the portfolio we ran different tests in python. First test was to clean the data and calculate daily returns. To have a better understanding of the data we created a visual plot by installing bokeh library. Bokeh is a Python library which allows to create interactive visualizations ranging from simple plots to complex dashboards. Compared to Matplotlib, Bokeh allows to create many sophisticated plots with fewer lines of code and have higher resolution. Below are the interactive timeseries charts created using the Bokeh library

![](/Resources/Major_Indices.png)

![](/Resources/ETF's.png)

![](/Resources/ETF's_vs_indices.png)

![](/Resources/Daily_returns.png)


## 2. James

## 3. Beta Analysis and Correlation
The rolling 30 day Beta anlysis with both NASDAQ and S&P500 show that the GBTC generally swings more than positive and negative 1 which indicates it is NOT strongly correlated with either markets at all.

### Rolling 30-Day Beta wrt NASDAQ of GBTC & ARKK ETFs
![](/Resources/Rolling30dayETFvsNASDAQ.png)

### Rolling 30-Day Beta wrt S&P500 of GBTC & ARKK ETFs
![](/Resources/Rolling30dayETFvsSP500.png)

When comparing the rolling 30 day Beta values for ARKK we notice that for both NASDAQ and S&P500 it generally stays at 1 or just above indicating a strong correlation with the markets.  

One instance of interest is where the value of Beta for ARKK follows closely with GBTC indicating a negative Beta is at the end of 2020/beginning of 2021 with respect to the S&P500.

This illustrates a stronger correlation with ARKK and GBTC to the NASDAQ (and tech stocks in general) than to the S&P500

## Linear Regression, Beta vs. Correlation

GBTC generally has a **weak positive correlation**, or almost none at all ot either NASDAQ or S&P500.  Although the returns are can be vast (big or small) the correlation an/or predictability of GBTC with respect to the markets is difficult to 

### GBTC correlation wrt NASDAQ
![](/Resources/GBTC-NDQ-LinearRegression.png)


### GBTC correlation wrt S&P500
![](/Resources/GBTC-SP500-LinearRegression.png)



ARKK has a **strong positive correlation** to both the NASDAQ and S&P500, but more so to the NASDAQ as can be illustrated by 'less of a scatter' in it's plot with respect to the NASDAQ.

### ARKK correlation wrt NASDAQ
![](/Resources/ARKK-NDQ-LinearRegression.png)


### ARKK correlation wrt S&P500
![](/Resources/ARKK-NDQ-LinearRegression.png)


The variance of the NASDAQ for the period of data taken was 0.00019043096387163434
The variance of the S&P500 for the period of data taken was 0.00013977358029211093

The Beta value of GBTC with respect to NASDAQ 0.9812143096130634
The Beta value of ARKK with respect to NASDAQ 1.377983639468541

The Beta value of GBTC with respect to S&P500 1.0224393152281361
The Beta value of ARKK with respect to S&P500 1.3668171105674543

Even though visually the Beta value swings much more for GBTC.  It's overall Beta value is more consistent with markets than that of ARKK for the period studied.


## 4. Monte Carlo Analysis

We have conducted 3 Monte Carlo simulation with 3 different profolio configuration of $15,000

1. Even distributed, 25% SP500 / 25% Nasdaq / 25% ARKK / 25% GBTC
2. Majority ARKK, 70% ARKK / 10% SP500 / 10% Nasdaq / 10% GBTC
3. Majority GBTC, 70% GBTC / 10% SP500 / 10% Nasdaq / 10% ARKK

###### Evenly Distributed

![](/Resources/M-1-1.jpg)
![](/Resources/M-1-2.jpg)
There is a 95% chance that an initial investment of $15,000 in the portfolio over the next 3 years will end within in the range of $14070.82 and $71855.74.

###### Majority ARKK

![](/Resources/M-2-1.jpg)
![](/Resources/M-2-2.jpg)
There is a 95% chance that an initial investment of $15,000 in the portfolio over the next 3 years will end within in the range of $7053.55 and $64072.11.

###### Majority GBTC

![](/Resources/M-3-1.jpg)
![](/Resources/M-3-2.jpg)
There is a 95% chance that an initial investment of $15,000 in the portfolio over the next 3 years will end within in the range of $3786.28 and $322990.18.

Result Table
        Even        ARKK        GBTC
Low     14070.82    7053.55     3786.28
High    71855.74    64072.11    322990.18


## Conclusion / Final Observation

1st: It appears a balanced profolio will net you the lowest risk
 
2nd: If you are adventurious investing into crypto will have a might higher potential in comparison to Tech Stocks
