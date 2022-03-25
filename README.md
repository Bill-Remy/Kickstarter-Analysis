**Kickstarter Analysis – Determining Impact of Launch Dates and Goals on Fundraising Campaigns**

1.0  Project Overview and Purpose
The project initiator, Louise, wants to understand how the success for fundraising campaigns is impacted by timing and published goal.

The purpose of the project is to examine a dataset of prior projects from multiple countries to determine the following:
- How does the timing of campaign launch impact the success of the “Theater” projects?
- How does the published goal impact the success of “Plays”?

3.0 Analysis and Challenges
The approach to analyzing the dataset was separated into two elements of work to align with the stated purpose.  Prior to starting the analysis, some additional fields were created to facilitate the analysis.  Specifically, the Category/Subcategory column was separated into unique “Parent” and “Subcategory”.  
Parent	Subcategory
film & video	television

Next the dates for launch were in Unix format and had to be converted to usable data formats along with creating a “Years” specific column.
launched_at	Launch Date -  Converted	Years
1434931811	6/22/2015	2015
1485872683	1/31/2017	2017

3.1  Impact of Launch Data on Campaign Success
To determine the impact of launch date on campaign success a pivot table was create that specifically examines various campaign outcomes by month for all years in the dataset.  The data was filtered to only include “Theater”  Parent category.   The specific pivot table is shown below along with a graphical representation of the data.

Table 1 Pivot Table of Outcomes Based on Launch Date
             

	3.2 Impact of Goal versus Outcomes for Plays
	The approach for understanding how outcomes were related to goals, a stratified review of outcomes versus goals was used.  Goals were divided into a total of twelve groupings starting with Goals less than $1,000 to greater than $50,000 in $5,000 increments.  The data was group only for the subcategory of “Plays” based on the scope of the project.  Campaign outcomes were categorized as “successful”, “canceled” and “failed” within each bucket by size of goal.  See Table 2 below.
Table 2 Stratified Outcomes by Goal
          
Next the percentages by goal bucket for each outcome were calculated and graphed to understand the trends and draw conclusions.  




4.0 Analysis Results
4.1 Outcomes Based on Launch Dates
Successful fundraising campaigns appear to be highly dependent on launch timing.  From the graph it can clearly be observed that launching a campaign in the May to July time frame has significantly better outcomes than early or late in the year.  The number of failed and canceled projects are mostly flat throughout the year.  It does not appear that timing has a significant impact on whether a project is failed or canceled.  
Volume of projects increased dramatically during the middle part of the year.  Also, volume overall does not appear to impact outcome since the volume of successful projects goes up with volume while the canceled and failed  projects remain mostly flat.
	4.2 Outcomes Based on Goals
	Projects with smaller goals, less than $5,000 have significantly better outcomes, greater than 70% success rate.  As the size of the goal increases the percent of successful outcomes drops and is roughly a breakeven at projects with goals in the $15-20,000 range.  
	Projects in the $35,000 - $50,000 range performed similar to the small projects with a percentage of success around 66%.  Unfortunately, the sample of size of these projects is very small compared to the small projects, less than $5,000.  The total number of $35,000 to $50,000 projects was nine as compared to 720 small projects.   Clearly small projects have a much higher likelihood of success while the larger projects can yield high values but have lower success rates.
4.3 Limitations of the Data
The data spans several years and this analysis weighted all years equally.  It is possible that trends in successful campaigns would change over time as the population changes.  The sample size of larger projects was very small compared to the smaller projects.  It is difficult to fully predict the success of a larger project based on the data available. 

4.4 Additional Analysis
Further analysis could include the following:
•	Segmentation of projects by region to see how both size of project and timing vary
•	Segmenting project by Parent and Subcategory to understand the impact of launch timing and size vary
