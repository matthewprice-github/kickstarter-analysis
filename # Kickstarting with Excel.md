# Kickstarting with Excel

## Overview and Purpose of Project

The purpose of this project was to help a playwrite, Louise, utilize 
kickstarter data of art projects in order to better inform her decisions
when launching a crowdfunding campaign for her new play. By uncovering trends in the data, 
like the most successful launch months and goal targets, we can help Louise optimize her 
campaign for the highest chance of success. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
For this analysis, I charted outcomes of theatre kickstarter campaigns by month launched, in order to get a better sense of how timing
plays a role in campaign success. Looking at the graph, we can see that the month with the highest volume of successful campaigns is May. More generally, we can see the summer months typically have a higher volume of successful plays than other months. 

### Analysis of Outcomes Based on Goals
For this analysis, I graphed outcomes of kickstarter campaigns against their goal amount, while filtering for plays ONLY. This will 
inform us what goal amounts typically see success (or failure) for plays, and if Louise's original $10,000 goal for her campaign 
is an optimal target. Looking at the graph, we can see a rather mixed picture. It makes sense that goals with very low targets (less 
than $1000) generally are quite successful in meeting those targets. Conversly, goals with very high targets (greater than $45K)
are fair more likely to fail. 

What is interesting is we see a rather mixed bag in between those two ranges. The majority of plays with goals from $20-35K fail, but 
the majority of plays with goals from $35-45K succeed. 

### Challenges and Difficulties Encountered
I would say one challenge working on the "Outcomes Based on Goals" analysis was bucking the goal amounts. While we could hard code 
all the Countifs formulas with number values, it would be time consuming, and not helpful if we would want to adjust the size of the buckets
later. My solution was two extra columns (using the "text to columns" feature), with the upper and lower bounds of all the buckets, 
and referenced those cells when creating my countifs formula. That way I was also able the drag down the formula for each column, 
instead of hardcoding each cell. 


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

I would advise Louise that the summer (and optimally May), would be the best time to launch her campaign. I could also tell Louise that there are a higher volume of theatre projects launched in the summer. 

- What can you conclude about the Outcomes based on Goals?

Louise's original goal amount was $10K, and plays with goals of $5-10K generally succeed more often than they fail, so I would say that 
is a plausible target for Louise. However, I would also inform Louise that the smaller her goal is, the likelihood of success increases.
This is somewhat intuitive, but worth mentioning because the data also supports it.  

- What are some limitations of this dataset?

One big limitation of this dataset is we don't really have a window into the more subjective/qualitative aspects of these projects. 
Was a show successful because it had the optimal launch date/goal amount? Or was the show just very interesting to the audience at large, and therefore got more funding? We do have a blurb about each project, but It's hard for us to factor that into any meaningful analysis. 

- What are some other possible tables and/or graphs that we could create?

I could see geography as an influencing factor in kickstart success. A graph that charted project outcomes by country could be interesting. Similarly, It could be interesting to see a table that had average donation amounts by country could also be interesting, it could help answer the question: who supports the arts the most?  

Something else I was wondering while doing the "Outcomes based on Launch Date" analysis was how we could account for duration of the kickstarter campaign. Did some projects fail simply because they didn't have a reasonable deadline? What is the average duration of a successful campaign? We could easily create another column that would give the duration of the campaign, given the launch date/deadline columns.  