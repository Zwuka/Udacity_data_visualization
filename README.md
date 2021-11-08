# Exploring riding made in a bike-sharing system

## by Evgeniy Kuryan


## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area.

Question's with what i begin:

When are most trips taken in terms of time of day, day of the week, or month of the year?

How long does the average trip take?

Does the above depend on if a user is a subscriber or customer?

## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.

After a brief check of the data set find that I might do some cleaning operations, like changing columns with dates from string to DateTime objects, adding columns with a day of week information

while we look at uni-variate visualization we find some interesting information like: we have big outliers in 'duration_sec' variable, member_birth_year.
Also interesting observation that most part of bikes was rented in area that stays in latitude 37.7 - 37.9, and longitude -122.4 - -122.2. This information need furher inspection.

After deeper look at date of birth of subscribers I found next information:
I think there are errors in the dates of birth before 1930, but I'm not entirely sure about the years in the range from 1910 to 1930 (maybe there are some strong old people riding bicycles, or maybe their children use parent's accounts). But I am absolutely sure that the records with the years of birth in the range from 1880 to 1900 were not created correctly.


## Key Insights for Presentation



> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.