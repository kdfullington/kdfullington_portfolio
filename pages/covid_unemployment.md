---
layout: page
title: "Covid Unemployment Project - R"
permalink: https://kdfullington.github.io/covid_unemployment
---

**Unemployment During the Covid-19 Pandemic**

**Introduction**

In March of 2020, a virus called Covid-19 started appearing at alarming rates in the United States after
ravaging much of China and East Asia. Health officials encouraged the government and businesses to
implement lock-downs to prevent the spread of the virus, for which there was no vaccine. The idea was
resented that we could flatten the curve (of the number of cases) and prevent our vulnerable health care
system from complete collapse as hospitalizations drastically increased. For roughly three months or less,
many businesses closed their doors or implemented strict social distancing policies. Many people stayed
primarily in their homes and many large companies initiated teleworking policies. Among the hardest hit
usinesses were restaurants, bars, clubs and others that depended on serving as many people as possible in
enclosed spaces.
While many people chafe at being confined to their homes, perhaps a more important impact of the pandemic
has been on employment. Starting in March of 2020, many large companies began to lay off their workers,
citing decreased profits or other issues caused by the pandemic. Based on numbers from the U.S. Bureau of
Labor Statistics, the overall employment rate decreased from 60.7% in the second quarter of 2019, to 53.0%
in the second quarter of 2020.[https://www.bls.gov/spotlight/2022/demographic-changes-in-employment
during-the-pandemic/home.htm]

**The Problem Statement**

One obvious risk-factor for unemployment during the pandemic was industry. As mentioned in the introduc
tion, those working in the food and service industries were likely to be let go due to the conditions created
by the pandemic. On a more micro level, I wanted to know what other characteristics were risk factors for
job loss during a situation such as this pandemic. Specifically, what demographic traits (gender and/or race)
were the strongest indicators for employment status during the widespread illness?

**Addressing the Problem Statement**

To address this problem statement, I first went to the U.S. Bureau of Labor Statistics to gather data. I
downloaded the tables that addressed demographics and employment status from 2019, 2020, and 2021.
Having data from multiple years to compare would make drawing comparisons easier than analyzing only
2020 (the year the pandemic began). Once I had the data sets, I read them into RStudio and cleaned the
data. I separated the specific data I was most interested from the large amount of statistics collected by
the Bureau. I made several different data frames, dividing the data into the following sections: white men,
white women, Black men, Black women, Asian men, and Asian women.
I did this for three years: 2019, 2020, and 2021. I analyzed 2019 to get a sort of baseline example of years
without pandemics such as Covid-19. Evidence shows that the unemployment rate gradually shrank as the
pandemic went on and we were faced with the choice of whether to continue implementing the strictest
safety measures or to continue making a living. So, 2021 provides more of an idea of what the baseline
unemployment would be during an extended pandemic.

After splitting off the data intosections and years, I used the sections to create charts and plots that could be compared to one another. I was hoping to perform a logistic regression or test for correlation, but as will be discussed in the limitations section, the data I was able to obtain did not make that possible.

**Analysis**

2019 Unemployment

![Graph](assets/images/covid_unemp_gen&race2019.jpeg)


2020 Unemployment
![Graph2](assets/images/covid_unemp_gen&race2020.jpeg)


2021 Unemployment
![Graph3](assets/images/covid_unemp_gen&race2021.jpeg)


**Implications**

Based on the data I analyzed in this paper, we see that unemployment for Black men and Black women is consistently the highest. Even when unemployment for other demographics increased, it remained the highest for these two groups. Additionally, we can see from the bar charts that even as unemployment decreased in 2021 unemployment for these groups remained high. In fact, it looks as though unemployment was close for all groups in 2020. But as people in those demographics returned to employment, unemployment for Black men and women remained high. 

More analysis is needed to discover the specific reasons that unemployment for Black men and women is so high compared to other demographics. Potential influencing factors that were left out of this analysis include job industry and age.

**Limitations**

One limitation of the analysis I performed was access to data. I would have liked to explore the impact on other ethnicities, in particular that of the United States' indigenous population, otherwise known as Native Americans. I suspect that this population was the hardest hit by pandemic unemployment (perhaps excepting Black women), but from the data I had there is no way to prove this. On the section of data I analyzed, there was also no information on Hispanic/Latinx populations.

Another limitation was the number of years analyzed. Many, many factors influence unemployment rates in the US. It is hard to say whether 2019 was a good baseline from which to get a "standard" unemployment rate. If this problem is ever to be analyzed in more depth, it would probably be good practice to analyze unemployment from many different years to account for the variability and changing factors that go into predicting what the unemployment rate will be.

Additionally, the data from the Bureau that I was able to analyze shows unemployment over a full year. This does not account for the level of variability caused by the pandemic. For instance, Covid-19 cases do not appear at a consistent level. Rather, they rise to peaks and fall to valleys over time. Notably the case numbers rise during the colder months and fall during the warmer months. Consider the nature of food service jobs. They are often part-time and heavily dependent upon the demand for the services the business provides. When case numbers peak, cities and various levels of government implement mask mandates or other measures. This impacts the level of demand there is for certain types of professions. For instance, in the food service industries it is likely that fewer customers will eat indoors or even go to restaurants at all. This decreases the demand for employees such as waitstaff, and can lead to layoffs. Thus, it would be important for a more accurate analysis to analyze the data for smaller time frames. 

Finally, it turns out that information on the specific results of surveys about unemployment and demographic factors are rather difficult for a non-government employee to obtain. I would have preferred to work with a large table with yes or no answers and rankings. I was planning to do a logistic regression in order to predict risk of job-loss based on demographic traits, but I do not have the right data to perform the regression.

**Concluding Remarks**

My first step were I to pursue modeling this data, would be to get my hands on specific survey data. This type of data would include individuals answer selections, primarily yes/no questions. This would make it suitable for logistic regression in addition to correlation tests.

Once this data was obtained, I would use the techniques I learned in this course to discover any significant correlations in the data (between industry and ethnicity for instance). Then I would choose a number of variables to attempt to predict based on those correlation tests. 
