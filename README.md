# PyBer_Analysis

## Overview of the analysis
Here we perform an analysis using `pandas` of rideshare datasets
[city_data.csv](Resources/city_data.csv) of format `city,driver_count,type`
and [ride_data.csv](Resources/ride_data.csv) of format
`city,date,fare,ride_id` to determine the following for each rural, suburban,
and urban cities:

- Total Rides
- Total Drivers
- Total Fares
- Average Fare per Ride
- Average Fare per Driver

We then visualize the relationship between fares and city type using
`matplotlib` to compare the three types and provide recommendations to maintain
an effective presence in each environment.

### Resources
- Data Source:
    - [city_data.csv](Resources/city_data.csv)
    - [ride_data.csv](Resources/ride_data.csv)
- Software:
    - Python 3.7.6
    - Matplotlib 3.1.3
    - pandas 1.0.1
    - Jupyter Notebook 6.0.3
 
## Results
We see from the [Pyber Summary Dataframe](Resources/pyber_summary_df.png) that
there are significant differences in ride cost and activity between the rural,
suburban, and urban cities.

### Total Rides
Breakdown of the total number of rides by city type:

- Rural: 125
- Suburban: 625
- Urban: 1,625

The number of rides in urban cities is 13 times that of rural cities,
which likely follows from a population difference of similar magnitude.

### Total Drivers
Breakdown of the total number of drivers by city type:

- Rural: 78
- Suburban: 490
- Urban: 2,405

Here we see the number of drivers in suburban cities is roughly 6.3 times that
of rural cities, close to the ratio between total rides of these two city
types.

### Total Fares
Breakdown of the total fare cost by city type:

- Rural: $4,327.93
- Suburban: $19,356.33
- Urban: $39,854.38

We find that urban cities provide approximately 63% of the total fares in this
data. This roughly follows from January 2019 through April 2019 as shown in
[Plot of Total Fare by City Type](analysis/PyBer_fare_summary.png).

### Average Fare per Ride
Breakdown of the average fare per ride by city type:

- Rural: $34.62
- Suburban: $30.97
- Urban: $24.53

We see that while there are fewer rides in rural cities, the average fare
per ride is greater than that of urban cities by a factor of roughly 1.4.

### Average Fare per Driver
Breakdown of the average fare per driver by city type:

- Rural: $55.49
- Suburban: $39.50
- Urban: $16.57

While the total fares in urban cities is higher than that of suburban and
rural ones, we find the total number of drivers has a greater effect on the
average fare per driver, causing it to be highest in rural cities.

## Summary
This analysis shows that urban cities have higher rideshare activity
producing a greater proportion of total fares relative to suburban and rural
cities.

### Recommendations Based on City Differences
We see in [Pyber Summary Dataframe](Resources/pyber_summary_df.png) that fares
generated in urban cities account for 63% of the total fares in our data,
indicating it is this environment in which rideshare companies are most likely
to find success. This is also shown from the significantly higher number of
drivers in urban cities relative to other types. It is therefore advised to
focus resources primarily in urban settings.

We also see from
[Plot of Total Fare by City Type](analysis/PyBer_fare_summary.png) that late
February to early March provide the largest total fares for each city type,
suggesting this may be an ideal time to increase the number of drivers to
accommodate this increased demand.

Finally, we see that the month of March provides particularly low fares in
suburban and rural cities. It therefore may be wise to move resources from
these types of cities to urban ones at this time in order to counter this
decline.
