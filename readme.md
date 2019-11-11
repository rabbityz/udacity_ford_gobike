Ford GoBike (Bay Wheel Bike) Usage trend analysis
Yunhan Zhu


Dataset - Ford GoBike

We used the anonymous usage data of Ford GoBike/Bay Wheel Bike for this analysis. The original data was downloaded from Ford GoBike/Bay Wheel Bike website, giving us over 4 million bike share entries between June 2017 and October 2019. Each entry has 16 features, including bike id, bike_share_for_all_trip, duration by second, start & end station details (id, longitude, latitude, station name), start & end time, member details (birth year, gender), and user type. Some features are numerical (such as duration), but most others are categorical.

For the purpose of our study, we have removed the entries with missing details. It is also worth noting that because data entries prior to 2018 are missing bike_share_for_all_trip details, they have been eliminated from our analysis. Overall, these changes narrow down our scope to 3.5 million entries.

In addition, we have also added some new features based on the existing information, including 1/ weekday, weekday type, year month based on start time; 2/distance based on star & end station longitude and latitude; 3/member age based on start time and member birth year.




Summary of Findings

Key findings from univariate exploration 
1. Usage has improved steadily over time. Usage dropped YoY and MoM during the three months between May and July 2019, although that has started to recover from Aug 2019.
2. Most Bay Wheel bike trips were made by subscribers as part of the whole trip. 
3. Within the subscribers, there are more men than women, and most of the subscribers fall between 25-35 years old.
4. Most rides are between 0.5-2km, within 15 minutes.
5. 7-9am and 4-6pm are two peak periods for bike sharing, and weekdays saw more usage than weekends.

Key findings from bivariate exploration
1. Duration tends to increase with distance, but longer duration doesn't always gurantee longer distance. This makes sense - speed also plays a role here.

2. It comes as a surprise that ride duration and distance are shorter for subscribers than customers (non-members). But on a second thought, this makes sense - subscribers probably use bike share more often, especially for part of their trip, which coincides with our other finding, that if bike share is used for part of the trip, duration and distance are shorter. 

3. Weekdays and weekends also have different usage patterns:

    a. Start hour distribution is different - whilst weekday start-hour has a bimodal distribution with two peak periods (7-9am and 3-6pm), weekend start-hour distribution is more centered around lunch time. 

    b. Weekends see longer duration and shorter distance than weekdays - this is probably because people tend to use bike share for more leisure (and hence slower) rides over weekends.

4. Among subscribers, usage patterns are modestly different by gender and age group.

    a. female subscribers are mostly centred around age 30, whilst the male members have a more evenly age distribution. 

    b. Older age groups (30+) are more active in early morning (4-6am) and early afternoon (3-5pm). Younger members between 20-30, on the other hand, are more active during the other periods. 

    c. Also, younger members around 25 years old more often uses bike share for the entire trip than the older ones. 

Key findings from multivariate exploration
First is that, usage pattern is different by type of weekdays. 
1. On weekdays, there are two peak periods between 7-10am and 4-7pm, with a greater number of rides and a larger number of longer rides by both duration and distance. 
2. On weekend, rides are normally distributed throughout the day between 7-10am, and longer rides (by both distance and duration) also happen during the peak period between 1-4pm.

Second, there exists a similar discrepancy 1/ when users choose bike share for only part of the trip and whole trip, and 2/age group (20-30 vs 25-35), to that of the different usage patterns on weekdays and weekends. Suggesting that there might be more working age adults using bike sharing for part of the trip, possibly for commuting purposes, during weekdays.

1. on either bike share for the entire trip or part of the trip:

    a. When users use bike share for only part of the trip, the behavior is similar to that on weekdays, i.e. there are two peak periods between 7-10am and 4-6pm, with more longer rides happening in those two periods. This suggests people tend to use more bike share as part of the trip during the weekdays.

    b. When users use bike share for the entire ride, the behavior is similar to that on weekends, although there is one less obvious peak period between 4-6pm. This implies that people are more likely choosing bike share for the entire ride, possibly for leisure purposes during the afternoon, over the weekend. On the other hand, duration is more centred between 3-10 minutes, suggesting people are less likely to use bike share for longer rides over the weekend. This is also in line with our earlier conclusion, that people might prefer to use bike share for leisure rides over the weekend.

2. By age group, weekdays peak hour rides are taken by older adults (aged between 25-35), whilst weekends see more rides by younger adults (aged between 20-30)




Key Insights for Presentation

1. Usage has been improving over time. 

2. Most Bay Wheel bike trips were made by subscribers, most of which fall between 25-35 years old. 

3. Most rides are between 0.5-2km, within 15 minutes.

4. Duration tends to increase with distance, but longer duration doesn't always gurantee longer distance.

5. Weekdays and weekends also have different usage patterns.  There exists a similar discrepancy 1/ when users choose bike share for only part of the trip and whole trip, and 2/age group (20-30 vs 25-35), to that of the different usage patterns on weekdays and weekends. Suggesting that there might be more working age adults using bike sharing for part of the trip, possibly for commuting purposes, during weekdays.