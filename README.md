# Kickstarting with Excel

## Overview of Project
Performing analysis on Kickstarter data to uncover trends

### Purpose
This project is to support up-and-coming playwrite Louise complete a crowdfunding campaign for her play, *Fever.* The play is estimated to cost $12,000. The object is to analyze data related to theater-related crowdfunding campaigns in order to identify trends and determine recommendations for optimal success.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To analyze the outcomes based on launch date, I used an Excel Pivot table to count the outcomes over time based on the Date Launched - which was provided originally in UNIX format but reformatted to short date. The short date column was then used to establish a Years column, which was then used, along with Parent Category, as a filter for the Pivot Table. After filtering on "theater" and retaining all years, the analyst created a Pivot Chart to visually describe the overall trend.

### Analysis of Outcomes Based on Goals
To analyze the outcomes based on fundraising goals, I segmented the fundraising goal amounts into categories and then used a COUNTIF() formula to determine the number of plays that either succeeded, failed or were canceled within that particular fundraising category. Additionally, I used the SUM() and AVERAGE() formulas to determine the total number of plays and the percentage of plays that succeeded, failed or were canceled. 
After completing this in an analytical table, I used PivotChart to show the trends of success or failure by fundraising goal.


### Challenges and Difficulties Encountered
No challenges or difficulties were experienced in the analysis done on outcomes based on either launch date or goal. The potential for difficulty is higher on the outcome based on goal analysis, as this required a COUNTIF() formula that if not written carefully could impact the overall count and therefore incorrectly identify the trend.


## Results

**What are two conclusions you can draw about the Outcomes based on Launch Date?**
The first conclusion is that the months of May and June appear to be the best months to launch a fundraising campaign.


**What can you conclude about the Outcomes based on Goals?**
The Outcomes Based on Goals data demonstrates that the higher the fundraising goal, the higher the likelihood of campaign failure.


**What are some limitations of this dataset?**
The most noticeable problem with the dataset is are that it is small (4114 records total). The applicable subset of data - crowdfunding campaigns for plays - was even smaller (1066 records), creating the potential for unreliable conclusions. 
There are outliers in the data, which needed to be managed.
The data is a dated (latest year for campaign data is 2017).


**What are some other possible tables and/or graphs that we could create?**
A graph that shows the relationship between backers and goals?


## Recommendations
Given Louise's estimation of a fundraising goal of $12,000, it is recommended that for highest success rate she should fundraise during the months of May and/or June. Lower fundraising goals do show a higher likelihood of success than higher goals, but there is evidence in the data of plays that shared her fundraising goal that met or exceeded that amount.