# Kickstarting with Excel

## Overview of Project

## *Enter Purpose here* (change back to \#\#\#)

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To create an analysis based on launch date, filterable by subcategory and year, it was first necessary to calculate the year for each record.  That was accomplished by adding a new column with the title 'years' and year forumala `=year()` with creation date as the argument in each cell.  

![ss1.png](/resources/ss1.png)
--- 
Next a new pivot table was created in a new worksheet, later renamed 'Theatre Outcomes by Launch Date'.  Filters were added on the 'Parent Category' and 'Years' fileds. The 'Outcomes'field was added to the Values and Columns to report a grand total and counts by outcome.  The date created field was added to rows, with the year and quarter elements removed to yield each month in a row. 

---
![ss2.png](/resources/ss2.png)
---
The Parent Category filter was set to 'theater' to ensure the results were relevant to the project.  From there the line chart below was generated.

![Theater_Outcomes_vs_Launch.png](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
In order to create a graph of Outcomes Based on Goals, it was first necessary to create a new table to organize and calculate the outcome data.  Columns were created to count successful, failed and canceled projects according to the goal ranges in column A.  Limiting the results to the subscategory 'plays', therefore required three search constraints, Goal, Subcategory and Outcome.  This was accomplished with the `=countifs()` function as show in this image:

--- 
![ss3.png](/resources/ss3.png)
--- 

The total number of projects was calcualted as the sum of the three outcomes for each range.  Percentages for each outcome were calculated by dividing the outcome count by the total number of projects.  The formula `=b2/$e2`, which anchors the column refrence to the 'Total Projects' column, was entered in cell F2, then filled down and right to calculate values for each outcome/range combination.  The line chart below was generated from the resulting data.

---
![Outcomes_vs_Goals.png](/resources/Outcomes_vs_Goals.png)
--- 
### Challenges and Difficulties Encountered

## *Enter Challenges Response here*

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The number of failed projects is relatively consistent throughout the year.  Both the total number of projects and the number of successful projects increase in the spring and early summer, specifically the months of May, June and July, in descending order.  Based on this, May would be the best month to launch for Louise to launch a campaign.

- What can you conclude about the Outcomes based on Goals?

## *Enter Answer here*

- What are some limitations of this dataset?

## *Enter Answer here*

- What are some other possible tables and/or graphs that we could create?

## *Enter Answer here*
