# Kickstarting with Excel

## Overview of Project
### Purpose
This project deals with a large amount of data for Kickstarter fundraisers for a variety of purposes.  The goal here was to help an imaginary friend to analyze the data to determine what they should do to have the most chance at success for the various types of Kickstarter campaigns they were interested in.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
The graph below shows the results of the Kickstarter data for theaters campaigns broken down by the month that the campaign was launched and whether the campaign ended in success, failure, or was canceled.  From the graph, it is evident that the most successful month of the year to launch a theater Kickstarter was in May and the least successful month was December.  It is also easy to see that the number of failed and canceled theater Kickstarters does have some variability from month to month but those two remain much more consistent than the successes.  Thus, the reached conclusion is that the best month to start a theater Kickstarter would be in May with each successive month lowering the chance of success for the remainder of the year.
![Graph 1](/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The graph below shows the outcome of the Kickstarter data for plays categorized by the amount of the goal.  The first thing to notice is that none of the Kickstarters here were canceled.  In other words, they were all either failures or successes.  From the graph, it is apparent that the categories of less than 100, 1000 to 4999, 5000 to 9999, 10000 to 14999, 35000 to 39999, and 40000 to 4499 have success rates that exceed that of the chance for failure.  Or in other words, the chance of success for each of those categories is higher than 50%.  Interestingly, the category 15000 to 19999 is a 50/50 split for success and failure.  For the other categories, the chance of failure is higher than that of success.
![Graph 2](/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
I did not run into any issues during this analysis that I did not overcome quickly.  I can easily imagine that someone inexperienced with Excel might run into problems using the COUNTIFS command.  The important thing to remember if that this command will count everything in the given range the satisfies all of the given conditions.  For example, to count the number of successful play Kickstarters with a goal of less than 1000 I used the command =COUNTIFS(Kickstarter!P:P, "plays",Kickstarter!F:F, "successful",Kickstarter!D:D,<1000).  The first part of narrowed the count to plays, the second part narrowed the plays down to successful, and the final part of the command narrowed the count to those with a goal of less than $1000.

## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?  
From looking at the graph, it is evident that the most successful months for theater Kickstarters is in the month of May and then there is a decline for the rest of the year.  On the other hand, the number of failed and canceled theater Kickstarters remain fairly consistent.  There is of course some month-to-month variation, but it is not as pronounced as it is with the successes.

- What can you conclude about the Outcomes based on Goals?  
The big conclusion from this graph is that goals in the following categories have a higher than 50% success rate: less than 100, 1000 to 4999, 5000 to 9999, 10000 to 14999, 35000 to 39999, and 40000 to 4499.  The other categories have success rates that are less than or equal to 50%.

- What are some limitations of this dataset?  
One of the limitations of this dataset is that we do not know the source of the data.  Was this all from one source?  Multiple? Who knows? Moreover, what type of Kickstarters were these?  Online? Donate in person? Donate by phone?  Featured on TV? Again, who knows.  Knowing both would help improve the credibility of the data.

- What are some other possible tables and/or graphs that we could create?  
I think it would have been helpful to do a month-by-month breakdown of the plays data as well to see if there are any trends there.  Additionally, I think the analysis would benefit from a goals breakdown of the theater data as well to see if goal amount and success are correlated or not.
