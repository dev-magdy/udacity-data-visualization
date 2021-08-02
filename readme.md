# Exploring Ford GoBike Data
## by Ahmed Magdy


## Dataset

> I have chosen the Ford GoBike dataset to investigate in this project. The following points are observed about such dataset.
- This is bike booking data for a bike sharing service run by Ford.
- We have 183,412 observation and 16 features in the dataset.
- Each observation represents an entire booking complete with data about start and end times, start and end stations, the customer making the booking, and even the booked bike itself.
- Time columns are read as strings and need to be converted to datetime for analysis.
- Some data is missing. No need to drop these rows from the dataset. Just need to be aware of this limitation.
- Some data makes no sense. We have member birth years of pre 1920's times. Granted some people born in these times are alive and well, but I seriously doubt they can ride a bike. I may need to correct some of these years and drop some others.



## Summary of Findings

> Here are my findings about this dataset:
- Birth year distribution is skewed to the left, indicating that younger people are more likely to book a bike.
- Male riders have the lion's share of trips in our data with about 75% of trips.
- A bike can be booked any time during the day, but we can see spikes at 8 AM and 5 PM, which are the usual commuting times.
- Our data spans only the month of Febraury 2019.
- Our data spans 3 cities, San Francisco, Berkley, and San Jose, with most of the trips taken in San Francisco.
- Although the females are under represented in our data, they tend to take longer trips than males.
- One time customers tend to take longer trips than our subscribers.
- Although some old people are taking pretty long trips, it's obvious there's a positive correlation between trip duration and birht year. This indicates negative correlation between trip duration and age, i.e. younger people tend to have longer trips.
- San Francisco is the most server city by the service. San Jose seems to be underserved considering its size.
- Living in a different city doesn't seem to affect the gender ratio of the users. Men seem to be using the service about 3 times more than women in all cities.
- San Jose data doesn't show the rush hour spikes seen in the other two cities and the overall data.
- Same observation for trips within the bike-share-for-all programm.
- More bookings are made during the week by both men and women. This makes sense since a lot of people are using the service for commuting.



## Key Insights for Presentation

> Here are the main points I'm going to present
- Introduction of the dataset and why we're exploring it.
- Summary statistics about the data, like the birth year distribution, gender distribution, and cities.
- Adjust the bins for the birth year distribution to align with decades start and end.
- Highlight the fact that women tend to book longer trips although they are as much served as men.
- Discuss the fact that most of the trips are used for commuting to and from work and the cases where this doesn't apply.
- Highlight rush hour times on the count plots for more clarity.