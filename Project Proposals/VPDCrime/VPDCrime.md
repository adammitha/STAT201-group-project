# Crime Rate of Neighbourhoods Pre and Post 2020

## Introduction

In the past several months, multiple articles in the popular press have raised the issue of increasing crime rates in Metro Vancouver. The economic contraction of Covid-19 combined with fewer and more difficult-to-access resources for those with unstable housing has driven increase in property-related crimes. In addition, hate crimes have more than doubled across the board, with those of East Asian descent being impacted most significantly, likely due to the origins of the Covid-19 virus. These issues have led to a heightened concern in the general population about crime rates, which has caused significant tension between municipal governments and police departments with respect to funding cuts due to Covid-related drops in municipal revenue sources.

In light of these events, we are interested in exploring how much (if at all) crime rates have increased in over the last year. We will be using the Vancouver Police Department's open crime data to compare 2017-2020 crime rates in neighbourhoods across the income spectrum to assess just how much crime rates have changed over the past year.

In our project, we will explore whether theft increased as a proportion of all crimes from mean of 2017-2019 to 2020. We will also evaluate whether the spread of proportion, as measured by the standard deviation, changed between these two intervals.

## Preliminary Results

- Compute estimates for theft as a proportion of all crime
- Update graph to just show thefts

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
3. https://bc.ctvnews.ca/hate-crimes-up-97-overall-in-vancouver-last-year-anti-asian-hate-crimes-up-717-1.5314307
4. https://www.cbc.ca/news/canada/british-columbia/city-of-vancouver-freezes-police-department-funding-as-part-of-2021-budget-1.5833731