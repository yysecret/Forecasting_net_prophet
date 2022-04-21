# Forecasting_net_prophet

In google colab, this assigment analyzed the unusual patterns and the seasonality of Google search traffic for MercodoLibre and its correlations to the stock prices using Python libraries pandas and hvplot. A time series model was created by using Prophet and the revenue was forecasted by the time series model. 

## Step 1: Find unusual patterns in hourly Google search traffic.

By calculating the total search traffic for May 2020 and then compare the value to the monthly median across all months. We found that the the Google search traffic increased during the month that Mercadolibre released its financial results. The overall monthly median search traffic value is 35172.5, while the search traffic value is 38181 during May 2020.

## Step 2: Mine the search traffic data for seasonality.

1. By grouping and plotting the search traffic data by the days of the week, we found that the search trends are higher at he begining of the week and graually fall at the weekend. Tuesday has the highest search traffic. 

2. By hvPlot, visualized this traffic as a heatmap, the day-of-week effect concentrates between 21:00 and 2:00 of that day.

3. By grouping the search data by the week of the year, we found that the search traffic trend increases from week 41 to week 50, but drops during week 51 and week 52. 

## Step 3: Relate the search traffic to stock price patterns.

1. By using hvplot to plot the search traffic and stock prices for the first half of 2020. Both time series indicate a common trend that market events emerged during the year of 2020 that many companies found difficult. But, after the initial shock to global financial markets, new customers and revenue increased for e-commerce platforms.

2. By reviewing correlation matrix of the time series, we found that here is no significant relationships exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns.

## Step 4: Create a time series model by using Prophet.

Using Facebook's Prophet to predict google search traffic for the end of 2020, we found that the predicted search trends will increase before October and then will decrease, and finally will go up at the end of the year. 

By plotting the individual time series components of the model, we know that midnight of the day exhibits the greatest popularity, Tuesday gets the most search traffic, and middle of October is the lowest point for search traffic in the calendar year. 

## Step 5: Forecast the revenue by using time series models.

By applying a Prophet model to dialy historical sales data and interpreting the model output, we found that Wednesdays are the peak revenue days. The most likely expected toal sales for the period of 5/15/2020 to 8/12/2020 is 969.58(million $), the best expected total sales is 1051.34 (million $), and the worst expected total sales is 887.91(million $).

