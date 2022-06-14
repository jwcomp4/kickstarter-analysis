# kickstarter_analysis
Performing analysis on Kickstarter data to uncover trends - bootcamp
# Kickstarting with Excel

## Overview of Project

This project assists Louise plan and execute a successful Kickstarter campaign for her production of *Fever* by investigating previous Kickstarter campaigns. The following includes a summary of the analysis that examines campaign outcome compared to goal in addition to campaign outcome compared to launch date. This analysis includes visuals, recommendations for Lousise, and possible next steps.
 
### Purpose

After nearing her funding goal shortly after her campaign's launch, this analysis takes a closer look at campaings for plays as they relate to their stated goal and campaign launch date.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

For this analysis, I created a pivot table that allows for filtering by Parent Category and Year. The rows contain the month of the campaign launch date, while the columns consist of the campaigns outcomes sorted by the successful outcomes in descending order. Creating this pivot table involved using the YEAR() function to extrapolate the campaing launch year from the Date Created Conversion column and creating a discrete Year column within the Kickstarter dataset. This pivot table enables me to create a line graph that visualizes that May and June are the best months to initiate a Kickstarter campaign.

![Outcomes vs Launch Visual](/resources/Theater_Outcomes_vs_Launch.png "Theater_Outcomes_vs_Launch")

### Analysis of Outcomes Based on Goals

To perform this analysis, I created a new sheet that allowed me to organize the data to show ultimately the percentage of successful, failed, and canceled campaigns related to a range of funding goals. Using the COUNTIFS() function allowed me to pipe the data into the appropriate rows and columns from the Kickstarter dataset based on funding goal, outcome, and the play subcategory. From this new table, I created a line graph that visualizes the outcomes based on campaign goal with Goals on the X-axis and Outcome Percentage on the Y-axis.

![Outcomes vs Goals Visual](/resources/Outcomes_vs_Goals.png "Outcomes_vs_Goals")

### Challenges and Difficulties Encountered

- Need to ensure that formulas in new sheets capture the correct data from the dataset.
    - This involves double-checking formulas capture accurate ranges and fulfill desired conditions.

- Need to ensure that tables are formatted to communicate visualized data clearly and accurately.

## Results

### Outcomes Based on Launch Date Analysis conclusions:

- Generally, more theater campaigns succed than fail with the late Spring being the best time to start and the end of the year being the worst time to start a Kickstarter campaign for a theater production

- May and June have the highest percentage of successful outcomes for theater Kickstarter campaigns with May being the best month to initiate a campagin. 
    - Also note that May has the highest number of Kickstarter campaigns for theater productions initiated.

- I recommend initiating the Kickstarter campaign in May.

### Outcomes Based on Goals Analysis Conclusions:

- Kickstarter campaigns with goal range of less than 1000 are 76% successful and campaings with goal range of 1000 to 4999 are 73% successful.
    - Note that the 1000 to 4999 goal range has 388 successful campaings compare to 141 successful campaigns in the less than 1000 goal range.

- From there, percentage of succcessful campaigns drops percipitously until goal ranges of 35000 to 39999 and 40000 to 45999. Both of these goal ranges are 67% successful.

- I recommend setting campaign goal either in the range of 1000 to 4999, while considering and weighing the risk of a larger production with goal range of 35000 to 45999.

### Dataset Limitations and Possible Analyses 

#### Dataset Limitations

- One limitation of the dataset is it does not capture the primary means of marketing the Kickstarter campaign. 
    - Having this information could help determine if marketing strategies and incentives affected campaign outcomes.
- The dataset also does not communicate if the campaign took place in a rural or urban community. The milieu of the campaign could affect both the goal size and the campaign's outcome.

#### Other Possible Analyses

- Finding descriptive statistical measures for the campaign goal related to outcome could reveal the central tendency and spread of the data to help better determine a successful goal amount.

- Providing an analysis of the goals and outcomes filtered by country could help Louise understand how best to carry out her campaign. 

- Providing an analysis based on the outcomes related to the length of the campaign could help Louise discern how long to run her campaign.
