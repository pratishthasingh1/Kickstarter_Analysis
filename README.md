# kickstarter-analysis
# Investigation of Kickstarter Campaigns Across the World
## Overview
A client, Louise, who believes her play will cost $12,000, asked for an analysis of all kickstarter campaigns to determine if her kickstarter will be viable. Additionally, she wanted to analyze what is it about certain campaigns that make them successful - looking at information such as the time of the year they are run, the duration of the kickstarter, or the goal/pledge ratio. 

## An analysis of kickstarter campaigns that allows us to see possible correlations between the outcomes of campaigns and their modality.
Analysis was performed using data inputted into Excel. 
It was first observed that from all the parent categories, theater kickstarter campaigns are overwhelmingly more successful than the other categories. After looking even more closely to theater, plays were almost two times as likely to be successful as they were to be failed. 
![Category_Of_Outcomes](https://github.com/pratishthasingh1/kickstarter-analysis/blob/master/Parent%20Category%20Outcomes.png?raw=true)

<b>This is good news!</b>

# Does time affect when theater kickstarter campaigns are more successful? 
It was important to see if time affected the success of campaigns, and if they did, then *when* were these theater campaigns are most successful? Using a pivot table, I filtered the parent category to only represent data from theater to further investigate. Summer, specifically May and June had the most amount of successful campaigns, 111 and 100 respectively. It is also important to note that the trend generally decreases after hitting its peak in May. 
![Outcomes_vs_Launch](https://github.com/pratishthasingh1/kickstarter-analysis/blob/master/Theater_Outcomes_vs_Launch.png?raw=true)

# Does the amount being asked affect the success rate? 
It was important to see if the goal being asked by these campaigns affect the success rate of them.
I made a table with the following headings in the columns and rows to see if certain ranges of goals being asked tend to be more successful, and *how* successful, in terms of percent.
If a campaign's goal was less than $1,000 to $5,000, it was mostly successful. However, the percent of campaigns being successful decreases every increment after, until it hits the range of $35,000 to $45,000. After this range, the trend shows a decline. 

![Outcomes To Goal Graph](https://github.com/pratishthasingh1/kickstarter-analysis/blob/master/Outcomes_vs_Goals.png?raw=true)

# Recommendations
I would recommend Louise to launch her kickstarter campaign in May, and to have it last at least until the end of the month. 
Something I would want to investigate more is finding out if the duration of the campaigns affected the success rate. With the failed campaigns showing a the highest number of failed campaigns also being in May, I think possibly adjusting the goal to be in a more favorable range may help. It seems that failed campaigns tend to have a higher goal, so I would possibly think about sticking to the ranges that were mentioned above. 

# Challenges
There was no data when I tried to make a pivot table to show plays that were canceled, no matter what range they were in. I tried to ensure my f(x) was correct by using sum f(x) to add up all the numbers in the column, and making sure that number was the same if I used =COUNTIFS(Kickstarter!$D:$D, ">0", Kickstarter!$F:$F, "failed", Kickstarter!$P:$P, "plays"). Both numbers yielded 0, which means there is no data on plays that were canceled.


# Results
## What are two conclusions you can draw about the Theater Outcomes based on Launch Date?
According to the data, launch date may impact the success of kickstarter campaigns. The most amount of successful plays were launched in May. However, it is important to note that May is also when the most amount of campaigns were canceled. The pivot chart shows the outcomes (successful and canceled) of the campaign generally follows the same trend over the year. Additionally, campaigns were generally canceled the most during January, but tended to be more stable the rest of the year, ranging less than 5 per month. 

## What can you conclude about the Outcomes based on Goals?
Generally it seems the higher the goals of a campaign, the less it's successful in yielding optimal results. There seems to be only a couple of optimal ranges where campaigns tend to do well, as previously mentioned. Outside of these ranges, it the success isn't that high, and the failed percentage tends to increase. 
This is possibly due to lack of confidence that the community may have in the play (or even knowledge), rendering it to go underfunded. The more affluent a person is, the more they are likely to invest in higher cost plays - unfortunately, there aren't a lot of affluent people that may help the other campaigns as well. 

## What are some limitations of this dataset?
One limitations may be that it's not clear what genre of plays tend to do well. This may also help Louise decide on whether her play will be successful (and if the genre of a play matters in May). 

## What are some other possible tables and/or graphs that we could create?
We can create pivot table to see the duration of these campaigns. This may provide an insight on how long failed campaigns are vs. successful vs. canceled. 
