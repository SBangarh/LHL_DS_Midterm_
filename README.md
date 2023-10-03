# LHL_DS_Midterm_

## Project goals
1. I have a goal of improving my EDA as it is something I have struggled with in past projects.
2. I will also aim to use python best practices like OOP, 
3. I want to work on slowing down and really planning my approach in writing before doing any coding
4. I want to commit more frequently to github for this project
5. Have fun

## Process
I selected my data. Data selected pertained to civilian complaints against NYPD from 1985 to January 2020. Over 33,000 rows of raw data, some missing data related to race and sex, multiple officers had 0 as their shield number as well. Data was obtained from [propublica](https://www.propublica.org/datastore/dataset/civilian-complaints-against-new-york-city-police-officers) and there is additional information at the link provided. 

My data question was the following: What is the breakdown among ethnicity, age, and gender for complainants, and what are they outcomes for those groups in regards to the board and interaction with police. 

Prior to performing EDA, I wrote functions to use on my data. I also used some of these to perform QA later on.

I performed EDA on my data to identify nulls and duplicates. For the nulls there was a 92% or greater rate of nulls for the years 1985 to 1998, so I removed them from the sample. I also removed the year 2020 as there were only four rows. For the remaining nulls, I was initially going to impute values for the critical categories - complainant ethnicity, age, and gender - however, the nature of the data and topic made it difficult for my current skill set. These data points were still important, so I changed them to "No Records Available". This data can be easily impacted by biases and I didn't want to take that risk, especially since I'm still learning data science concepts. 

I cleaned the data removing nulls, duplicates, standardizing the data, and formating datatypes.

I saved my final data as a csv and from there I made a separate file with relevent data to be used in my Tableau dashboard.

I performed basic QA on my final dataset(final_df.csv) to determine the quality of my data. 


## Results
Dashboard 1 - Complaints
Of the 33,358 raw data point, 28,105 data point were left after cleaning. Of these data points, 36% of interactions resulted in no arrest or summuns, while another 30% was attributed to an arrest for an "other violation/crime". In every year, there were more resolved complaints than complaints made. The majority of complaints were due to an "abuse of authority" 50% with "force" second, 24%. Approximately, 75% of all board dispositions found the complaints to be unsubstantiated or exonerated, but exonerated was defined as "The alleged conduct occurred but did not violate the NYPD’s rules, which often give officers significant discretion over use of force." The remaining 25% were substantiated complaints. 

Dashboard 2 - Complainants
The majority of complainants were between the ages of 18 - 24 and were primarily Males (>60%) with black, hispanic, and white ethnicities. The breakdown among ethnicities throughout the years has been relatively steady with the exception from 1999 to 2007 where there was an increase every year. 

Dashboard 3 - Officers
Officers were primarily in the 24 to 44 age groups. The vast majority were Males among all ethnicities. There was a noticible change in the complaints against when comparing ranks at the time of incident where Police Officers accounted for almost 20,000 complaints. However, when viewing the current ranks, there was a greater diversification. It would be too great of a stretch to speculate as to why though. 

Dashboard 4 - Conclusions
This dashboard shows the ethnicity and gender of complainants, the board disposition, and ranks - current and at time of incident. A lot of this information - at a high level - was explained in the earlier dashboards. The purpose of this dashboard is relate elements of the previous three together. Across police ethnicities and genders for law enforcement, the predominant board dispositions were unbstantiated and exonerated and for the complaint outcome, the majority were no arrest/summons, arrest - other, summons - disorderly conduct, and summons - other. 

## Challenges
- Partner dropped out of the program 75% of the way through the project and I had to abandon some parts due to time. For instance, I did not build a model and my QA could have been a lot better.
- struggled with some logic in Tableau - I think I should have done all data related stuff in Python then moved over, not just EDA
- struggled to build a model with categorical data which was compounded by the sensitive nature of the data (e.g., ethnicity and police interactions)
- I found the data was slightly limited and would need to be combined with other data to get better insights. For example, location data so I could breakdown by neighbourhood, the perceived trust in police for each demographic.
- I did struggle with the data too, I found it slimy, like it could be used to fit an agenda very easily.
- I struggled with understanding what was under the hood in Tableau for more complex visualizations and was not entirely confident in what was happening.

## Future goals
- I would like to come back and spend more analyzing the data in python by developing metrics better metrics that I found difficult to do in Python.
- Develop a better plan, I find I'm not specific enough in my "to-do list" or goals and end up procrastinating due to a lack of direction. 
- I would like to combine this data with location data and perceived trust by demographics if possible
- understand the complaint process better to better understand the data
- I am going to re-do this project while also researching related data to better analyze the data set. 
