# Feedback

STAT 201 group project.

## Mechanics

Okay.

## Reasoning

Abstract:

"Novel inferential techniques" --- are they really novel? Did you design new inferential techniques? "Novel" typically means that you're proposing a brand new method; do not claim to use novel inferential techniques if you're only going to use a basic hypothesis test. (Done!)

"Novel inferential techniques are applied to estimate the proportion of theft crime relative to all crime between now (2020) and the mean proportion of the past 3 years (2017 to 2019)." --- Are you using inferential techniques to do some comparison here too? After estimating the proportions, are you testing for differences? It is not clear from this sentence. (Done!)

Does "now" mean the start of 2020 or some other date (like March 1st)? (Done!)

Introduction:

"The City of Vancouver, specifically, enacted a freeze on the police budget in 2021 [CBC, 5]." --- Is this freeze coming after the end of your data? Do you have data for 2021? (Done!)

Based on the average incomes, is it clear that Marpole is middle class and Strathcona is lower class? These numbers seem quite close. (TODO)

"We can use the City of Vancouver's local profiles as they match the VPD's neighborhood classifications" --- So why not just use the VPD classifications? Is their classification more current than the 2016 data from the City of Vancouver? (Done!)

"How has the proportion of theft-related crime changed, if at all, in Vancouver during 2020, the year of the COVID-19 pandemic, when looked at across the full economic spectrum via three neighborhoods: Strathcona, Marpole, and Shaughnessy?" --- This sounds like you're looking at a change in proportion of theft crime over the year 2020. Previously it sounded like you were comparing the proportion from 2020 to the previous 3 years. I think this statement can be made more clear. (years added, done!)

"when looked at across the full economic spectrum" --- It's not clear if you're looking at proportions separately on each economic class, or combining them and looking at proportions across all three combined.
("the various strata", done!)

"We're considering our sample to be what is available in the Vancouver Police Department's database" --- Can you be more specific about what kind of data is actually available in this database? Does it include all reported thefts, or do you have reason to believe that there is some missing data? (Done!)

"our population is all actual crime that occurred in Vancouver, not just reported crime" --- Do you have reason to believe that the proportion of crime reported relative to all crime (reported or not) has been constant over time? Or do you think for some reason, that the amount of reported crime could have increased in 2020, which might skew your results? Some commentary here would be nice. (Done!)

"through our data set sample we'll be able to produce an estimate." --- so the data contains only reported crime and you want to estimate the true population proportion of thefts (reported or not)? How would you extrapolate from your data of only reported crimes to all crimes? Is there any previous work or related literature that could guide you on this? For example, it would be helpful if we knew that on average, in Vancouver, 80% of all crimes are reported -- or something like that. (done!)

OR are you assuming that the proportion of reported crime to all crime is constant over time, and you're using data from reported crimes to assess if the proportion of all crime has changed in 2020 relative to previous years?
Technically, do you need to assume that the proportion of reported thefts to all thefts and the proportion of all reported crime types to all crimes is constant over time? For example, would it be an issue to your inference if in 2020 thefts were just as frequent as previous years, but were reported less frequently. Meanwhile, other crime types were just as frequent as previous years, and were reported just as frequently. (TODO come back to this)

"We'll use data from 2017 to 2020." --- time intervals are usually written such that the upper bound is not inclusive. I think what you intended to convey was that you are using all data from Jan 1 2017, to Dec. 31 2020. Is that right? (yes, done!)

"Our random variable of interest is the difference in the proportion of theft-related crime with respect to all crime through COVID." --- Difference between what and what? Through COVID makes this sound like you're interested in the change of proportion of thefts throughout 2020. However, your next sentence makes it sound like you're comparing Pre-Covid proportion of thefts to 2020 numbers. (done!)

