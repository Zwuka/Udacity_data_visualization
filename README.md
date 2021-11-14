# Exploring riding made in a bike-sharing system

## by Evgeniy Kuryan


## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

Question's with what I begin:

When are most trips taken in terms day of the week, number of week or month of the year

How long does the average trip take?

Does the above depend on if a user is a subscriber or customer?

## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.

After a brief check of the data set find that I might do some cleaning operations, like changing columns with dates from string to DateTime objects, adding columns with a day of week information

while we look at uni-variate visualization we find some interesting information like: we have big outliers in 'duration_sec' variable, member_birth_year.
Also interesting observation that most part of bikes was rented in area that stays in latitude 37.7 - 37.9, and longitude -122.4 - -122.2. This information need further inspection.

After deeper look at date of birth of subscribers I found next information:
I think there are errors in the dates of birth before 1930, but I'm not entirely sure about the years in the range from 1920 to 1930 (maybe there are some strong old people riding bicycles,
or maybe their children use parent's accounts). But I am absolutely sure that the records with the years of birth in the range from 1878 to 1920 were not created correctly.

We have 283 station that longitude lower in area between -122.4 to -122.2, there 329 station at all. So 86.0% of stations stays in this area
Interesting thing here, a lot of rides end in stations id 130-140.

All trips were completed in February 2019. 16 trips started in February and were completed in March 2019.
In our data, we have complete information about 3 weeks (week number 6,7,8), weeks 5 and 9 represented partly.
Also at first look most of rides was done in week number 8.

Also, looking at the distribution plots, we can see that some bicycles are used more often than others.
This information need to be confirmed with adding riding time on bikes.

Almost 90% of rides was done by subscribers (exact value = 89,17%)
The average trip duration on weekends is higher than on weekdays.
Average trip duration of all users are 726 seconds, average trip of subscriber are 640 seconds, and for customer in average time is 1432 seconds. 


## Key Insights for Presentation


Almost 90% of rides was done by subscribers (exact value = 89,17%)
Interesting thing here: average duration for subscriber trip is 640 second, and for Customer: 1432 seconds. Average duration of trip at all is 726 seconds.
The average trip duration on weekends is higher than on weekdays.

Our customers prefer long trips on weekends, but the duration of the trips for subscribers is practically independent of weekends or weekdays. Also, there are practically no relations between the number of rides and day of the week for our customers, but our subscribers mostly use our bikes on weekdays. This information can be used in planning a marketing campaign to increase the use of our bicycles on unloaded days.

The heavily loaded stations serve around 300 visits per day, while there are many stations with less than 4 visits per day. Let's see how it looks. I think we could check the equipment at these stations and, if necessary, transfer some of it to highly loaded stations.

.