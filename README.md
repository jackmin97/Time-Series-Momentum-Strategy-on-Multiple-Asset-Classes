# Time-Series-Momentum-Strategy-on-Multiple-Asset-Classes
In this notebook, we will code and analyse a time series momentum strategy across multiple asset classes. We will use lookback period of 12 months and holding period of 1 month.
In time series momentum, we look at the past performance of financial instruments over time. If the financial instruments perform well in the past, we will buy; otherwise, we will sell.

### 1. Read prices from CSV file
First, we will import the necessary libraries and then, we will read the csv file with the different security prices using the 'read_csv' method of pandas.

### 2. Calculate strategy returns
We create a new function called get_ts_mom_strategy_returns function and pass data, lookback period and holding period as parameters. In the function, we calculate the strategy returns.

### 3. Analyse strategy performance
We create a new function, analytics_returns and pass strategy returns as a parameter to calculate Sharpe ratio, annualised returns, annualised volatility and maximum drawdown. Here, we will create an equal-weighted portfolio where we will allocate equal weight to each security in a particular class.

#### Store securities according to their classes

As we can observe, the time series momentum fails for most of the securities. The possible reasons for this failure could be:
1. Time series under observation might not be trending
2. 12 months and 1 month might not be the optimal lookback and holding period for all securities.
