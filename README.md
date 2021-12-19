# Crowdfunding for "Fever"

## Overview of Project
Louise, a playwright, wants to produce a play titled "Fever". She estimates that the project will cost $10,000. She aims to crowdfund the sum. She would like to get recommendation based on cowdfunding campaign data on how to make her campaign a success.

### Purpose
The purpose of the analyses is to use data on over 4000 crowdfunding campaigns between 2009-2017 to advise Louise on campaign strategy. The data include campaign goal and pledge, start and end date, and campaign categories and subcategories. 

## Analysis and Challenges
To look at campaign outcomes based on the type of the project and when the campaign was launched, new columns was created by splitting category and subcategory of projects, and by converting campaign start and end date to standard date format. 

Next, Pivot tables and accompanying charts were generated to see how campaigns performed depending on type of the project. The chart shows that most campaigns were for theatre projects where there are more successful campaings than failed ones.
[SCREENSHOT]

As we drilled down with another pivot table with subcategories of the theatre category, we see that most campaigns are for projects in the play subcategory. Unfortunately, in the play subcategory, there are almost twice as many failed campaigns as successful ones.
[SCREENSHOT]

The most challenging part of the analyses was to use the excel COUNTIFS function for the table by goal amounts. This was overcome by following the lesson carefully and spending time to understand the syntax well. 

### Analysis of Outcomes Based on Launch Date
A pivot table which pivots on category and year was prepared where the rows give us numbers of successful, failed and canceled campaigns by months of the year. A line chart was generated based on this table.
[SCREENSHOT]

The table was pivoted to show data by theatre category only. The line chart, as a result shows relationship between campaign outcome based on which month of the year they were launched in.

### Analysis of Outcomes Based on Goals
Since Louise' project is a play and she needs to raise $10000, we preapared a table on campaigns for subcategory play by goal amount. The goal amounts were grouped into 12 ranges starting at less than $1000 to more than $50000 to show numbers of successful, failed and canceled projects and their percentages. A line chart visualizes the data.
![Outcomes_Goals](C:/Users/Nimme/Documents/MODULE 1_CHALLENGE/Resources.Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

## Results
### Outcomes based on launch date
From the analyses of outcomes by launch date, we see that campaigns launched in May had the highest rate of success. The adjacent months also do well. The worst time to launch a campaign seems to be between August and January with campaigns launched in December producing more failures than success.
[SCREENSHOT]

Now we narrow it down to theater category by pivoting the table. May is still the best month to laumch a campaign and the trend is even more pronounced in the theatre category. The worst months to launch a campaign for a theatre project are the colder months and December in particular.
[SCREENSHOT]

Based on above finding, we would suggest that Louise launches her campaign between May and June but no later than July.

### Outcomes based on goal
From the analyses of outcomes based on goals, we see, not suprisingly, that at least three out of four campaigns for plays with less than $5000 as goal succeed in raising the sum. The rate of success then drops sharply as the goal amount increases and after $15000, there are more failures than success.
[SCREENSHOT]

The range we are interested in is $1000-$15000 since this is how much Louise needs to raise. It's evident from the chart that there are almost as many successes as failures in this range.

Based on above finding, we would advise Louise that while it's possible to raise the $10000 she needs, it will be challenging.

### Limitations
One of the limitations of the dataset is that, for successful campaigns, the date of reaching the goal amount is not available. This information would be useful in advising Louise on ideal campaign duration.

Also, the dateset contains no metadata with description of the columns. Some of the columns are self-descriptive. But it's not clear what "staff_pick" and "spotlight" mean so these could not be considered in the analyses.

Finally, the amounts are reported in a few currencies but exchange rate or conversion to USD is not provided. This makes the analyses by goal amounts flawed.

### Recommendation
Further analyses Louise can benefit from may include:
* descriptive statistics table with median and quartiles of successful and unsuccessful campaigns' goals;
* table and chart on plays (within theatre category) outcomes based on launch date (since Louise' project is a play);
