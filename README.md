# Kickstarting with Excel

## Overview of Project
Performing analysis on Kickstarter data to uncover trends

### Purpose
This project is to support up-and-coming playwrite Louise complete a crowdfunding campaign for her play, *Fever.* The play is estimated to cost $12,000. The object is to analyze data related to theater-related crowdfunding campaigns in order to identify trends and determine recommendations for optimal success.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To analyze the outcomes based on launch date, I used an Excel Pivot table to count the outcomes over time based on the Date Launched - which was provided originally in UNIX format but reformatted to short date. The short date column was then used to establish a Years column, which was then used, along with Parent Category, as a filter for the Pivot Table. After filtering on "theater" and retaining all years, I created a Pivot Chart to visually describe the overall trend.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/87709841/135179176-905b1fda-b8f9-4187-a79f-de20af162516.png)


### Analysis of Outcomes Based on Goals
To analyze the outcomes based on fundraising goals, I segmented the fundraising goal amounts into categories and then used a COUNTIF() formula to determine the number of plays that either succeeded, failed or were canceled within that particular fundraising category. Additionally, I used the SUM() and AVERAGE() formulas to determine the total number of plays and the percentage of plays that succeeded, failed or were canceled. 
After completing this in an analytical table, I used PivotChart to show the trends of success or failure by fundraising goal.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/87709841/135179198-70aa6c64-2ade-4a9a-88e2-be30a6f817d7.png)


### Challenges and Difficulties Encountered
No challenges or difficulties were experienced in the analysis done on outcomes based on either launch date or goal. The potential for difficulty is higher on the outcome based on goal analysis, as this required a COUNTIF() formula that if not written carefully could impact the overall count and therefore incorrectly identify the trend. I think a bigger challenge in this analysis was the inability to identify more specific actions to guide Louise in her campaign, based on these two analyses. (The outcomes based on goals analysis indicated that a fundraising campaign at her goal amount of $12,000 had about a 54% chance of success, but no additional information could be gleaned on how to increase that.)


## Results

Based on the charts provided above in the Analysis and Challenges section, in reviewing the results of the outcomes based on launch date, the first conclusion is that the months of May and June appear to be the best months to launch a fundraising campaign, and the second conclusion that successful outcomes decrease over time, after that apex.

The Outcomes Based on Goals data demonstrates that the higher the fundraising goal, the higher the likelihood of campaign failure. Louise's goal fell into a range where trends showed a 54% success rate.

The dataset showed several limitations. The most noticeable problem with the dataset is are that it is small (4114 records total). The applicable subset of data - crowdfunding campaigns for plays - was even smaller (1066 records), creating the potential for unreliable conclusions. Additionally there were outliers present in the data that without proper management could also skew the results. The dataset is "dated" the latest year for campaign data is 2017, making this 4, nearly 5 years old.

Another graph that might be created to demostrate the viability of Louise's success might be a **Box Plot of Successful US Plays**, to keep the comparison to the geographic location and to see whether her fundraising goals fall within a reasonable area. A review of the **Subcategory Statistics** showed that US plays enjoy a higher success rate than their peer subcategories of musicals and spaces.


## Recommendations
Given Louise's estimation of a fundraising goal of $12,000, it is recommended that for highest success rate she should fundraise during the months of May and/or June. Lower fundraising goals do show a higher likelihood of success than higher goals, but there is evidence in the data of plays that shared her fundraising goal that met or exceeded that amount.
