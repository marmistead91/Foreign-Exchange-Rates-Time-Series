# Foreign Exchange Rates Time Series

## Background

The foreign exchange rate is based on the conversion of one coutries economy to anothers. Things that can factor into this are trade, economy, tourism and geo-political risk. Looking at the monthly exchange rates against the US dollar with other countries you can see when wars have broken out or economic calapes occured. After looking at the different countries I decided to try to preidct the foreign exchange between US and Australia. The main reason for this is becasue Australia has had the most consistent economy with the US, so hopefully we can come up with a good model for future predictions. 

## EDA

All of the countries were broken down by economic level so they are more digestable to look at. 
*graphs

## Forcasting

I used Dickey-Fuller tests to figure out the best way to make the data stationary. 
*graphs

Natrual log of the first difference was the most stationary

Using ARIMA model I looped through a list of parameters to determine what would be the best for p,d,q

Looking at Mean Squared Error and Absolute Mean Squared Error the best parameters were 1,0,0

I predicted the valuse from 5/2010 to 4/2020, graphing the predicted values to the actual values my predicted values was a constant slope and didn't look like the actual values. This happen when your data doesn't have strong seasonality and the model finds it difficult to predict the future, therefore it simply takes the average of the previous values and predicts it.

I went back to look at my seasonality for the data.
*graph

