# Module 8 Challenge - Pandas

## Goal

The goal of this challenge is to analyze the Google search trends data for MercadoLibre and apply time series forecasting using the Prophet model. Specifically, we aim to explore the patterns in search traffic, such as identifying peak times, trends, and forecasting future search volumes. We will use Pandas for data manipulation and Prophet for the forecasting model.

## Problem or Question

The main questions to answer during this analysis include:
- What are the peak hours and days for search traffic related to MercadoLibre?
- How does the search traffic vary over a weekly and yearly cycle?
- Can we accurately forecast future search traffic for the next 2000 hours?
- What is the lowest point in search traffic across the calendar year?

We will also identify the most significant time-based patterns in the data, such as daily and weekly cycles, and use these insights to inform future predictions.

## Steps Taken

1. **Data Preparation**: The initial step involved reading the dataset and cleaning it. This included converting the `Date` column into a datetime format and ensuring there were no missing values.

2. **Data Analysis**:
   - We explored the search traffic trends over various time periods, including the daily, weekly, and yearly breakdowns.
   - We visualized these trends to identify peak times and potential seasonal patterns.

3. **Prophet Model**:
   - We used the Prophet library to forecast future search trends. This included:
     - Preparing the data by renaming the necessary columns (`ds` for date and `y` for search traffic).
     - Fitting the Prophet model on the data.
     - Creating a future dataframe to predict search trends over the next 2000 hours.
     - Visualizing the forecast results, including confidence intervals for the predictions.

4. **Analysis of Forecast**:
   - After fitting the model, we analyzed the near-term forecast for search traffic, as well as the individual time series components such as daily, weekly, and yearly trends.
   - We answered questions regarding the peak time of day, day of the week with the most search traffic, and the lowest point in search traffic for the year.

## Unique Observations

- The data revealed distinct patterns in the search traffic for MercadoLibre, with peak traffic observed during specific hours of the day and certain days of the week.
- The Prophet model successfully provided future predictions for search trends, including upper and lower bounds based on confidence intervals.
- One interesting observation was the consistency in traffic patterns during weekends, which might suggest higher user engagement for MercadoLibre during these times.

## Conclusion

By analyzing the search traffic data, we gained valuable insights into the patterns of search interest for MercadoLibre. The use of the Prophet model allowed us to create reliable forecasts, which can be useful for planning and optimizing marketing strategies.

## Resources Used

- [Prophet Documentation](https://facebook.github.io/prophet/docs/)
- [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
- [Matplotlib Documentation](https://matplotlib.org/stable/users/index.html)
- Class slides and activities
- Google
- Open AI

