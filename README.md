SWPPX Stock Price Forecast Using LSTM

Overview:
This project aims to forecast the stock price of the SWPPX (Schwab S&P 500 Index Fund) using a Long Short-Term Memory (LSTM) neural network. The dataset consists of historical SWPPX closing prices over time.

Dataset:
The dataset comprises historical SWPPX closing prices stored in a CSV file. Each row contains the date and the corresponding closing price of SWPPX. The data is preprocessed and indexed by date for time-series analysis.

Model:
An LSTM model is implemented using TensorFlow's Keras API. The model architecture includes LSTM layers, dense layers, and other recurrent layers. The goal is to capture temporal dependencies in the stock price data to make accurate forecasts.

Training:
The dataset is split into training and testing sets. Time-series data preprocessing techniques are applied, such as scaling and creating time windows. The model is trained using the Adam optimizer with mean absolute error (MAE) as the loss function. Early stopping is utilized to prevent overfitting during training.

Results:
The trained model successfully predicts future SWPPX stock prices with reasonable accuracy. The Mean Absolute Error (MAE) is calculated to evaluate the model's performance, providing insights into the forecast's reliability. Importantly, the relative MAE of the LSTM model, 6%, significantly outperforms a simple linear regression prediction, 25%, demonstrating the effectiveness of LSTM in capturing the complexities of the SWPPX stock price dynamics. Additionally, a forecast for the next year has been generated, and its accuracy will be evaluated in the future.

Usage:
To use this forecast model:

Download the provided Jupyter notebook (SWPPX_Forecast.ipynb) and the SWPPX dataset (SWPPX.csv).
Run the notebook on platforms such as Google Colab or locally with TensorFlow and Keras installed.
Follow the instructions in the notebook to preprocess the data, train the LSTM model, and make forecasts.
Adjust hyperparameters or model architecture as needed for further experimentation.
This project demonstrates the potential of LSTM neural networks in forecasting stock prices, providing valuable insights for investors and financial analysts interested in predicting SWPPX's future performance. Additionally, the forecast for the next year will allow us to evaluate the model's accuracy over longer time horizons.
