# Unit 10 - Time Series Analysis

In this assignment, we have tested some time series tools that we previously learned in order to predict future movements in the value of the Canadian dollar versus the Japanese yen. In the first part of the assignment we applied the following tools:

1. Hodrick-Prescott Filter
We identified 3 patterns using the Hodrick-Prescott filter; 
- The first pattern is a constant decline from 2015 to 2017. There are some peaks, but overall its a continuous decline.
- The second pattern between 2017 and 2020 is a more stable pattern, it too has peaks and dips, but not as significant.
- And then the third pattern sees another sharp decline, and a start to stabilize or move upwards.

2. ARMA Model
The ARMA model was inconsistent and maybe not the best fit per our results.

3. ARIMA Model
The ARIMA model helped to forecast a 5-day price run for Yen in the near future, also the AIC and BIC variables were lower in comparison to the ARMA model indicating that ARIMA was a better model.

4. GARCH Model
The GARCH model helped in forecasting the volatility of teh Yen, plus the p-values for GARCH and volatility forecasts tend to be much lower than our ARMA/ARIMA return and price forecasts. In particular, here we have all p-values of less than 0.05, except for alpha(2), indicating overall a much better model performance. In practice, in financial markets, it's easier to forecast volatility than it is to forecast returns or prices.

In the second prt of the assignment we applied the following tools:

1. Scikit-Learn linear regression model to predict CAD/JPY returns with lagged CAD/JPY futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects)

In this part of teh assignment we evaluated the model using out-of-sample and in-sample data. The results were as such:

Out-of-Sample Root Mean Squared Error (RMSE): 0.6445805658569028
In-sample Root Mean Squared Error (RMSE): 0.841994632894117

Since the RMSE for out-of-sample data is lower than the RMSE for the in-sample data which implies that the model performs better on the out-of-sample data.
