# Rideshare_Analysis
## Purpose:
Analyzing rideshare data and producing visualizations
## Overview:
### Purpose:
The goal of this analysis is to compare various metrics around ridesharing profitability, usage frequency, and availability at various types of cities (Urban, Suburuban, and Rural). We were particularly interested in the fares (revenues) generated in the first four months of the year. By pivoting our data by 'week', we hope to identify any trends hidden in any of the city types.

## Results:
![summary_df](/Analysis/Rideshare_Summary_DF.png)
### Rural Cities
We see that Rural cities have low demand for rideshares, resulting in lower 'total' fares (just over $4K), and fewer drivers (< 100) due to lower demand. Due to the low driver count however, we see that individual rides appear to be more expensive (approx $35 on average), likely due to the supply shortage. Drivers are also generating higher fares (approx $55 on average) compared to those in Suburban and Urban cities, as each driver is receiving a larger proportionate share of the demand for rides.

### Urban Cities
In Urban cities, we see the opposite. These cities have the highest demand for rideshares, resulting in the highest 'total' fares (close to $40K, which is approx 10x that of Rural Cities and 2x that of Suburban Cities). We also see a higher driver count (> 2k drivers needed to meet the high demand). Due to the high driver count however, we see that individual rides appear to be the cheapest in Urban settings (approx $25 on average), likely due to high competition (large supply pool). Drivers are also generating lower fares (approx $17 on average) compared to $55 on average in Rural cities and $40 on average in Suburban cities, as each driver is receiving a smaller proportionate share of the demand for rides.

### Suburban Cities
The data for Suburban cities generally falls between Rural and Urban cities. The demand for rides seems more aligned with the supply (driver count) at a ratio of 1.3 rides per Suburban city driver, versus 1.6 rides per Rural city driver and 0.7 rides per Urban city driver (calculated as total rides divided by total drivers in each type of city). However, although there is alignment between supply and demand, the total fares generated in Suburban cities is still only approx half of the fares generated in Urban cities, likely due simply to lower demand in these types of cities. 

### January - April (weekly data)
![jan_apr_weeklydata](/Analysis/Rideshare_fare_summary.png)
The line chart above, representing the total fares generated in the first four months of 2019 (on a weekly basis), support our findings above. We can clearly see that the total fares generated in Urban cities (gold line) is at the top (higher performance is consistent throughout the 4 month period), and total fares for Suburban cities (coral line) and Rural cities (sky blue line) do not cross or "beat" Urban city fares in any given week.

## Summary:
### Business Recommendations
1. Based on the data for Urban cities, we see that there are more drivers than there were actual rides in 2019, which means that there were drivers who generated $0 in fares. We recommend setting a limit on the number of drivers at each city based on ride demand, such that the ratio of total rides in a city to the total count of drivers should always be greater than 1:1.

2. While we see that Rural city drivers are generating higher fares per ride, we recommend focusing business initiatives on Urban and Suburban cities, as they collectively represent over 93% of total revenues.

3. The analysis above is primarily based on quantitative data. It is highly recommended that further analysis is performed on qualitative aspects that may impact rideshare utilization / profitability. One possible way to achieve this would be to conduct surveys, possibly offering company gift cards as 'raffle reward' to incentive riders and drivers to participate.


