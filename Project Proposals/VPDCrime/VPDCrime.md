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

The zip file from above contains a data set that has all crimes reported to the VPD.  

We have to conside that although the data set contains all the crimes reported to VPD, it does not represent all the crime that occured in Vancouver. Reported crime are a sample of all crimes occured in Vancouver, collected via people calling in to reported that a crime has occured. This means that there will be crimes that occured, and was not reported to VPD since people might not consider petty crimes to be worth the time involving the police.  That might be an inherient bias for us, as we are looking at if petty crime increased during 2020.  

That said, those bias might be mitigated since we are analyzing if the proportion of thefts increased in 2020 compared to previous years.  
Since proportion of thefts is calculated by (All reported thefts that occured)/(All reported crimes), there are two ways that might increase the proportion of thefts:

- The more thefts are reproted compared to the other crimes that are reported in 2020.
- Even as people report less crime, the amount of thefts that are reported is at least the same amount as previous years.

This means that unless there are other unforeseen reason of why people might change why they will report certain crimes and not other, as long as the ratio of reported thefts and actual thefts that occured does not change (an parameter that we cannot observe), we can assume that more theft has to occur for the proprotion of reported thefts to increase.

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
- West End
- Shaughnessy

As for right now, we will focus on Strathcona and have the other neighbourhood as further analysis.

We base our selection on of the neighbourhood base on the 'Average total income in 2015 among recipient'(ID#1858) as reported in Census Local Area Profiles 2016 from City of Vancouver[1].  The list above ranks the neighbourhood from the lowest average total income to the highest, with West End roughly at the median of all the neighbourhood.

While we have all the crimes reported of all in Vancouver, we don't actually have all the crime that occured in Vancouver;  we have a sample of crimes collected via people reporting it to the VPD.  There might might inherent bias in what type of crimes might be reported, as people might not think petty crimes are worth the time to call the police.  That side, we believe that IF petty crime was to increase, there should be more petty crimes reported in proportion to other crimes.  

Since we do not know the actual

## References

NEED TWO SOURCES WITH REGARDING INCREASE CRIME RATE
- maybe look at news report about increase crime?  then compare it to our data?

[1] Census local AREA profiles 2016. (2018, April 10). Retrieved March 06, 2021, from https://opendata.vancouver.ca/explore/dataset/census-local-area-profiles-2016/information/

Canada 2020 Crime &amp; Safety Report: Vancouver. (2020, June 19). Retrieved March 05, 2021, from https://www.osac.gov/Country/Canada/Content/Detail/Report/fd184899-ac3b-4e43-a31b-18f82fda35c4

City of Vancouver FREEZES police department funding as part of 2021 BUDGET | CBC News. (2020, December 09). Retrieved March 06, 2021, from  https://www.cbc.ca/news/canada/british-columbia/city-of-vancouver-freezes-police-department-funding-as-part-of-2021-budget-1.5833731

Sajan, B., &amp; Mangione, K. (2021, February 19). Hate crimes up 97% overall in Vancouver last YEAR, ANTI-ASIAN hate crimes up 717%. Retrieved March 06, 2021, from  https://bc.ctvnews.ca/hate-crimes-up-97-overall-in-vancouver-last-year-anti-asian-hate-crimes-up-717-1.5314307

Vancouver crime rate steady in 2020 compared TO 2019, according to new stats FROM VPD | CBC News. (2020, October 28). Retrieved March 05, 2021, from      https://www.cbc.ca/news/canada/british-columbia/crime-statistics-vancouver-2020-1.5779400

