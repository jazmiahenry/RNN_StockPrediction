# RNN_StockPrediction

## Model
This is an improvement on my SNP Market Over Time project found here: 
https://github.com/jazmiahenry/SNPMarketOverTime. 

In this project, I take a deep learning approach to examining SNP market values over time, and compare actual and predicted market values for Q1 and Q2 in of 2020 to make a more robust and informative predictive model. My analysis is able to identify the effect of COVID19 on SNP performance during the first half of this year. 

Due to the strength of recurrent neural networks to process sequential data, I have created a stock prediction model using RNNs. 

The prediction model training dataset is the daily market values of the *SNP from March 9th, 2009- "rock bottom" of the 2008 financial crisis and the lowest close of the SNP since since September 12, 1996.(https://money.cnn.com/2009/03/09/markets/markets_newyork/)

#### Train Data

<img width="647" alt="traindata" src="https://user-images.githubusercontent.com/48301423/88071575-0297bc00-cb42-11ea-86d8-d09e55c3f06d.png">

>*designated by the ^GSPC ticker. 

The test dataseet is the Year-to-Date daily market values of the SNP in 2020.**

#### Test Data

<img width="647" alt="testdata" src="https://user-images.githubusercontent.com/48301423/88071355-b51b4f00-cb41-11ea-9f45-5b9d5dc9d09b.png">

>**The data was downloaded from Yahoo Finance.

## LSTM Algorithm

    To account for unknown lags in the data, I used the LSTM algorithm to process the data. 
    The LSTM algorithm is composed of four parts:
    1. Cell
    2. Input Gate
    3. Output Gate
    4. Forget Gate

![lstm](https://user-images.githubusercontent.com/48301423/87892868-48eaff00-ca0c-11ea-8785-90c41b046bef.png)


>*LSTM Diagram*


LSTMs improve sequential processing and accounting for the vanishing gradient problem prevalent in back propagation by passing through relevant information and "forgetting" nonrelevant information. Information is stored within the cell and the gates either block or allow information through while back propagating error and adjusting weights through gradient descent. 

* Read more on LSTMs here: https://pathmind.com/wiki/lstm#long

## Plot
<img width="1050" alt="snppredict" src="https://user-images.githubusercontent.com/48301423/88070193-691bda80-cb40-11ea-921d-2fe7f04a802a.png">

>*Plot of SNP Predicted vs. Actual Values*