"We will be studying the change of this value from 2017 to 2020 across three different Vancouver neighborhoods" --- "This value" refers to the population parameter discussed in the previous sentence. But are you actually studying the change in only reported crime? Be careful to make the distinction if your data is only reported crimes, but you're trying to make an inference about all crime. (return to this sentence, but mostly done!)

Your SE formula should have the square root over the whole expression.
You should define p, q, and n in the context of your study.
(TODO: fix formula)

Preliminary Results:

"We chose three neighborhoods that we believe are representative of different economic classes present in Vancouver, in terms of median wealth:" --- previously you were looking at mean wealth (fixed!)

"We're hoping to compare crime rates across years in neighborhoods that represent a reasonable distribution of incomes." --- What is unreasonable about using the full dataset of all neighbourhoods? Don't all neighbourhoods give the true distribution of incomes in Vancouver? Selecting 1 neighbourhood of each "class" feels like you're artificially modifying the socioeconomic composition of your data to fit your belief about how Vancouver should be. What if, in reality, Vancouver is composed of many low income neighbourhoods and only a couple wealthy ones?
More justification as to why you select 3 neighbourhoods, of different economic classes, is needed. For example, do you plan to look at how theft rates have changed within different economic classes of neighbourhoods? Or are you trying to make sure you have a sample that is somehow representative of Vancouver and you're controlling for a lurking variable? If your goal is to quantify changes in theft rate in Vancouver, then why not use all data from all of Vancouver? (we just used all data)
Why these three neighbourhoods in particular? Yes, they may each be from a different wealth class, but there must be other ways to take a sample of 1 neighbourhood from each class. If someone was reviewing your work they would want to know why you picked these three and want to know that you didn't just cherry pick neighbourhoods that made your results more significant. (this will be changed)

"A line plot of total crime over time" --- Isn't your data only reported crimes, not total crime like you specified to be your population? (done!)

Should provide a year range on your stacked bar chart. (done!)

"30 items." --- Items means reported crimes? (yes, done!)

Your estimates break down proportion of theft crimes across neighbourhoods, but are the proportions out of the total number of reported crimes in all of Vancouver, out of the total number of reported crimes in these 3 neighbourhoods, or just within each neighbourhood? Make sure this is clear without the reader having to decipher your code. (added line!)

Methods:

"We're also using blocking in our analysis." --- Is there random sampling within blocks at all? It seems like you just hand picked a neighbourhood from each block.
(done kinda!)

"Crime has been linked to wealth (and more specifically, socioeconomic status, or SES) " --- If so, then why not use the full data of all neighbourhoods from Vancouver, rather than artificially creating a sample of neighbourhoods from different SES? Are you not changing the composition of SES, relative to the full data for Vancouver, by handpicking neighbourhoods?
(changed!)

"trust in police generally was found to be at a "record low" in August of 2020 [New York Times, 10]." --- Do you think these findings also apply to Vancouver police?
(TODO: find stats can article)

"Shaughnessy, for one, being at a rather high-end extreme of wealth, might be less useful in our analysis, as it doesn't really generalize to any kind of useful population outside of that specific neighborhood." --- So why did you pick it over another high income neighbourhood?
(TODO: fix neighbourhoods)

When writing hypotheses, be sure to define variables like p and delta p.
(TODO: define variables)

"We'll likely go with something like 10%, since we're working with a social science topic, and thus more variability is generally considered acceptable." --- Maybe provide some reference for this. It's good to cover your bases and be able to justify decisions like significance level, especially when it's not a standard one.
(TODO: re-write)

Which statistical test do you plan to use?

## Writing

While very thorough, your proposal is far too long. That said, the writing is very good. It reads nicely and is structured well.

"Novel inferential techniques are applied to estimate the proportion of theft crime relative to all crime between now (2020) and the mean proportion of the past 3 years (2017 to 2019)." -- Splitting this sentence into two could make it more easily decipherable.

"Note that two-tailed hypothesis tests are confidence intervals are practically equivalent " --- "and confidence intervals"