# Kickstarting with Excel
**This analysis was made with primarily focus on theater kickstarter campaigns**

## Overview of Project

This project firstly gathers pertinent data regarding the kickstarting world like for example: failures, successes and cancelations. In specific about the theater and being more precisely about plays or musicals. Secondly it also answers two questions the client had after recieving the first analysis. 

### Purpose

As mentioned before there are two main tasks so there are two purposes:

1. Perform analysis on Kickstarter data to uncover trends, evaluate and inform the client if a Kickstarter project is viable. As well, as running a second analysis to answer specific questions the client had afterwards the initial analysis was given.  

2. Answer the doubts that spawned after the first analysis: how different campaigns fared in relation to their launch dates and their funding goals. 

## Analysis and Challenges

**Start-First Anlysis**

### Viable Kickstarter information gathering

- While soting out the data down for the outcome of the parent category of the kickstarter data we are able to see that not only there has been a lot of campaigns for this category but actually it is one of the most successful in fullfilling their goals.

![Parent Category Outcomes](https://user-images.githubusercontent.com/110573146/191825388-edf2625a-4da7-4d55-a89d-1fb85dab7dc2.png)

- Further narrowing the information to country (US) and for theater we can see that the story repeats itself, it has a lot successful campaigns, which are good news! 

![Parent Category Outcomes US](https://user-images.githubusercontent.com/110573146/191825911-e423ea94-3083-43dd-bc2f-a64bdc90e642.png)

- Investigating a little further down we are able to see that from all the theater campaigns a good amount (671) are plays, and the 61.4% of those were successful.

![subcategory outcome](https://user-images.githubusercontent.com/110573146/191826689-01df361e-b18d-4c35-9151-5f0601613e1e.png)

- Now talking a little about the time, it was also investigated when the campaign should be held and how long it should last, **as it can determine its success or failure**. The main tendency throughout the years is that most of the successful campaigns were hold may and june so it is recommended to use this time period to hold the kickstarter campaign for a theater related event.

![Outcome based on launch date](https://user-images.githubusercontent.com/110573146/191828250-26174af3-1af2-4a08-bb31-0289e042afad.png)

- Finally using central tendency tools in specific data from the US, it can be determined that the Goal for the campaign must not be over 5000 US dollars but is is recommended for it to be about 3000 US dollars as it it both the median of all successful campaigns and for the successful pledged. Also a box chart was made to analyze the musicals in GB as they can be helpful as a comparison with our main focus, also as to use as a reference for future projects in this region. In the chart we can see how the information is a little skewed to the right as the mean is higher than the median which is explained by two points considered outliers which should not be considered for the anaylisis since one was to build a theater and the other was cancelled. The same can be said for the pledged category as the outlier is for the construction of a theater. With the other data now we can determine that most of the campaigns goals are way over the actually pledged so now we can decide a viable and real goal that can be reached, one taht at least 75% of all pledged data says that can be achieved something about $1,500

![Box plot GB musiclas](https://user-images.githubusercontent.com/110573146/191835807-435073e8-5f93-49f0-a127-2fc51087100f.png)

**Start-Second Analysis**

### Analysis of Outcomes Based on Launch Date

- For this part of the analysis it was necessary to create a create a graph that shows a more visually appealing result of all the kickstarters in the theater category by Launch date regardless if they were successful, failures or canceled. In other words it divides in "successful", "failed" and "canceled" the total amount of each outcome by month, this being the launch date of the kickstarter, **also it is importnat to mention that we used information from any year available for this graph**. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/110573146/193384155-db04f15f-7695-45f1-8b1b-d57d39b20161.png)

- In order to obtain this graph a pivot table was created by selecting the necessary information like the outcomes for the columns, the date for the rows, using especific filters for our data (so that it can be used to study other categories or different years). 

- So basically looking at the graph it is pretty obvious when it most convinient to start a Kickstarter (May) or in comparisson when to avoid starting it (October-December).

### Analysis of Outcomes Based on Goals

- In this part it was necessary filter the data and purify it, since we were going to work with only a part of the total data. Only the amount of kickstarters with each outcome was needed, but it was needed grouped in ranges depending on the goal amount of each one. 

- In order to achieve this it 12 ranges starting from less than a thousend to 50000 or more with a step of 5000 each, after this in order to obtain the information needed the COUNTIFS function was used to count the amount of kickstarters that checked all the criterias given: it was in the range in turn, it had the outcome in turn and it was under the "play" subcategory. Once the data was gathered a percentage was calculated, 100% being the total of the sum of the three outcomes.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/110573146/193392994-8c8e05f8-5125-42e8-8617-499586713b1a.png)

- A line graph was used to present the results of these percentages, which basically shows both the successful and failed kickstarters, but in detail since it shows how much money they had as goal. As it can be appreciated from less than a 1000 was the range with most successes. 

### Challenges and Difficulties Encountered

There were indeed challenges encountered for example:

1. Even though the instructions tells you how to do something. There are moments when it is your total responsability to find out how to do it by yourself so in times it gets a little frustating not knowing if what you are doing is correct. But in order to overcome it you just need to investigate a little more in Google, read with more attention or just trial and error since it is a valid way to learn. 

2. Managing time to do all the activities and deribables is also challenging as the course continous and there are other personal activities we have to attend. To overpass this hurdle it was needed to work each day a little in it so it was not as a demanding activity as it could be. 

3. In the Outcomes based on Launch date it was challenging trying to figure out which values to choose for the pivot table since the instructions did not tell you explicitely, but by reviewing a little back in the lessons it was possible to find out what to use for the table.  

4. For the Outcomes based on goals it was extremely challenging for me to get the COUNTIFS formula to work because my graph did not look as the example, so the debbuging lesson came to mind so I started checking for errors in the writing and there it was, instead of looking for subcategory "plays" I was looking for category "theater" so I learned to review everything even things you don't expect to be wrong. 

## Results

**First Analysis**

After all the investigation and findings provided, for a theater kickstarter campaign to be successful it is assumed that the US is a great region to have this project, as many have been successful before, but not only with stuff related to theater like building it but also for plays as 61% of all play's campaigns have been successful. From May to June is the time period which is the most successful for funding the play ** it is heavily recommended to use this time.** Finally a real achievable goal for a musical in GB as it was another interest of the client is $1,500 as 75% of all the musicals pledged at least this amount. 

**Second Analysis**

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The first conclusion wis that the best period of time to launch a theater based Kickstarter is near May, as it has the highest value overall with 111 successes. The second is that it is best to avoid launching at the end of the year, starting from october and ending in december or even january. So it is best to launch near the middle of the year. 

- What can you conclude about the Outcomes based on Goals?
It can be concluded that canceled values did not made any impact in the results, since there were none, but still it was necessary to include them in the calculations since it was a finding of the analysis. It was not expected. Also that there are two ranges that have the best chance to complete the goal, less than a 1000 (76%) or 1000 to 4999 (73%), the ranges from 35000 to 44999 are way to risky to take into account even though their percentage is of 67% that is because there have been a vey small amount of kicksstarters with those goals to even consider.   

- What are some limitations of this dataset?
It does not tell us how much money they made after debut, maybe it can be used to check the preferences of the audience. What is more appealing to them. It also does not tell us why some where canceled, maybe they ran into a common problem or why they failed, maybe they lost the director or staff or the way they were gathering the donations was wrong. These could have been an easy way to eliminate outliers. 

- What are some other possible tables and/or graphs that we could create?
A bar graph that shows how much support (backers) each category or subcategory had, as it would show what does people want to invest in and with this a pivot table also.    

A pie chart could be useful to show the percentages found in the outomes based on goals in an specific range to show with much more detail how it is arrenged.

A chart with multiple graphs could also work for the outcomes based by launch date as a more visually appealing look as it is easier to read and digest which month has the highest successful value and which ones don't. 
