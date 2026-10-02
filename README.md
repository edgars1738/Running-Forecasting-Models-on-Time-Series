# Running-Forecasting-Models-on-Time-Series

## This assignment was done using the US Total Vehicle Sales data set

## Models Run throughout the assignment:
- Mean - The mean model forecasts future TOTALSA values using the average of all historical observations. Because the forecast is based on the historical mean, the forecast remains relatively constant across the future periods.
- Naive - The naive model uses the most recent TOTALSA observation as the forecast for all future periods. This means the forecast does not change over the forecast horizon.
- Random Walk with Drift - The random walk with drift uses the most recent observation while also incorporating the overall historical direction of the series. Therefore, the forecast can increase or decrease over time rather than remaining constant.
- Seasonal Naive - The seasonal naive model uses the observation from the same month in the previous year. Since TOTALSA is monthly data, the seasonal period is 12 months. This allows the model to account for repeating seasonal patterns.
- Moving Average 5 & 9 - The moving average smooths the TOTALSA time series by averaging observations over a specified number of periods. This helps reduce short-term fluctuations and makes the underlying pattern easier to observe.

## Mean Absolute Error (MAE) Accuracy Measure
- MAE measures how far the forecast was from the actual value on average. The lower/closer to 0 the MAE is, the more accurate the forecast is
- The best model with the lowest MAE for this assignment was the Random Walk with Drift with a 0.57 MAE
