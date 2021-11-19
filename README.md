# Ford GoBike Data Exploration

## Dataset

The data consists of information regarding 1,83,412 records in the dataset with 16 features. The attributes included in the interested featues in the dataset such as duration, customer, subscriber, male, female and age. The dataset can be found in the
repository [here](https://s3.amazonaws.com/baywheels-data/201902-fordgobike-tripdata.csv.zip),
with feature documentation available [here](https://www.lyft.com/bikes/bay-wheels/system-data).


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
duration of trip and day of week, user types, member gender and bike share for 
all trip. The relationship is unimodel between trip duration and total number 
of trips when trip duration is transformed to be on a logarithmic scale. I found 
a somewhat surprising result initially when the trip count for the user type, 
member gender, and bike share for all trip variables indicated that higher count 
was associated with subscriber and male featires. When I isolated trip duration 
with user type, gender and bike share, there was a clear pattern showing that
customer and female were preferring long duration trips where as all were reluctant
while sharing the bike during the trip.

For the dataset given, there was an interesting interaction in the categorical 
variable features. The maximum long duration trips were taken by female customer
during weekend as compared with male subscriber male.


## Key Insights for Presentation

For the presentation, I focus on just the influence of the duration, user type,
member gender and day of week and leave out most of the intermediate derivations. 
I start by introducing the duration variable, followed by the pattern in trip 
duration distribution, then plot the trip count barplot.

Afterwards, I introduce each of the categorical variables one by one. To start,
I use the box plots of duration across categoric variables. I'm only looking at
various plot here since it's the clearest example of how the
categorical variables affect trip duration. The combination of all categorical 
variables are covered afterwords using heatmap plots. The different colors to 
in heatmap clears the difference between trip duration.