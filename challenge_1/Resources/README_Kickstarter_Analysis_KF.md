# Kickstarting with Excel

## Overview of Project
This project was an effort to analyze a dataset of Kickstarter campaigns across the globe and including multiple categories seeking funding. 

### Purpose
Two key takeaways from this data were to be produced:
---
1. How did campaign outcomes fare based on launch date - specifically, by month of launch?
2. What were the outcomes of kickstarter campaigns based on goal quantity. This was categorized into various ranges.

## Analysis and Challenges
The principal challenge of this analysis was encoutered while attempting to count the number of successful, failed, and canceled campaigns. This was difficult because the COUNTIFS funciton will process all data present, even if filtered/invisible. There are work arounds, such as SUBTOTAL and AGGREGATE, but methodically applying the filters as multiple criteria in a COUNTIFS formula will work. It is imperative to track across columns carefully though. Using the F4 key to toggle pieces of the formula to absolute was helpful in building the "Outcomes Based on Goals" sheet.



### Analysis of Outcomes Based on Launch Date
The Theater category was under the lens for this piece of analysis. Per the line chart that was produced, it is evident that the month of May exhibits the highest number of successful campaigns, while October gernerated the highest amount of failed campaigns. It should be noted that October shows the closest pass of "successful" and "failed", so it can be deduced that the ratio of success to failure is much smaller, independent of the shear quantity of campaigns launched.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/109499859/187087704-4fd39af3-aca1-497b-a9b0-31095176360e.png)


### Analysis of Outcomes Based on Goals
Perhaps predicatably so, lower goal values result in a higher incidence of success. Goals set at less than $5000 succeeded over 70% of the time. In the realm of campaigns for plays, success begins to noticebly dip above $5000 and slips below 50% success at the $20000 mark. Beyond the $20000 point, the total sample sizes of each campaign category are very limited. Therefore, simply saying that they tend to fail, while ostensibly the case, can not be said with extreme confidence. In the highest bracket, $50000 or more, the rate of success is poor. Only 12.5% of these high-goal campaigns were successful.

![Theater_Outcomes_vs_Goals]https://github.com/kelmo974/kickstarter_analysis/blob/main/challenge_1/Resources/Outcomes_vs_Goals.png

### Challenges and Difficulties Encountered
This project was fairly straightforward, but it wasn't without its potential pitfalls. One much be comfortable with stringing together multiple ranges and criteria in a COUNTIFS function and then meticulous enough to adjust across columns for specific conditional strings wihtout muddying the water.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. There is an uptick at which theater campaigns are launched during the late spring and into summer months. This trend is accompanied by an increased rate of success as well, which can be seen as the successful and failed lines show an increased distance from one another. 
2. Building on that, the number of successes relatives to failures is rather constant, independent on total launches, except for the increased success exhibited around the month of May.
- What can you conclude about the Outcomes based on Goals?
1. It is safe to conclude that a tipping point, of sorts, exisits somewhere in the $15000-$19999 range of campaings. The lines intersect here and success rates begin to be less common than failure. 
- What are some limitations of this dataset?
1. There are too few data points for larger sum campaign goals. With this sample size, it is imprudent to say that all larger sum campaigns are destined to fail. Further analysis to explain other reasons may be required. 
- What are some other possible tables and/or graphs that we could create?
1. Outcomes success/failure percentage in various countries.
2. Outcomes by parent category
3. Percent pledged above goal by parent category
4. Percent pledged above goal by country
5. Campaign backers by sub-category
