# timeseries
Kaggle Time Series Competition - Completed Notebook

(Available on Kaggle here - better option than GitHub as the links still work: https://www.kaggle.com/code/johncbaldwin/time-series-nb/)


In this notebook, I create a predictive model to predict sales for a Kaggle competition about predicting sales for a chain of grocery stores in Ecuador: https://www.kaggle.com/competitions/store-sales-time-series-forecasting/overview

The competition consists time series of 36 categories of items between 54 stores, for a total of around 2000 individual time series data streams.  I chose one of those data streams and built a progressively more complicated predictive model to increase accuracy.  After I created my final model on one data stream, I expanded the exercise to create models for each of the 2000 data streams and predict sales for each.

My modeling on the individual data stream improved accuracy by 42% over the baseline of predicting the mean, and my final model scored in the 50th percentile (exactly average) and took about 15 minutes to train.  This was especially impressive given I used only basic models in my design (hybrid of OLS and Random Forest)

I tried the following models for my individual data stream before expanding to the full dataset:
- ARMA with and without covariates
- OLS with progressively more covariates
- Hybrid of OLS and Random Forest on the residuals
