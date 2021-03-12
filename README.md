# Kickstarter-analysis
## Project Overview
### Backgroud and Purpose
Louise is an up and coming playwright with a new play named "Fever". Louise is looking for a way to fund this play by starting a crowd funding campaign.
She has an estimated budget in mind, but she is hesitant about jumping both feet first into the sea of crowd funding without informed knowledge of how successful, or not, past crowd funding campaigns have been, particularly for plays.
The purpose of this kickstarter project is to help set Louise up for success by analysing historical excel data for past campaigns, to find if there are any specific factors that make a crowd funding campaign successful.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch dates
This particular analysis is to show relationship between outcomes and launch month of past campaings to help Louise make an informed decision, as to when to time her campign for most chances of successd by following the steps below;
* A pivot table from the KickStarter worksheet is created, and placed in a new sheet labeled "Theater Outcomes by Launch Date."
* The pivot table shows months (i.e. time in a year) on its rows, and outcomes (i.e. successful/failed/canceled/live) of campaigns in its columns
* The pivot table can be filtered based on "Parent Category" and "Years."
* Column labels is then filtered to show only "successful," "failed," and "canceled."
* A line chart is created from the pivot table to show the relationship between outcomes and launch month

- ![Thearter_Outcome_vs_Launch](https://github.com/Omodayo/Kickstarter-analysis/blob/main/Theater_Outcome_vs_Launch.png)

### Analysis of Outcomes Based on Goals
This particular analysis is done to visualize relationship between goal dollar amount (i.e. proposed budget) of campaigns and their outcomes to help Louise set a goal amount for her crwod funding campaing that will most likely provide her with the most chances at success by taken the steps below;
* A new sheet in the KickStarter worksheet, labeled "Outcomes Based on Goals", and new columns are created to help with the analysis
* In column "A", ranges were created to  group campaigns based on their goal amount.
* COUNTIFS() functions is then used to populate the Columns "B", "C" and "D" 
* SUM() function is used to populate column "E"
* Percentage of outcomes are then calculated in Column "F", "G" and "H"
* A line chart is created to visualize the relationship between the goal-amount ranges and the percentage of outcomes

- ![Outcomes_vs_Goals](https://github.com/Omodayo/Kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
* Due to the large size of the data available, one of the challenges encountered is how to ensure that the analysis is not skewed one way or another because of outliers. This obstacle was overcomed by using a box-plot to weed out any outliers
* Another challenge is how to filter the data to show only relevat data that are peculiar to the nature of Louise play. This is overcome by filtering the "parent category"  and "Subcategory" down to reflect only data relevant to Louise

