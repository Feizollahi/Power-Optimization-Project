# Model 2 - Forecasting Electricity Prices

The project employs a Long Short-Term Memory (LSTM) algorithm to learn from training data, and forecast the Locational Based Marginal Prices (LBMPs) for a given test date. The lookback hyperparameter determines the extent of historical data that can be utilized by the model for making predictions. Additionally, the LSTM_alg() function allows users to configure the number of training epochs. 

# Requirements
- python 3.8.12
- numpy 1.20.3
- pandas 1.3.4
- matplotlib 3.5.0
- seaborn 0.11.2
- torch 1.10.1





## How to run:

The user needs to provide test_date, number of training days (num_train_days), time resolution (delta_t) and look back parameter in the main forecast algorithm. For example:
main_forecast_alg(test_date='2022-08-06',num_train_days=21,delta_t=60,lookback = 24)
	


The output of the method includes the predicted and actual LBMPs for both training and test intervals. Moreover, the method provides a comparison of the obtained results with the average LBMP for each time stamp in the dataset.
