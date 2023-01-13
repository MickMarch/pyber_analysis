# Ride-sharing Analysis

## Overview of Project

### Purpose

The purpose of this project is to use Jupyter Notebook to analyze ride-sharing data. This will be done by:

- Creating a summary of the data by **city type**
- Generating a **multi-line chart** that shows **weekly fares** for each **city type**.

<!-- -------- -->

### Datasets

The first dataset contains the following data for each city:
- City Name
- Driver Count
- City Type

The second dataset contains the the following data for each ride:
- City Name
- Date
- Fare
- Ride ID

<!-- -------- -->

## Results


### Restructuring of Datasets

Merging the datasets on the "city" column was an important first step to get all the data into one data frame:

![merged_data_example](/analysis/merged_data_example.png)

<!-- -------- -->

### City Type Statistics

After aggregating elements from the newly merged data frame, a new data frame was created with the statistics of each city type:

![pyber_summary_table](/analysis/pyber_summary_table.png)

- Urban:
  - Highest ride count, driver count, and total fares.
  - Lowest average fare per ride and average fare per driver.

- Rural:
  - Highest average fare per ride and average fare per driver.
  - Lowest ride count, driver count, and total fares.

- Suburban:
  - Middle of the road for every stat.

<!-- -------- -->

### Visualizing Weekly Fares by City Type (Jan 2019 - Apr 2019)

Using a simple approach of a multi-line chart, it becomes apparent just how much more Urban cities were making than both Suburban and Rural city types:

![pyber_fare_summary](/analysis/pyber_fare_summary.png)

<!-- -------- -->

## Summary

### Observation

We can see that the success from this data is a matter of perspective. In Rural cities, we can see that the ride-sharing company made the least amount of revenue - but - we can see that the drivers had a much higher average fare. In Urban cities, we can see that the ride-sharing company made the most revenue - but - not only is the average fare per driver the lowest in this city type, there are also more rides than there are drivers. **This means that not every driver made money in Urban cities.** Suburban cities are in the middle, a situation that can make both the drivers and the ride-sharing company happy to some degree.

<!-- -------- -->

### Recommendations to Address Disparities

1. In Urban cities, there are more drivers than there are rides. This may be a sign to boost the company's presence within the Urban cities, to be able to raise the amount of rides being made to at least match the drivers in the company's employ. This would be to combat the huge difference in average fare per driver.

2. Alternatively, it may be worth it to prevent having so many drivers in Urban cities. When there isn't guaranteed work for 32.4% of the registered drivers, it could be time to consider slowing the onboarding of new drivers. This approach could prevent being seen as an unreliable place to work. This would also be an attempt to increase the average fare per driver.

3. It may be a good idea to do some market research into the Suburban and Rural cities. They may be strained with their limited driver count. There might be more rides than the drivers can be available for. This is to combat the low total fare amounts of Suburban and Rural cities.