# RNN_StockPrediction

## Model
This is an improvement on my SNP Market Over Time project found here: 
https://github.com/jazmiahenry/SNPMarketOverTime. 

In this project, I take a deep learning approach to examining SNP market values over time, and compare actual and predicted market values for Q1 and Q@. of 2020 to make a more robust and informative predictive model.

Due to the strength of recurrent neural networks to process sequential data, I have created a stock prediction model using RNNs. The prediction model training dataset is the daily market values of the *SNP from March 9th, 2009- "rock bottom" of the 2008 financial crisis and the lowest close of the SNP since since September 12, 1996.(https://money.cnn.com/2009/03/09/markets/markets_newyork/)

>*designated by the ^GSPC ticker. 

The test dataseet is the Year-to-Date daily market values of the SNP in 2020.**

>**The data was downloaded from Yahoo Finance.

To account for unknown lages in the data, I used the LSTM algorithm to process the data. 
![lstm](https://user-images.githubusercontent.com/48301423/87892868-48eaff00-ca0c-11ea-8785-90c41b046bef.png)

>*LSTM Diagram*

## Plot
<img width="1050" alt="snppredict" src="https://user-images.githubusercontent.com/48301423/88070193-691bda80-cb40-11ea-921d-2fe7f04a802a.png">

>*Plot of SNP Predicted vs. Actual Values*
