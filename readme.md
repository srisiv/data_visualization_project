# Flight Data 2008 Exploration
## by Sridhar Sivanand


## Dataset

> Provide basic information about your dataset in this section. If you selected your own dataset, make sure you note the source of your data and summarize any data wrangling steps that you performed before you started your exploration.
Flight data for the year 2008 was selected for analysis. It contained over 7 million records. Some of the data wrangling done was as follows
- The Month and Day of Week columns were numerical. They were converted to appropriate text values to become categorical
- All records had an arrival delay value even if the flight was on time or early. So in order to distinguish a delayed flight from a flight that was early/on time, a FlighStatus column was added. From the data, it was noted that the different delay factors had values only if the arrival delay was at least 15 minutes. So any record with an arrival delay below 15 minutes was marked as "On Time" 


## Summary of Findings

> Summarize all of your findings from your exploration here, whether you plan on bringing them into your explanatory presentation or not.
- The distributions of number of flights by day of week, number of flights by month, number of flights during a day were done. None of them yielded any significant insights. 
- The arrival delay and distance distributions were right skewed, and log transformation didn't help in bringing about a normal pattern for distance. Log transform wasn't done on arrival delay as there were negative values in the column. These wouldn't be added to the explanatory presentation
- The number of cities in Origin and Destination was too huge, to be used for any meaningful analysis as categorical variables. A few plots like the top 5 cities for originating flights, for delayed flights, cancelled flights etc were created and some of these may be brought on to the explanatory presentation.
- Plots for the contributing factors to delay and cancelled flights were also plotted and will be brought on to the explanatory presentation, such as the proportion of the factors contributing to the arrival delay or flight cancellation
- There were also bar charts for flight delays and cancellations across different months and days of week. I might add the distribution about months to the explanatory presentation
- box and violin plots were explored for relationship between arrival delay and day of week and month. But the results didn't yield any insights and so will not be going into the explanatory presentation. A multivariate plot of the different delay factors against day of week and month yielded no interesting results either.
- Scatter plots for arrival delay against departure time, as well as against departure time yielded no linear relationship. A square (since arrival delay had negative values) followed by log transform of arrival data was also done with the above scatter plot analysis but no relationship could be discerned. So these plots wouldn't go into the explanatory presentation.
- A clustered bar plot of the flight status for the 5 busiest airports was created and will be used in explanatory slides

## Key Insights for Presentation

> Select one or two main threads from your exploration to polish up for your presentation. Note any changes in design from your exploration step here.
- I would be starting with the number of flights handled by the top 5 busiest airports
- Then percentage of overall flights that are on time, delayed and cancelled will be provided
- The percentage of flights on time, delayed and cancelled for flights originating from each of the 5 busiest airports will be provided
- The contribution of the each delay factor to the overall flight delays will be plotted
- The distribution of flight delays over the months of the year will be shown
- The contribution of each cancellation factor causing cancelled flights will be displayed
- The distribution of flight cancellation over the months of the year will be shown
- The proportions of factors causing the arrival delay and the proportion factors causing cancellations