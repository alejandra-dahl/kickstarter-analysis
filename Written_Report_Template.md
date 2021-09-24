# Kickstarting with Excel

## Overview of Project

### Purpose
In this project, there are two main deliverables that Louise wanted to see. Because of the success of one of her plays, Louise wanted to know the outcomes of other similar campaigns in association with their launch dates and funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The first analysis done was to determine the outcomes of similar campaigns based on their launch date. One of the first things that needed to be done was convert the Unix timestamp into a format that was more readable. Once the conversion was done, the year of the launch date was pulled into a column of it's own. Because Louise was only interested in comparable campaigns, the data was also filtered by parent category: theater. A pivot table and chart was created to show launch dates (by year then grouped by month) and the outcome: canceled, failed, successful.

When the chart is filtered by the parent category, theater, it's easy to see that it had the most success during the summer months although with a slight increase in failed outcomes. There has also been a very low count of canceled theather campaigns. As the chart is filtered by theater and year, it can be seen that campaigns started to see the most success after 2014, even though there were some that failed or were canceled.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/90485451/134447177-9477b40e-62fb-4d3c-b5b2-77e338b26876.png)

### Analysis of Outcomes Based on Goals
The second analysis done was to determine the outcome of campaigns, specifically for plays, based on their goal amount ranging from less than $1,000 to greater than $50,000 (US dollar). The same outcome categories were used - succesful, failed, and canceled. In order to figure this out, each campaign needed to be categorized by goal and outcome category. Goal amounts were placed in increments of $5,000. Then the countif() function was used to count how many campaigns succeeded, failed, or were canceled under each monetary increment. Percentages for each category was calculated. 

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/90485451/134600571-0433db74-3628-478c-b632-a984686e5789.png)


### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Theater campaigns saw the most success during the summer months, March to almost September, even though there was a small uptick in failed campaigns compared to the winter months. Another thing to note, is that 2014 was the first year where theater campaings started either succeed, fail, or get canceled. That data before 2014 seems limited and only shows only theather campaigns that succeeded.

- What can you conclude about the Outcomes based on Goals?
The first thing to note was that there were no play campaigns that were canceled. The next obvious thing was the drastic percentage of failed campaigns after $44,999 and above. There were only 2 successful campaigns and 14 failed campaigns with goal amounts greater than $50,000. Campaigns seemed to have the most success when the goal amounts were $4,999 or below. This range also showed the smallest amount of failed campaigns. There was a spike in successful campaigns in the $35,000 - $44,999 range with a slighly higher failure rate compared to those in the first two smaller goal categories.

- What are some limitations of this dataset?
The data could be incomplete. For example, they have not recorded failed or canceled theater plays before 2014. It is also difficult to determine the reason why certain campaigns failed or where canceled. 

- What are some other possible tables and/or graphs that we could create?
It would be helpful to build a pivot table and line chart to show failed, succesful, canceled campaigns based on pledged amount. Were campaigns more likely to succeed if they met or surpassed their goal and by how much?
