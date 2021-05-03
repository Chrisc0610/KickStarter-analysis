# Kickstarting with Excel

## Overview of Project

### Purpose
To help Louise visualize how different campaigns fared in realtion their launch dates and their funding goals.

## Analysis and Challenges
- In order to properly visualize the dataset by year, the original Kickstarter spreadsheet needed the following adjustments:
	* A new column named "Date Created Conversion" was made that converts The "launched_at" column from Epoch time to Date/Year using a formula.
	* Then a new column named "Years" needed to be created which only pulls the year out of the "Date Created Conversion" coulumn.
	* Finally Pivot Tables are created. 
	* The "live" catergory has to be been removed from the filter as this data may cause any chart to get skewed.
### Analysis of Outcomes Based on Launch Date
- This analysis was achieved by creating a pivot table. 
	* Then  I filtered out the Parent Catergory and Years from the original spreadsheet. 
	* I then created columns based of Succesful, Failed,Canceled and their Grand Totals.
	* the X axis is comparing it by months with the Values being Count of Outcomes. 
	* The picture below shows the comparison line graph that visualizes the data.
	* ! [Outcomes_Based_on_Goals](Outcomes_Based_on_Goals.png)
	
	
### Analysis of Outcomes Based on Goals
- Once I created a list of goals to be the referenced for the X axis of my chart. 
	* I created columns for the total percentages of Succesful,Failed or Canceled kickstarters.
	* I used a countifs formula to help me gather and split up the data based off the goals I created. 
	* Once I got the countifs calculated I totaled them up in a separate columns.
	* I used the totals to run a simple percentage calculation, to get the total percentage values.
	* The image below shows the outcome, notice how one line is stagnant at zero, this is due to there being no values for cancelled fundraisers.
	
### Challenges and Difficulties Encountered
- Some challenges that you may encounter.
	* You have to make sure that the proper catergories are filtered, as our data contained "Live" dataset. This would have skweed the graph.
	* For the outcomes based on goal chart the proper countifs have to be done otherwise the data would result would be in accuarte. the proper formula to search through the data.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	* Based out of the Analysis, It appears that launch dates during the summer spike up in funding for theater Campaings.
	* Failed outcomes are under 60, while canceled outcomes are under 7 with the exception of Janaury.
	* Based of this data Louise should look to launching her play in late may early june to maximized funding.
	
- What can you conclude about the Outcomes based on Goals?
	* Based of the data it seems there was a some back and forth between successful and failed outcomes.
	* The goldilock zone for goals would be from 35000 to 44999, this is the goal Louise should aim for.
	
- What are some limitations of this dataset?
	* Some limitiations are that the data is not a live dataset, therefor our numbers can get outdated rather quickly. 

- What are some other possible tables and/or graphs that we could create?
	* a circle graph detailing the total succesful, failed and canceled by sub catergories
	
