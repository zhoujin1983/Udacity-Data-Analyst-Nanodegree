# Ford GoBike Dataset Analysis 
## by Jin Zhou


## Dataset

The dataset is downloaded from Ford GoBike and licensed by Ford GoBike for the whole year 2018 in San Francisco Area. This dataset includes 1.85 million trips with various features including as start/end locations, time and user attributes. 

The data wrangling steps are as follows:
* remove rows where start/end_station_id, start/end_station_name is null.
* Change start_time/end_time data type to datetime type.
* Change all ids, station_id, bike_id to be object type.
* station longitude/lattitude has some outliers, which need to be removed. 
* By clustering station longitude and lattitude, there are actually three cities included, 'San Francisco', 'Oakland' and 'San Jose'.

## Summary of Findings

* More trips are with subcribers than customers.
* For week days, there are more trips than weekends.
* Summer time there are more trips than other seasons.
* Most trips happended when people use them to go to work or get off from work.
* Median duration secs is only around 540 secs on week day, while on weekend, the median duration will be 640 seconds.
* Median duration secs is relative lower on the beginning of day (with large fluctuation), while on weekend, the median duration will be higher around 3pm. Then lower again till 5pm.
* For user type, we can see that regular customer, duration secs median is 900 secs. While subscriber take less time, median is 500 seconds, possibly means that subscribers use bike for work, thus, less fluctuation than regular customer.
* For all the three cities, we both see the trend that the median duration secs is lower during week day than weekends, with clear trend that median duration for San Francisco is highest, then Oakland, followed by San Jose. The trend seems true for all 7 days of the week.
* For subscribers, the median trip duration secs change during the week of day is relatively small. Unlike customers, the median trip duration secs have a trend that is lower on week day than weekends.


## Key Insights for Presentation
* Median duration secs is only around 540 secs on week day, while on weekend, the median duration will be 640 seconds.
* For all the three cities, the median duration secs is lower during week day than weekends, with clear trend that median duration for San Francisco is highest, then Oakland, followed by San Jose. It seems true for all 7 days of the week.
* For subscribers, the median trip duration secs change during the week of day is relatively small. Unlike customers, the median trip duration secs have a trend that is lower on week day than weekends.
* In oakland, median duration secs seems have the trend of increasing duration secs for both subscriber and customer. While it is not true for other cities, like San Francisco and San Jose. San Francisco and San Jose subscriber median trip duration secs is less changing with week of day. San Jose the customer median trip duration secs trend for weekend and week day is not obvious than other two cities.
