# Kickstarting with Excel

## Overview of Project

This project utilizes Microsoft Excel to analyze a large crowdfunding dataset.

### Purpose

An individual wishes to know how to optimize their upcoming fundraiser in order to achieve the best possible outcome. By analyzing historical crowdfunding data, we are able to draw some conclusions about the best time of year to launch fundraising campaigns depending on their category, as well as determining realistic goals in order to establish a budget, and also to maximize the chance for a successful campaign.

## Analysis and Challenges

We start off by reviewing the spreadsheet containing historical crowdfunding data to determine its size and the types of data used. It contains data for around 4000 fundraising campaigns across various categories (predominantly in the United States and Great Britain), including their respective goals, dates, outcomes and more. It's immediately obvious that some of the columns need to be converted to human readable dates, while others need to be converted to currencies. Some columns will need to be split into multiple columns to allow more specificity in our analysis.

![Screenshot Conditional Formatting and Filtering](https://github.com/bristlab/kickstarter-analysis/blob/main/Resources/Screenshot_Conditional_Formatting_and_Filtering.png?raw=true)

After we've given the spreadsheet a rough overview, it's time to start drilling down into the dataset to discover any patterns or trends it might reveal. We can do this by leveraging a very powerful function in Excel called PivotTables which, when used properly, allow the user to quickly organize and tabulate large datasets.

![Screenshot_PivotTable.png](https://github.com/bristlab/kickstarter-analysis/blob/main/Resources/Screenshot_PivotTable.png?raw=true)
![Screenshot_PivotTable_Settings.png](https://github.com/bristlab/kickstarter-analysis/blob/main/Screenshot_PivotTable_Settings.png?raw=true)

### Analysis of Outcomes Based on Launch Date

Once we've produced some charts based on our PivotTables, we can draw a few conclusions about the best time of year to launch a fundraiser for an upcoming theater event. Whereas the horizontal axis displays the number of campaigns per month, the vertical axis displays the number of campaigns that either succeeded, failed, or were canceled each month.

![Theater Outcomes vs Launch](https://github.com/bristlab/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png?raw=true)

From this visualization we can conclude that May is historically the best time to launce a theater fundraiser, followed by June and July. The month of October appears to be too late in the year to launch if we wish to ensure a successful campaign, and December is even worse.


### Analysis of Outcomes Based on Goals

We'll use another PivotTable to create a chart representing the percentage of fundraisers for plays which are successful based on their initial fundraising goals.


![Outcomes vs Goals](https://github.com/bristlab/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png
?raw=true)

The dataset indicates that fundraisers with smaller goals have a greater chance of success than fundraisers with larger goals. Interestingly, and perhaps counterintitively, we found that while the rate of success decreases as the goal amount increases, there appears to be a sweet spot between $35,000 and $45,000, beyond which the rate of success drops to approximately zero.

### Challenges and Difficulties Encountered

Due to the volume of this dataset, it can be difficult at first to gain an broad overview, so we use Excel functions like Conditional Formatting and Filtering in order to gain a better understanding of the data we're dealing with.

The PivotTable function is invaluable for digesting large amounts of data. While PivotTables can be rather tricky to set up, they are well worth the time. And from our PivotTables we can produce charts that help visualize the results of our analysis for our audience.

## Results

- We can conclude that a theater fundraiser should be launched in May to acheive the best result, and that December is historically the worst month to launch a theater fundraiser.

- We can also conclude that an ideal campaign goal is less than $5,000 because historically such campaigns have around a 75% chance of success. If the producer feels that a larger budget will be necessary, then they should try to aim for somewhere between $35,000 and $45,000, but any higher than that is likely to result in the fundraiser coming up short of its stated goal.

- While the dataset does seem pretty comprehensive, the biggest issue is that, according to the dates of the most recent campaigns, the dataset is not current. We know this because the most recent event fundraiser was launched several years ago in 2017. It's likely that the fundraising climate has changed drastically since then, so our conclusions might not reflect the current day reality.

- We feel that information about each campaign's advertising budget could paint a more complete picture. It's possible that some campaigns were successful primarily due to increased public awareness of their campaign. It's also possible that some campaigns succeeded due to current events surrounding the time of their launch which would have made the subject matter of the play more relevant to their respective audiences. Broader economic factors could also play a large part, although those could be much more difficult to quantify.

- Taking this analysis further, it may be insightful to create a chart that illustrates how many campaigns were successfully funded by many small "grassroots" contributions versus campaigns that were funded almost entirely by a few large donations.