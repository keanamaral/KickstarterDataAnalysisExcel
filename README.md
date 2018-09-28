# Kickstarter Data Analysis

This is the main class repository. **Classwork** contains lecture slides, activities (including solutions), and other class material that will be updated after they are covered. **Homeworks** will contain the prompts for each assignment as well as their solutions.  

## Objective

To analyze kickstarter data in MS Excel using charts, pivot tables and regression analysis.  Summarize results in MS Word document.

## Background

Over two billion dollars have been raised using the massively successful crowdfunding service, Kickstarter, but not every project has found success. Of the over 300,000 projects launched on Kickstarter, only a third have made it through the funding process with a positive outcome.

Since getting funded on Kickstarter requires meeting or exceeding the project's initial goal, many organizations spend months looking through past projects in an attempt to discover some trick to finding success. For this week's homework, you will organize and analyze a database of four thousand past projects in order to uncover any hidden trends.

We are given a little over 4000 records to analyze.

## Dataset

![Kickstarter Table](ImagesforReadme/01RawData.PNG)

Dataset includes project name, description, funding goal in US$, money pledged in US$, `state` which is either `successful` or `failed` or `canceled`, country, currency, deadline date (timestamp), launched date (timestamp), category and sub category.

## Added Fields to Dataset

![Added Fields](ImagesforReadme/02DataColumnsAdded.PNG)

In order to do our analysis we added 6 fields: % Funded,	Avg Duration,	Category,	Sub-Category,	Date Created,	and Date Ended

We used formulas to calculate the values in these fields

![Calculated Fields](ImagesforReadme/03DataColumnsAddedFormulas.PNG)

Created a new sheet with a pivot table to analyze initial worksheet to count how many campaigns were "successful," "failed," "cancelled," or are currently "live" per **category**.

![Pivot Table 1](ImagesforReadme/04Pivot01.PNG)

In the same worksheet we also created a stacked column pivot chart that can be filtered by `country` and `parent-category` based on the dataset.

![Pivot Table 2](ImagesforReadme/05Pivot02.PNG)

Created a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.  And charted the results of the pivot table in a pivot chart to see trend by month

![Pivot Table 3](ImagesforReadme/06Pivot03.PNG)

Created a new worksheet to run an analysis using a table with 8 columns: `Goal`, `Number Successful`, `Number Failed`, `Number Canceled`, `Total Projects`, `Percentage Successful`, `Percentage Failed`, and `Percentage Canceled`.

We used this table to count how many successful, failed, and canceled projects were created with goals (Less Than 1000, 1000 to 4999, 5000 to 9999, 10000 to 14999, 15000 to 19999, 20000 to 24999, 25000 to 29999, 30000 to 34999, 35000 to 39999, 40000 to 44999, 45000 to 49999, and Greater than or equal to 50000).

Created a line chart which graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.

![Analsis Table](ImagesforReadme/07Analysis.PNG)

Ran 2 regression analysis to see if a statistically strong relationship existed to explain relationship between input variables

### Regression Analysis 1: If the Goal $s are higher or lower does it necessarily mean that the Pledged $s will have a relationship higher or lower?

![Regression 1](ImagesforReadme/08Regression01.PNG)

### Regression Analysis 2: If there are more backers will it result in more Pledged $s?

![Regression 2](ImagesforReadme/09Regression02.PNG)

Finally we summarize the results of our analysis in a word document.

![Results](ImagesforReadme/10Results.PNG)


