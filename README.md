# PyBer Analysis

## Overview of the Project

### In this project we work for PyBer, a Python based ride-sharing app. We have been tasked with performing an exploratory analysis on ride-sharing data. Once we perform our analysis we must create visualizations in order to tell a compelling story about the data. We will present these visualizations to the CEO.

### After performing our analysis and presenting our findings, the CEO has tasked us with an additional analysis. Our task is to use our Python skills and knowledge of Pandas to create a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, we will create a multiple-line graph that shows the total weekly fares for each city type. The CEO has also asked us to submit a written report that summarizes how the data differs by city type and how those differences can be used by decision-makers at PyBer.

## Results

### After merging all of our data and performing our calculations, we arrive at the below DataFrame:

![](https://github.com/christianhargett/PyBer_Analysis/blob/master/analysis/City_Type_Summary_DataFrame.png)

### This DataFrame displays summary statistics for each city type in our dataset (Rural, Suburban, and Urban). The Total Rides and Total Drivers values from least to greatest are as follows: Rural, Suburban, Urban. This makes intuitive sense considering the general trend in population size for these city types follows the same pattern. The same applies for the Total Fares columns. It makes sense that Urban areas generate the most amount of fares considering this city type alone accounts for 68% of all of PyBer's rides. 

### When looking at the Average Fare per Ride column, the values from least to greatest are: Urban, Suburban, and Rural. This is the opposite pattern of the previous columns, however this trend also make intuitive sense. Since the formula for average fare price = total fares / total rides, the average fare price for Rural cities is bound to be the highest among the 3 city types. This is because there are the fewest amount of rides in Rural cities, and PyBer's pricing model likely aims to offset the revenue loss from shortfall in rides by bumping the ride price up (compared to other city types). The result of this is a higher average fare price per ride in cities with lower populations, and this theory is supported in our city type DataFrame. The same logic applies to the Average Fare per Driver column.

### We also created a visualization that plots weekly fares by city type:

![](https://github.com/christianhargett/PyBer_Analysis/blob/master/analysis/PyBer_fare_summary.png)

### This chart displays the total fares that PyBer earned on a weekly basis for each city type in January through April of 2019. As expected, Urban cities accounted for the most fares earned on a weekly basis while Rural accounted for the least. Each city type appears to have a rise and fall in fares on a weekly basis. One data point that stands out in the visualization is the first week of April. It appears that all city types experienced a large decrease in total fares. 

## Summary

### After reviewing the DataFrames and visualization, there are 3 areas that PyBer should look into. The first area I would recommend that they look into is increasing the rides in Rural areas. Rural areas only accounted for 5% of total rides and 7% of total fares in the first 5 months of 2019. There might be a larger market for rides that PyBer can access through methods such as increased marketing tactics, employing more drivers in those areas, etc. Another recommendation I would make is to evaluate their fare prices in Urban areas. Since demand for rides is much higher in Urban areas, it might be worth testing how high they can increase their fare prices before they begin seeing dips in revenue. This way they can find the optimal price point in Urban areas to maximize PyBer's revenue. Lastly, the final recommendation I would make is to further analyze why all city types saw such a big decrease in total fares in the first week of April. If this big decrease in fares is something that PyBer can avoid, then it is perhaps worth the time and effort it takes to look into the issue.
