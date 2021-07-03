# Kickstarting with Excel

## Overview of Project

### Purpose
This analysis was done to help analyze and visualize two specific cuts of the Kickstarter data:
1. Theater Outcomes Based on Launch Date, specific to the campaign parent category of "theater". This will help us visualize what months would be the best and the worst to launch a theater campaign with Kickstarter. 
2. Outcomes Based on Goals, specific to the campaign subcategory of "plays". This will help us visualize what fundraising goals have the most likely chance of success or failure, within a range. 
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
For Outcomes Based on Launch Date, we analyzed all Kickstarter campaigns listed, across all countries and years, in the parent category of "Theater" (all sub-categories included). We counted how many campaigns were successful, failed, or canceled, in each calendar month, based on the launch date of the campaign. "Success" was determined based on whether the campaign's pledge met or exceeded it's stated goal. Canceled campaigns would be those ended by the organizer prior to completion of the goal or stated time frame. To accomplish this, we used a pivot table to summarize the data combined with a pivot chart for visualization. See chart below in conclusions. 

### Analysis of Outcomes Based on Goals
For Outcomes based on Goals, we analyzed Kickstarter campaigns listed in the sub-category of "plays" across all years and countries. We split the goals into ranges of $5,000 per range, with Less than $1,000 and over $50,000 as the bottom and top ends, respectively. We categorized each sub-category "play" campaign into successful, failed or canceled (there were no canceled plays in the data set) by the range that the campaign's goal fell into. We then calculated the percentage in each range that was successful or failed, to get a sense of what ranges tend to have more or less chance of success, based on their stated fundraising goal. This was completed using formulas with a line graph for visualization; see graph below in conclusions. 

### Challenges and Difficulties Encountered
The main challenges encountered are due to the data that is available for analysis; see limitations of the data set and other analysis we could create below for some challenges encountered in the data set as well as recommendations for future analysis. All subtotals were verified for accuracy as analysis was being performed. 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/85597801/124364838-a3737000-dc09-11eb-8dbf-a15e5fa007ba.png)
1. The best month to start a campaign for a theater Kickstarter would be May, followed closely by June. These months have the highest number of successful campaigns, with no corresponding major uptick in failed or cancelled campaigns.
2. The worst months to start a campaign would be October or December. 
		-While March & September both have a lower number of successful campaigns than October, they also have a lower number of failed campaigns, leading us to believe that there were fewer campaigns started in those months, but not necessarily that they had a lower chance of success. 
		-Specifically for December, the number of failed & successful campaigns are almost equal, giving it the lowest chance of success, around 50-50.


- What can you conclude about the Outcomes based on Goals?
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/85597801/124364835-9ce4f880-dc09-11eb-8a45-c3978e795981.png)
1. It seems that in general lower funding goals have a higher chance of reaching the goal. One outlier appears to be $35,000 to $44,999, however there were only 9 projects in this range on which to judge, compared to 534 projects in the $1,000 to $4,999 range, so this may be an anomaly based on the specific projects being funded having more interest. Excluding that range, it otherwise seems as though anything over $19,999 will have less than a 50% chance of success.


- What are some limitations of this dataset?
	1. The projects are heavily skewed towards those with lower fundraising goals. The median goal is $5,000 with an interquartile range of $13,000, meaning any campaigns above $34,500 should probably be disregarded as outliers. 
	2. The data is from 2010 to 2017, which makes the very newest data available to us 4 years out of date, prior to the COVID-19 pandemic which has likely had an impact on this. There is also an approximate inflation rate of 23% since the earliest data, which means we would now need to raise $6,500 for what in 2010 was $5,000; it is difficult to predict how success/failure might skew with inflation.
	3. Specific to our analysis on goals, we did not filter for US only, which means other country currency is also included, potentially further skewing our monetary ranges. It may be beneficial to convert other country currency to equivalent US currency to perform a more robust analysis. 
	4. With this analysis, we only reviewed successful or failed, but not the % of the goal funded, which leaves gaps in what happened. For example, a play with a goal of $20,000 could have raised $15,000, which would be considered a failure, while a play with $10,000 goal raised exactly $10,000 and was considered successful. The first still resulted in a higher range of funds raised, and it is impossible to know if people had overinflated their goals believing they would not be met (overshooting the target).

- What are some other possible tables and/or graphs that we could create?
	1. More information on the actual pledged amount may be useful to balance out #4 above. 
	2. Creating another analysis using only March 2020-present data may be useful, to compare how things have skewed due to COVID-19, if at all.
	3. Reviewing the Outcomes based on Goals but only including US goals, or converting other currencies into US currency equivalent
