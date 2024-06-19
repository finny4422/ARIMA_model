CARBON-PRICING
Carbon Pricing effectively shifts the responsibility of paying for the damages of climate change from the public to the GHG emission producers.  
This gives producers the option of either reducing their emissions to avoid paying a high price or continue emitting but having to pay for their emissions. 


ARIMA 
ARIMA stands for AutoRegressive Integrated Moving Average. It is a statistical tool which is used for time series data for analysing and prediction of future trends. To apply ARIMA effectively the dataset needs to be made stationary by differencing the data

ARIMA has 3 parameters : p,d,q

p : the number of lag observations in the model, also known as the lag order. d : the number of times the raw observations are differenced to make ; also known as the degree of differencing. q : the size of the moving average window, also known as the order of the moving average. We import the model. We are trying to predict the future trends for China and India and knowing that China has implemented Carbon Pricing while India has not, we expect China to perform better. As the absolute values for China are much larger owing to the country size, we need to normalise the values. For the purpose of normalisation, I have used population values from 1990 to 2019 for both India and China and saved them in CSV files(uploaded in the main branch). Any other relevant normalising factor can also be used, for example area of the country.

We divide the values. To apply ARIMA model we need p value below 0.05, initially the dataset gives p value as 0.94, as it is not differenced. On differencing twice we get an optimal value of p and so d value is 2 (this step has not been shown in the final code as we are concerned with this step only to get d value). We run the model for both the countries, plot and compare the predictions


ADFULLER hypothesis
The ADF (Augmented Dickey-Fuller) test is used to see if a time series is stationary. Here's how to interpret the results: The Hypothesis: The test has a null hypothesis that the data has a unit root, which means it's not stationary. The alternative hypothesis is that the data is stationary or trend-stationary.
