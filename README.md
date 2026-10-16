# Running-Forecasting-Models-on-Time-Series

## This assignment was done using the US Total Vehicle Sales data set

## Models Run throughout the assignment:
- Mean - The mean model predicts future vehicle sales using the average of all historical observations. This provides a baseline forecast but does not account for changes in trend or seasonality.
- Naive - The naive model uses the most recent vehicle sales value to predict all future months. It assumes sales will remain at the latest observed level
- Random Walk with Drift - The random walk with drift model uses the latest observation and the average historical change to forecast future vehicle sales. It accounts for an overall upward or downward trend.
- Seasonal Naive - The seasonal naive model predicts future vehicle sales using the values from the same months in the previous year. This is useful for TOTALNSA because vehicle sales may follow recurring seasonal patterns.
- Moving Average 5 & 9 - The five-month and nine-month moving averages smooth fluctuations in vehicle sales. The five-month average responds more quickly to changes, while the nine-month average produces a smoother trend.
- ETS - The ETS model automatically selects an exponential smoothing method based on the historical data. Its forecast uses the selected level, trend, and seasonal components to predict future vehicle sales.
- Holt-Winters - The Holt-Winters model uses exponential smoothing to estimate the level, trend, and seasonal patterns in vehicle sales. Its forecast extends these estimated patterns into the next 12 months.

## The model outputs display the forecasted vehicle sales for the next 12 months, along with prediction intervals for the forecasting models. Comparing the results shows how each method produces different forecasts based on its assumptions about historical averages, recent values, trends, and seasonal patterns. These outputs help evaluate how the models interpret the TOTALNSA data and predict future vehicle sales.

## The combined chart compares the historical TOTALNSA data with forecasts from the different models. Each colored line represents a model's predictions for the next 12 months. Differences between the forecast lines show how the models interpret historical vehicle sales differently, particularly in terms of trends and seasonal patterns. This chart provides a visual comparison of the models, while the accuracy measures are used to determine which model performs best.

## Mean Absolute Error (MAE) Accuracy Measure
- MAE measures how far the forecast was from the actual value on average. A lower MAE indicates that a model's forecasts were closer to the actual values, while a higher MAE indicates larger forecasting errors.
- Based on the MAE comparison, the Holt-Winters model performed best, with an MAE of 0.4066513. This means that its forecast had the lowest MAE among the models evaluated. Therefore, this model is the best forecasting method for TOTALNSA based on its test-period accuracy.
