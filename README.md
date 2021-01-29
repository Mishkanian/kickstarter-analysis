# Kickstarting with Excel

## Overview of Project

### The purpose of this project is to analyze how Louise's play "Fever" performed against similar Kickstarter campaigns. More specifically, launch dates and funding goals will be discussed in depth and their impact on the overall success of Kickstarter campaigns. Advanced Excel methods are utilized in this project to analyze over 4,000 Kickstarter data points. 
---
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
When comparing the 1369 Theater Kickstarters based on their outcomes and their launch dates, it is found that the **two most successful months are May and June.** There is a large dropoff in success rates after the summer, with November and December being the two lowest performing months. **Less than 50% of Theater Kickstarters are successful in December.** The first three months of the year can be expected to have an average success rate. The graph below illustrates these outcomes across all years, with the y-axis indicating the number of campaigns.
![Theater_Outcomes_vs_Launch](https://github.com/Mishkanian/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
For this section, the data is based only on Kickstarters that are considered "Plays," which are defined as a subcategory of "Theater." Unsurprisingly, the highest success rate of these campagins are for those with the smallest funding goals. **Kickstarter Plays with funding goals under $1,000 had an overall success rate of 76%.** Interestingly, there have been 0 canceled "Plays" Kickstarter campaigns, which may be a result of the small data set. It should be noted that due to this small data set, the success of campaigns with funding goals between $25,000 - $50,000 cannot be commented upon. However, the data does suggest that campaigns with **funding goals greater than $50,000 mostly fail with success rates of only 13%.**
![Outcomes_vs_Goals](https://github.com/Mishkanian/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
There were a variety of challenges in this Project related to Excel formulas, creating tables, and graphing. Knowledge of central tendency and measures of spead are required. The tools and formulas necessary to undertake this project in Excel include: Sort & Filter, PivotTables, PivotCharts, IFERROR, ROUND, COUNTIFS, QUARTILE.EXC, STDEV.P, SUM, AVERAGE, MEDIAN, DATE, and YEAR. Additionally, VLOOKUP was used to quickly generate data for individual indivdual entries that our client, Louise, wanted to learn about.

An interesting challenge that I encountered in this project was converting campaign launch and deadline dates from their original Unix timestamps into more readable data (MONTH/DAY/YEAR). Unix timestamps are measured as the number of seconds since January 1, 1970. This can be converted with the following Excel formula: =(((unix/60)/60)/24+DATE(1970,1,1))


## Results and Conclusions

Based on the analysis of Theater outcomes in relation to their launch dates, it can be concluded that the best month to begin a Theater Kickstarter campaign is in May. It is also important to avoid campaigns during the winter months due to their historically subpar performance.

As a general rule, the campaigns with smaller funding goals have a higher chance of success. This is especially true for campaigns with goals under $1,000, which have had the highest success rates. It is also advised to avoid goals above $50,000 due to their extremely low chances of success.

The primary limiations of this analysis that I have enocountered are the size of the data set and the categories of data that is available. Some important categories of information are missing, such as the Revenue and Critic Ratings. For example: In the case of "Theater" Kickstarters, it is not certain if a fully funded campaign was well received critically or how long the "Plays" lasted after being funded. It is also unclear how well these successful Kickstarters performed financially. What percentage of these plays were well received critically? How many of these "successful" Kickstarters underestimated their necessary funds? How many Theater plays are financially sustainable in the long term? More data is required to answer these questions.

Other possible tables and graphs we could create using this data set include the success rates of competing categories to identify the Kickstarters with the highest chances of succes. This information could be used to guide Louise when choosing her next project. It could also be interesting to find out if there is a correlation between the number of backers and success rates by generating new tables and charts. If a positive correlation is found between backers and success, then it may indicate that having a Kickstarter with wide appeal, rather than niche, is advantageous.
