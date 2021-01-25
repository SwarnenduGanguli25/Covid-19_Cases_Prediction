# Covid-19_Cases_Prediction
### *PART-1*:
We have applied (K-Nearest Neighbors) model for the prediction.
<br>
For, Covid Cases prediction, we first analyzed the data and performed some feature engineering techniques(Imputing NULL values, standardization of non-categorical columns and one-hot encoding). Then, we applied some ML models like KNN Regression, Decision Tree Regression, Random Forest Regression, SVM Regression and Stacking Regression and calculated the R-2 score for each of these models. The best R-2 score was given by our KNN Model(0.77). So, we used this model for prediction of our Covid Cases. This basically happened because this is a distance-based algorithm and since we have already standardized the columns before so it was not impacted by the outliers.

### *PART-2*:
We have used ARIMA(AutoRegressive Integrated Moving Average) model for the prediction with R-2 score(0.9).
<br>
For Foreign Visitors Time series prediction, we first imputed the NULL values in our months column. Then, we checked for the stationarity of the Time Series by using Plotting Rolling Statistics and Dickey-Fuller Test. By this we came to conclusion, that our Time Series is not stationary and the reason behind this is TREND. For removing the TREND, we checked with various techniques like Log Scale Transform, Moving Average, Exponentially weighted moving average and Differencing. Then, we used Autocorrelation Function(ACF) & Partial Autocorrelation Function(PACF) to find the p and q to be used in our ARIMA Model.
