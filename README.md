# Time-Series_Analysis_of_Covid-19_data using Prophet Package and ARIMA Model

## Tasks performed:

    - Scrape out the COVID-19 data from government website
    - Scrape out the COVID-19 from websites
    - Figure out the death rate and cure rate per 100 across the affected states
    - Create different charts to visualize the following:
        Age group distribution of affected patients
        Total sample test done till date
        Growth rate of COVID in top 15 states
        Top 10 States in each health facility
        State wise testing insight
    - Use Prophet to predict the confirmed cases in India
    - Use ARIMA to predict the confirmed cases in India
    - Compare the Indian COVID cases globally

## Data Source:

    https://www.mohfw.gov.in/
    https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset
    https://www.worldometers.info/coronavirus/#countries
    https://api.covid19india.org/


## Prophet Package

Prophet is open source software released by Facebook’s Core Data Science team. It is available for download on CRAN and PyPI.

Prophet is a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.
References
    https://facebook.github.io/prophet/
    https://facebook.github.io/prophet/docs/
    https://github.com/facebook/prophet
    https://facebook.github.io/prophet/docs/quick_start.html

The input to Prophet is always a dataframe with two columns: **ds** and **y**. The **ds (datestamp)** column should be of a format expected by Pandas, ideally YYYY-MM-DD for a date or YYYY-MM-DD HH:MM:SS for a timestamp. The y column must be numeric, and represents the measurement we wish to forecast.

## ARIMA Model
ARIMA stands for **Auto Regressive Integrated Moving Average**. There are seasonal and Non-seasonal ARIMA models that can be used for forecasting.

Autoregressive (AR) component: A purely AR model forecasts only using a combination of the past values like linear regression, where the number of AR terms used is directly proportional to the number of previous periods taken into consideration for the forecasting.

Moving Averages(MA): Random jumps in the time series plot, effect of which is felt in two or more consecutive periods. These jumps represent the error calculated in the ARIMA model and represent what the MA component would lag for.

# How this model can be useful in fighting the COVID-19 pandemic?

    - Medical resource optimization
    - Ensuring demand planning stability
    - Contact tracing
    - Situational awareness and critical response analysis
