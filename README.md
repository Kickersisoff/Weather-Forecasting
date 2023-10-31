# Efficient AI-Based Weather Forecasting using Field Data

In order to increase the precision of the forecast of Shenzhen weather features, a long short-term memory (LSTM) neural network was employed for the daily weather forecast in Shenzhen. This model took advantage of the LSTM model's advantages in time-series data processing.The experimental findings demonstrate that our EMD-LSTM model design outperforms conventional models in terms of forecasting precision and efficiency, which offers fresh approaches to weather forecasting.

🚩: We are Initially utilising ARIMA and then we aim to utilize the combined work by (Haoyi Zhou, Shanghang Zhang, Jieqi Peng, Shuai Zhang, Jianxin Li, Hui Xiong, Wancai Zhang) in Informer forecasting model:Beyond Efficient Transformer for Long Sequence Time-Series Forecasting.

<img src="https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/768e16ae-8a7f-4e43-b7ad-0b9ff80b556e" width="600" height="200">

Figure 1. An example of training dataset

<img src="https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/6b4fd649-c8f7-4a32-b24f-a89bb1a84490" width="500" height="300">

Figure 2. Line plot for Target Variable

#### Informer Model
Informer is an upgraded version of the Transformer model that maintains a larger prediction capacity while being more efficient in terms of architecture, memory usage, and computation. There are several severe issues with Transformer that prevent it from being directly applicable to LSTF (Long sequence Time series forecasting), including quadratic time complexity, high memory usage, and inherent limitation of the encoder-decoder architecture.

<img src="https://github.com/Kickersisoff/Oil-Well-Production-Optimization/assets/34878344/e1fe6725-109e-432f-885b-7e810ebabfa5" width="400" height="300">

Figure 2. The architecture of Informer model.

Requirements
* Python 3.6
* matplotlib == 3.1.1
* numpy == 1.19.4
* pandas == 0.25.1
* scikit_learn == 0.21.3
* torch == 1.8.0

<img src="https://github.com/Kickersisoff/Weather-Forecasting/assets/34878344/d6905844-031f-4651-b6f5-938165ab30cb" width="600" height="300">


Figure 5. Multivariate forecasting results (for 96 days).

🚩: Find the research report here - https://drive.google.com/file/d/1fwwCZzIIfk6Hiip40Z6bgMQQZSp9eS_J/view?usp=sharing
