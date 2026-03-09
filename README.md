Monthly data on the U.S. Consumer Price Index (CPIAUCSL) were obtained from the Federal Reserve Economic Data (FRED) database and imported into Stata using the freduse command. The dataset covers the period 1947–2026. The date variable was converted to a monthly time format (mdate) and the dataset was declared as a time series using tsset.

A time-series graph of the CPI level was first plotted. The graph showed a strong upward trend over time, indicating that the price level has increased steadily in the United States. This visual pattern suggested that the CPI series is non-stationary, as it does not fluctuate around a constant mean.

To obtain a stationary measure of price changes, the CPI series was transformed. The natural logarithm of CPI was calculated (lcpi), and the first difference of the log was taken to construct the inflation rate. A graph of the inflation series showed fluctuations around a relatively stable level rather than a persistent trend.

An Augmented Dickey–Fuller (ADF) test was then conducted on the inflation series. The test statistic was far below the critical values and the p-value was effectively zero, leading to rejection of the null hypothesis of a unit root. This indicates that the inflation series is stationary.

Finally, a correlogram analysis was performed to examine the autocorrelation structure of inflation. The autocorrelation function (ACF) declined gradually across lags, while the partial autocorrelation function (PACF) showed a dominant spike at the first lag. This pattern suggests that the inflation series may follow an autoregressive process of order one, AR(1).
