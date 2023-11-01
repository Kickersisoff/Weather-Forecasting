# Efficient AI-Based Weather Forecasting using Field Data

This experimental findings demonstrate that the EMD-LSTM model design outperforms conventional models (like RNN) in terms of forecasting precision and efficiency, which offers fresh approaches to weather forecasting.

🚩: We are utilising LSTM with Empirical mode decomposition(EMD) to engineer extra features and we aim to utilize the combined work by Guici Chen, Sijia Liu and Feng Jiang in DailyWeather Forecasting Based on Deep Learning Model: A Case Study of Shenzhen City, China.

🚩: Find the `Research Report` here - [Link](https://drive.google.com/file/d/18QjJG85U3vOnafZkZCHBxW3WJNVU3m-m/view?usp=drive_link)


### EMD-LSTM Model
All features are dependent on each other so we are taking all features in order to find one feature and then EMD that feature into IMF. Further we find the best correlation IMF using Pearson coefficient. We give input of all features along with the IMF and train the model on that to give that feature value as the output.

<p align="center">
<img src="https://github.com/Kickersisoff/Weather-Forecasting/assets/34878344/f2ee24b0-1801-46a2-b802-6b785890df8b" width="500" height="400">
<br><br>
<b>Figure 1.</b> AVGP and its IMF (Intrinsic mode function) values
</p>

<p align="center">
  <br><br>
<img src="https://github.com/Kickersisoff/Weather-Forecasting/assets/34878344/29c0010c-aec4-49d7-a945-b9293836736e" width="500" height="400">
<br><br>
<b>Figure 2.</b> IMF value and its pearson correlation (for average pressure, AVGP)
</p>

Requirements
* Python 3.10
* matplotlib 
* numpy
* pandas 
* tensorflow (including keras)
* EMD-signal

### Results

<p align="center">
  <br><br>
<img src="https://github.com/Kickersisoff/Weather-Forecasting/assets/34878344/d6905844-031f-4651-b6f5-938165ab30cb" width="600" height="300">
<br><br>
<b>Figure 3.</b> Future forecasting results for Average Pressure (14 days).
</p>
<p align="center">
 <br><br>
<img src="https://github.com/Kickersisoff/Weather-Forecasting/assets/34878344/b5e4b3c9-44a6-4de8-8c0e-26dc9950ef39" width="600" height="300">
<br><br>
<b>Figure 3.</b> Future forecasting results for Minimum Humidity (7 days).
</p>
</p>
<p align="center">
 <br><br>
<img src="https://github.com/Kickersisoff/Weather-Forecasting/assets/34878344/47339d1b-3464-4a4a-899b-2a35b67402be" width="600" height="300">
<br><br>
<b>Figure 3.</b> Future forecasting results for Average Temperature (7 days).
</p>
<p align="center">
 <br><br>
<img src="https://github.com/Kickersisoff/Weather-Forecasting/assets/34878344/36aa0799-98f4-484e-8c29-7579b649b9cf" width="600" height="300">
<br><br>
<b>Figure 3.</b> Future forecasting results for Minimum Pressure (7 days).
</p>

### What we Achieved
* Correctly predicted humidity, minimum pressure, maximum pressure, average pressure, maximum temperature, minimum temperature, average temperature, and wind speed with non-stationarity and seasonal fluctuations.
* Increased the precision and efficiency of the forecast compared to conventional methods (like RNN)
* Reduced the effect of data noise and seasonal changes by filtering the correlation coefficients of each variable that were decomposed by EMD and then putting the data back together in an LSTM network.

