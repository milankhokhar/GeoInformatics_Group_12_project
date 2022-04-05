# Exercise 4: Calculate cumulative precipitation time series

In this section you want to narrow down your area of study and concentrate on the counties Olpe (OE) and Hochsauerlandkreis (HSK). 
You may have noticed the differences of SMI between OE and HSK for the month of July 2018. 
The SMI difference are not as big in May, June, and in August the SMI become quite similar. How can you explain this?
Does it have something to do with precipitation events? 
You will have to use the precipitation data offered by the German Weather Service (DWD) to find out.

We would like to emphasize again that the monthly SMI data provided by the UFZ drought monitor are snapshots of actual values at the 16th of each month 
(i.e. 2018-05-16, 2018-06-16, 2018-07-16, 2018-08-16). To investigate the influence of precipitation on SMI we look at the period from 2018-04-16 (one month before the first SMI map) until 2018-08-16 (the timestamp of last SMI map of interest). 

## Aggregate hourly precipitation rate to achieve daily precipitation rate

To identify rain events you will plot daily precipitation in a vertical bar chart. You have to aggregate the hourly precipitation rate (mm/hr) over a day to yield the daily precipitation rate (mm/day). 
Start with an appropriate Jupyter notebook from the lecture to create a dataframe with precipitation time series merged columnwise such that each column contains the time series for one station. Extend the notebook to aggregate the hourly data to daily resolution. Consider to use the Pandas Dataframe function `df.group_by(...)` or use other methods if you like.

### Cumulative precipitation time series
You should generate two diagrams: 

- A bar chart of the daily precipitation rates (mm/day) covering the four months of the study 
(from 2018-04-16 until 2018-08-16) to identify interesting precipitation events
- A line graph showing the cumulative precipitation for the same period.

You should consider the following:
- Think about how to organize the representation. 
You are generating several graphs in one diagram from weather stations in OE and HSK (maybe using facets?)
- Consider correct labeling of your graphs. Use legends when appropiate.
- The images should be tidy. Take care of occlusions of graphs that are not readable.
- Make sure to include relevant information in your plots, such as time resolution, units, time period, etc.

* [Previous](ex3.md)
* [Next](ex5.md)
