# Flight Data Analysis
## by Timileyin Oladayo


Flight Data analysis for Udacity ALX data analysis

## Dataset

> The dataset for this study comprises roughly 7 million records of domestic flights in the United States. These records contain information such as date, distance, arrival time, and various other features including delay factors. As part of my analysis, I excluded approximately 150,000 flight data points that were either canceled or diverted, as well as those originating or ending in Hawaii

## Summary of Findings

> During this investigation, I examine the connection among all the variables. As anticipated, I discover that Departure Delay and Arrival Delay, as well as Distance and Elapsed Time, have a significant correlation. This exploration follows three primary paths:

- I examine the relationship between delays and various other features, including the airline, departure airport, route (which is a combination of departure and arrival airports), time, date (month and day of the week), and elapsed time. I investigate whether there is a correlation between delays and these other factors or not.

- The delay that a flight experiences can be categorized into two parts: Departure Delay and Elapsed Time Delay. The latter is the difference between the scheduled elapsed time (CRS) and the actual elapsed time. This delay is the extra time that passengers spend in the plane. I opted to examine these two delays individually and discovered that Departure Delay is usually longer than Elapsed Time Delay. The distribution of Departure Delay is skewed to the right, and it generally takes higher values, whereas the distribution of Elapsed Time Delay is symmetrical and tends to take lower values. Surprisingly, these two delays are not significantly related to the distance of the flight.

- The dataset includes five factors that cause delays: "NASDelay", "LateAircraftDelay", "CarrierDelay", "WeatherDelay", and "SecurityDelay". The most frequent delay factor is "NASDelay", followed by "LateAircraftDelay" and "CarrierDelay". Since "SecurityDelay" has minimal impact compared to the other four factors, I focused my investigation only on these four. However, I found that none of these four factors had a significant correlation with the distance of the flight.


- To conclude, I created a visualization that clustered the length of the four delay factors based on four levels of Departure Delay time. Since distance did not significantly impact delay time, I did not consider it in the visualization. The Departure Delay was divided into five levels, and the distribution of each of the four factors in each level was displayed using a clustered violin plot. The plot revealed that longer Departure Delay times were associated with longer CarrierDelay and WeatherDelay. Then, I focused on Elapsed Time Delay and re-created the plot, but this time with two levels of ElapsedTimeDelay instead of DepartureDelay. The new plot indicated that only NAS Delay factor was related to longer DepartureDelay times.



## Key Insights for Presentation

> During the presentation, my focus will be on the association between the length of DepartureDelay/Elapsed Time Delay and the distribution of each of the four factors.

> To begin the presentation, I will compare DepartureDelay and ElapsedTimeDelay using a scatterplot. Next, I will illustrate the occurrence rate of each of the four delay factors using a bar chart and their delay time distribution using a violin plot. I will also demonstrate that distance has minimal impact on delay time. Following this, I will reveal the two primary findings of this analysis using a clustered violin plot that clusters delay time by DepartureDelay levels. Another clustered violin plot, grouped by ElapsedTimeDelay levels, will follow for comparison.