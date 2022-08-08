# GoogleDAcertificate_capstone
## My Google Data Analytics Capstone project

These Python scripts perform various analyses of the data from [Be Focused](https://xwavesoft.com/be-focused-pro-for-iphone-ipad-mac-os-x.html).

This repository contains three Jupyter Notebooks:
1. productivity dashboard
2. productivity analysis
3. weather influence


## Productivity Dashboard 

This script is intended to be run early in a month to analyze your productivity for the previous month, both in itself and compared with the previous year.

* Creates a bar chart of the number of intervals you completed for tasks that you consider most important for the previous month.

* Creates a bar chart showing the total number of intervals completed in each month for the previous 13 months.

![sample dashboard output](https://briandomino.com/images/monthly_dashboard.png)

(click to see the full image)

* Admonishes you if you did not complete at least one interval for each of your important tasks. For example: 
`You did not do even a single interval of the following: writing.`

## Productivity Analysis

Answers two questions: First, how diverse is each month in terms of the tasks completed? Second, to what extent were above-average and highly productive days due to work-related intervals? The answer to the first question is presented as a bar chart, and the second as three simple statements.

## Weather Influence

Looks to see if there is a correlation between day length and productivity. Answers this by calculating the Pearson's correlation coefficient and presenting both a scatterplot and a binhex plot.

## Requirements

* The scripts all use the Pandas and Matplotlib libraries.
* You'll need your productivity data in CSV form. Be Focused has an export to CSV function that does this, although your data need not be from that exact app. All you need is a CSV file with one column listing the date and the other giving the name of the task completed.
* The weather data I used was provided by the [National Oceanic and Atmospheric Administration (NOAA)](https://www.noaa.gov). You'll need to request a dataset tailored to your location and timeframe.

## Changes you will need to make

* If you want to run these notebooks on your own data, you will need to change the paths to the data files. These are in the second cell of each notebook.

* In the Productivity Dashboard, you'll want to change the list `most_important_tasks` to reflect which tasks are important to you.

* In Productivity Analysis, you'll want to change `only_work` to list whichever tasks are work-related.

## Learn more

If you would like to learn a little more about this project, please visit [BrianDomino.com/befocused_analysis.html](BrianDomino.com/befocused_analysis.html).
