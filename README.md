# surfs_up

## Overview

### The purpose of this analysis is to understand weather trends on the island of Oahu in order to determine the viability of opening a surf shop.

## Results

### We can see that the averages of the June and December data are close together. We can also see that the December data set is overall smaller than the June data set. Additionally, the standard deviation of the December data is higher:

![june](https://user-images.githubusercontent.com/104467100/177467869-0ae89ae4-b061-4d69-93db-6d13da09c3dd.png)
![december](https://user-images.githubusercontent.com/104467100/177467881-8d7fab0b-a6d9-4ebc-8d9a-3c98c553ba04.png)

## Summary

### We can see from the statistical results of the "June" temperature data frame that the mean temperature is not drastically different from the mean temperature of the "December" temperature data frame. However, it is important to note that the count of December temperatures is smaller so there isn't as much data available for December. This gives us an incomplete picture of December temperature data from a statistical standpoint and suggests our average may not be as reliable the June average. This is also indicated by the higher standard deviation of the December data.


### Two additional queries could be performed to gather precipitation data. There queries would be:

### session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 6) (June)

### session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 12) (December)
