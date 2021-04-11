# rideshare-analysis

## Overview

Objective:
>Create a summary DataFrame of ride-sharing data by city type. Then, using Pandas and Matplotlib, create a multiple-line graph that shows the total weekly fares for each city type.
  
The analysis will break down city data into 3 categories:

 - Rural
 - Suburban
 - Urban

The Data Represented:

  - *Total Rides* - Total number of rides
  - *Total Drivers* - Total number of drivers assigned to city type
  - *Total Fares* - Total number of Fares
  - *Average Fare per Ride* - Average fare earned per ride in given city
  - *Average Fare per Driver* - Average fare earned per driver in given city

## Results
### Deliverable 1: Get a Summary DataFrame
The first deliverable was to merge the two sets of data in to a single dataframe, group the data by city type, and calculate the totals.

| City Type | Total Rides | Total Drivers | Total Fares | Average Fare per Ride | Average Fare per Driver |
|----------|-------------|---------------|-------------|-----------------------|-------------------------|
| Rural    | 125         | 78            | $4,327.93   | $34.62                | $55.49                  |
| Suburban | 625         | 490           | $19,356.33  | $30.97                | $39.50                  |
| Urban    | 1625        | 2405          | $39,854.38  | $24.53                | $16.57                  |

Urban rideshares yield the highest volume, almost tripling the nearest amount of the other categories. The total fares do not scale as well as the Rural and Suburban rideshares, as the Urban rideshares yield and average of $24.53 per ride. Suburban and Rural rideshares yield higher fares per ride, which could be attributed to the liklihood of the distance of the ride being longer due to being further from the city. When compared to the number drivers, the Urban category stands out significantly due to the high number of drivers. This is not necessarilly a bad thing, because when surges in demand in urban cities (conferences, airport delays, stadium games/events), a high driver count can respond quicker and maximise the opportunity for fares.

### Deliverable 2. Create a multiple line plot that shows the total weekly of the fares for each type of city.
The second deliverable was to show the weekly totals of the fares per city type from March 1st, 2019 to April 29th, 2019.
![image](https://user-images.githubusercontent.com/80546200/114324235-ad943f80-9aee-11eb-91b8-73c5c0dda99c.png)

The data used to populate the graph is shown below:

| Week of     | Rural    | Suburban   | Urban     |
|-------------|----------|------------|-----------|
| 2019-01-06  | $187.92  | $721.60    | $1,661.68 |
| 2019-01-13  | $67.65   | $1,105.13  | $2,050.43 |
| 2019-01-20  | $306.00  | $1,218.20  | $1,939.02 |
| 2019-01-27  | $179.69  | $1,203.28  | $2,129.51 |
| 2019-02-03  | $333.08  | $1,042.79  | $2,086.94 |
| 2019-02-10  | $115.80  | $974.34    | $2,162.64 |
| 2019-02-17  | $95.82   | $1,045.50  | $2,235.07 |
| 2019-02-24  | $419.06  | $1,412.74  | $2,466.29 |
| 2019-03-03  | $175.14  | $858.46    | $2,218.20 |
| 2019-03-10  | $303.94  | $925.27    | $2,470.93 |
| 2019-03-17  | $163.39  | $906.20    | $2,044.42 |
| 2019-03-24  | $189.76  | $1,122.20  | $2,368.37 |
| 2019-03-31  | $199.42  | $1,045.06  | $1,942.77 |
| 2019-04-07  | $501.24  | $1,010.73  | $2,356.70 |
| 2019-04-14  | $269.79  | $784.82    | $2,390.72 |
| 2019-04-21  | $214.14  | $1,149.27  | $2,303.80 |
| 2019-04-28  | $191.85  | $1,357.75  | $2,238.29 |


## Summary

### Suggestions and Recommendations
1. Include route/positional data for rides.
2. Include non-fare travel time/distance.
3. Determine effectiveness of pretermined routes/hot zones near places of interest.

>1. Include route/positional data for rides.
>
Including route/positional data for rides would allow further analysis on more efficient ways to get more fares. Positional data combined with a start ride time and end ride time combined with a heat map over time would allow you to see where and how the demand for rides shift over position and time. Using these trends you could better anticipate and maximize number of fares per driver.

>2. Include non-fare travel time/distance.
>
Including non-fare travel time will help provide insight on "dead-zones" and timing windows where drivers are less needed. This will help operation time be better spend on periods and places where it is most needed. 

>3. Determine effectiveness of pretermined routes/hot zones near places of interest.
>
Predetermined routes can help consolidate high volume places of interest. How effective and if it is worth while to impletment a system for predetermined routes will require further analysis depending on the city.


