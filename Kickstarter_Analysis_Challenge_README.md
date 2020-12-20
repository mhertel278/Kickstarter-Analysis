# Kickstarting with Excel

## Overview of Project

Louise has started a Kickstarter campaign to fund her play *Fever*.  The campaign has quickly come close to reaching its fundraising goal. The purpose of the following analysis is to provide Louise with insights into the likelyhood of her campaign reaching its goal.  The analysis was performed on data in an excel spreadsheet for several kickstarter campaigns.  The data for each campaign included details such as Project Name, goal and pledged amounts, country in which the campaign took place, the outcome of the campaign, the launch and deadline dates, and category and subcategory of the project in the campaign.  

## Analysis and Challenges

In doing this analysis, I first examined how the time of year Kickstarter campaigns launched affected the out come of the campaigns.  Second I focused on how the amount of the campaign goals affected the outcomes.  

I focused on projects in the **theater** category.  The original data set listed category and subcategory in the same column ![category_subcategory_column](resources/category_subcategory_column.png).  I added additional columns to the spreadsheet and used the Text to Columns feature to split the category and subcategory information into the columns *Parent Category* and *Subcategory*.  ![](resources/parent_sub_category_split.png)



### Analysis of Outcomes Based on Launch Date

In order to examine how launch date affected the outcomes of Theater projects, I created a pivot table from the full data set. ![](resources/pivot_table.png)
I filtered the table to display only projects in the Theater Parent Category.  The month in which campaigns launched regardless of year are listed in the rows of the table, while the outcomes Successful, Failed, and Canceled are the column headers.  The values in the table show the count of Successful, Failed, and Canceled campaigns launched in each month of the year.  From this table I then created a chart to quickly visualize how the outcomes of campaigns differ throughout the year.  ![](resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

I then focused on how the amount of a campaign goal affected the campaign outcome.  I added a new worksheet to the workbook and created a table with ranges for the dollar goal amount of campaigns.  ![](resources/Table_Outcomes_vs_Goals.png)
I used the CountIfs function to populate the 'Number Successful', 'Number Failed', and 'Number Canceled' columns of the table.  For a given cell of the table, a campaign from the original data set in the Kickstarter Analysis worksheet would be counted by the CountIfs function if: it's goal fell within the range listed on that row, it's outcome matched the column, and the project's subcategory was *Plays*.  I then used these totals to calculate the percentage of campaigns within each range that were Successful, Failed, or were Canceled.  I created a chart to visualize the percentage of each outcome as goal amount increased to shed insight on how the goal amount would influence a project's success.
![](Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
