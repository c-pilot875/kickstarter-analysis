# An analysis of kickstarter campaigns
Performing analysis on Kickstarter data to uncover trends
## Findings
* Theatrical Plays in the US have significant successful campaigns on kickstarter
  - Best launch time is between April and June
* Theartrical Plays in Great Britian are also successful with lower campaign goals
  - Median campiagn goal around 4200
![Data Class Category Outcomes Graph](https://user-images.githubusercontent.com/115188500/196483612-50c90ae2-aefc-458f-82d3-78765a4f4b7e.png)
![Data Class Launch date Outcomes](https://user-images.githubusercontent.com/115188500/196483695-72a00bdc-c318-4939-a13d-e68a72fcb709.png)
---
## Suggestions
* Launch a play campaign in the US between April and June
* Budget around $4000 for the goal
---
# Kickstarting with Excel

## Overview of Project

### The purpose of this analysis is to compair the outcomes of play campaigns based on their fundraising goals and launch date. Team member request to analize different campaign outcomes based on their goals and launch date.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
* Created a pivot table of the Kickstarter dataset filtered by Subcategory "Plays" and "Year".
* Sorted Outcomes by decending
* Created a line chart to visualize the outcomes based on dates.
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/115188500/196557075-66f0d018-cf06-4c43-81bf-3eb3902beb41.png)
---
### Analysis of Outcomes Based on Goals
* Created a new sheet to count outcomes of the Kickstarter dataset organized by goal range 1000 - 50000 and filtered by subcategory "plays".
* Used the =countifs() formula with range1= Goal($ amount), range2= Outcomes (separated successful, failed, and canceled), and range3= Subcategory "Plays"
* Used the =sum() formula to calculate total project count taking outcome counts of successful, failed and canceled
* Calculated percentage of outcomes by using =value/value formula, taking the outcome count and dividing by the total project count. Rendered the percentage columns to percentage type to achieve correct numerical values.
* Created a line chart to visualize the outcomes based on goal amount. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/115188500/196557130-d1a1e9a3-2145-418b-9645-618d0dff970c.png)
---
### Challenges and Difficulties Encountered
* Difficulty encountered at first data points for counting outcomes. Resolved by adding a 0 to the first range in the count formula. (mistake was <100, fix was <1000)

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1 Peak success launch date for play campaigns are May, June, & July
2 Peak failure launch dates for play campigns are May, and October

- What can you conclude about the Outcomes based on Goals?
1 Campaigns ranging goals less than 5000 and between 35000 and roughly 45000 had seen the highest success rate while campaigns ranging goals between 20000 and 35000 and over 45000 had seen the most failure.

- What are some limitations of this dataset?
1 limitations to this data include range points for percentages or a corralation bewtween launch date success/failure and goal amounts.

- What are some other possible tables and/or graphs that we could create?
1 recommending graph to include most successful launch dates with goal range together.
