# stock-predictor 
## stock prediction app using prophet and yahoo finance

curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://35.163.200.64:8000/predict

### Algorithm Understanding
#### How does the Prophet Algorithm differ from an LSTM? Why does an LSTM have poor performance against ARIMA and Profit for Time Series?
The prophet algorithm is spefcifically designed to analyze time series data using statistical approach while the LSTM model is a neural network type model designed to improve on patterns/relationaships in sequential data.  LSTM requires a lot of data to learn the dependencies in the sequential data. Also, LSTM might be overfitting time series data that can be fit with simpler models. Last, LSTM requires careful hyperparameter selection which might render its prediction poor if not selected carefully. Hence,  lack of data, simple data and hyperparameter selection are the main reasons Prophet and ARIMA might predict better than LSTM.

### Interview Readiness
#### What is exponential smoothing and why is it used in Time Series Forecasting?
Exponential smoothing is used in time series forecasting to give more weight to recent data points. The weight given to each point decreases exponentially as the time points get older. This method is used in time series prediction because it is great in capturing seasonality and trends and is easy to implement.

### Interview Readiness
#### What is stationarity? What is seasonality? Why Is Stationarity Important in Time Series Forecasting?
Stationarity means that a time series data: mean, variance, & autocorrelation do not change over time. In contrast, seasonality refers to patterns that repeat in time series data at fixed intervals. Stationarity allows for data prediciton using simpler models like ARIMA and Prophet while seasonality requires more complicated models like LSTM.


### Interview Readiness
#### How is seasonality different from cyclicality? Fill in the blanks:
seasonality is predictable, whereas cyclicality is not.






