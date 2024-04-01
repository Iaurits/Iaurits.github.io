---
layout: post
title:  "A data-viz story about prostetution and types of arrest."
date:   2024-03-27 09:47:40 +0100
categories: homework
---

For this week's blog post we here at iaurits.github.io wanted to dive deep into the underworld of prostitution in San francisco, we have focused our attention to the data set from 2003 to 2018 [1]: Since this dataset is so comprehensive we need to have a general understanding of what the data set consists of. 
Each entry in the data set is an incident report, meaning that a crime has been committed. To that crime more data adheres such as the time of the incident and the type of incident. In this report we have decided to focus on only the crimes considered prostitution, and furthermore we looked at what kind of arrest it was, whether it is cited or booked. A cited arrest is an arrest where the arrested person has been given a fine or a warning, and a booked arrest is where the arrested person has been taken into custody by the police officer.


<iframe src="/figures/barplot.html"
    sandbox="allow-same-origin allow-scripts"
    width="150%"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>


In the plot above we notice that different times of day seem to have different rates of booked and cited f.x. from 1-4 in the morning it seems that there are more booked arrests than at other times. This might be because the more serious crimes are committed at night. Simply looking at the hourly crime rate might not paint a clear picture of the booked rate in San Francisco, therefore we decided to also look at the booked rates in different districts in the city.

We believe that some districts would have a higher rate of crime and also that the type of crime and punishment depends on the districts. Districts where the local police are understaffed and busy might have a tendency to have more cited arrests, since they may not have the manpower to book all arrests for lesser crimes. Below can be seen a plot of prostitution in San Fransisco where each area has been colored depending on the ratio between booked arrests and all arrests.


<iframe src="/figures/map.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="500"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>


Here we can see that areas such as Tenderloin, Central, Northern, Mission and Richmond tend to have fewer booked arrests for prostitution compared to the total number of arrest resolutions for prostitution. Areas such as Taraval, Park and Southern tend to have a higher booked rate. However, it is important to know that this rate is calculated in relation to only booked and cited arrests, so this plot does not indicate that there is more prostitution in the aformentioned areas, simply that more often offenders gets taken to the police station insted of getting fined. In fact areas where the rate is low could be because patrolling police are more busy or more needed on the road and therefore more often decide to let offenders off with fines as for example Tendorloin is a neighborhood notorious for criminal activity. The following plot shows prostitution arrests as a function of time. The x-axis is given in 24 hours and the y-axis as given as the years between 2010 and 2015. In the plot booked arrests and cited arrests have been colored differently. The plot allows the user to select specific points and then be shown data on these points such as date and incident.

<iframe src="/figures/prostitution_tenderloin.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

\

We notice from the prostitution related crime that most of the cited cases are loitering, it is most likely prostitutes who are fined by the police instead of being taking into custody. We also notice that the more serious crimes such as pimping and human trafficking are almost always booked. All of this supports our hypothesis that police in this area tend to focus more on the serious crimes and are more lenient towards less serious crimes. All of this might be due to the fact that Tenderloin has a high crime rate in general and police are understaffed in the area. An article from the San Francisco Standard made in 2023 explains how the police in the area has resorted to pulling back cops from retirement and discharged officers to do drug busts [2]. Another article from CBS News made in 2023 explains how the current major is requesting more funding to police departments, especially in Tenderloin in an attempt to combat drug issues in the area [3]. All of this might explain why police in Tenderloin generally tend to choose more lenient resolutions for crimes like loitering.

[1]: https://data.sfgov.org/browse?category=Public+Safety
[2]:https://sfstandard.com/2023/02/28/tenderloin-crackdown-brings-back-troubled-cops-dubious-covert-tactics/
[3]:https://www.cbsnews.com/sanfrancisco/news/san-francisco-crime-tenderloin-drugs/
