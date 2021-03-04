# Crime Rate of Neighbourhoods Pre and Post 2020

## Introduction

2020 had impacted the lively hood of those that were fortunate and those that were already homeless.  In desperate times, Vancouver news outlet reported that crime hate has increased in Vancouver as people are trying to get their basic necessities met.  

In our project, we are interested in exploring the question: has crime rate in actually increase in Vancouver by a significant amount in 2020, as reported by the new outlets?

## Preliminary Results

## Methods: Plan

We will retrieve Vancouver Police Force's crime data from the link below:
http://geodash.vpd.ca/opendata/crimedata_download/crimedata_csv_all_years.zip?disclaimer=on&x=101&y=21

Inside the zip file, there is a CSV file call 'crimedata_csv_all_years.csv' with the following headers:

- YEAR
- MONTH
- DAY
- HOUR
- MINUTE
- HUNDRED_BLOCK
- NEIGHBOURHOOD
- X
- Y

To narrow the scope of our project, we will focus on these neighbourhoods and run individual analysis on the crime rate of those neighbourhood:

- Strathcona 
- Shaughnessy
- Marpole
- (Try to get a good spread of wealth of neighbourhood, since VPD bases their subdivision according to Stats Canada Census Division, we can use that to base our focus neighbourhoods)

Since we have the population of all crime reported in Vancouver, we will create a sampling distribution for 2020 and combination of 2019, 2018, and 2017(maybe? see if we need to do bootstrap.  If so, we can draw a sampel form the data set of the neighbourhood we are interested in and go form there).  

Using our distribution, we will find the proportion of Thefit related crime in 2017-2019 to use as our null hypothesis of what the crime rate in 2020 should be.  
Then we will run our analysis to see if there is a significant change in crime rate in 2020 (either increase or decrease) for our hypothesis testing.


## References

NEED TWO SOURCES WITH REGARDING INCREASE CRIME RATE
- maybe look at news report about increase crime?  then compare it to our data?

1. https://www.cbc.ca/news/canada/british-columbia/crime-statistics-vancouver-2020-1.5779400
2. https://www.osac.gov/Country/Canada/Content/Detail/Report/fd184899-ac3b-4e43-a31b-18f82fda35c4