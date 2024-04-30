---
layout: post
title:  "A data-viz story about prostetution and types of arrest."
date:   2024-03-12 09:47:40 +0100
categories: homework
---

For this week's blog post we here at iaurits.github.io wanted to dive deep into the underworld of prostitution in San francisco, we have focused our attention to the data set from 2003 to 2018 [1]: Since this dataset is so comprehensive we need to have a general understanding of what the data set consists of. 
Each entry in the data set is an incident report, meaning that a crime has been committed. To that crime more data adheres such as the time of the incident, the type of incident, in this report we have decided to focus on only the crimes considered prostitution, and furthermore looked at what kind of arrest it was, whether it is cited or booked. A cited arrest is an arrest where the arrested person has been given a fine or a warning, and a booked arrest is where the arrested person has been taken into custody by the police officer.


<iframe src="/figures/barplot.html"
    sandbox="allow-same-origin allow-scripts"
    width="150%"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>


In the plot above we notice that different times of day seem to have different rates of booked and cited f.x. from 1-4 in the morning it seems that there are more booked arrests than at other times, this might be because the more serious crimes are committed at night, however all that this tells us is that there might be something interesting going on, but to figure out what is going on we need to dig deeper.


As a part of this project we decided that it would be interesting not just to simply analyze the crime rate or the area, but also the resolution of the crime. Some crimes tends to have softer punishment, such as fines or warnings, while others tend to have harsher punishments where the offender is actually prosecuted. In this case we thought it might be a good idea to see whether there is a difference between the number of booked arrests (offender is arrested and taking to a police station) and cited arrests (offender is let of with a fine or warning), depending on the neighborhood. Below can be seen a plot of prostitution in San Fransisco where each area has been colored depending on the ratio between booked arrests and all arrests.


<iframe src="/figures/map.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="500"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>


Here we can see that areas such as Tenderloin, Central, Northern, Mission and Richmond tend to have fewer booked arrests for prostitution compared to the total number of arrest resolutions for prostitution. Areas such as Taraval, Park and Southern tend to have a higher booked rate. However, it is important to know that this rate is calculated in relation to all other resolutions, so this plot does not indicate that there is more prostitution in the aformentioned areas, simply that more often offenders gets taken to the police station. In fact areas where the rate is low could be due to the fact the patrolling police are more busy or more needed on the road and therefore more often decide to let offenders off with fines as for example Tendorloin is a neighborhood notorious for criminal activity.

<iframe src="/figures/prostitution_tenderloin.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>



We notice from the actual prostitution related crime that most of the cited cases are loitering, most probably prostitutes who are then fined by the police instead of being taking into custody. We also notice that most more serious crimes such as pimping and human trafficking are almost always booked. All of this supports our hypothesis that police in this area tend to focus more on the serious crimes and are more leniant towards less serious crimes. All of this might be due to the fact that Tenderloin has a high crime rate in general and police are understaffed in the area. An article from the San Francisco Standard made in 2023 explains how police in the area has resorted to pulling back cops from retirement and discharged officers to do drug busts [2]. Another article from CBS News made in 2023 explains how the current major is requesting more funding to police departments, especially in Tenderloin to try and combat drug issues in the area [3]. All of this might explain why police in Tenderloin generally tend to choose more lenient resolutions for crimes like loitering.

[1]: https://data.sfgov.org/browse?category=Public+Safety
[2]:https://sfstandard.com/2023/02/28/tenderloin-crackdown-brings-back-troubled-cops-dubious-covert-tactics/
[3]:https://www.cbsnews.com/sanfrancisco/news/san-francisco-crime-tenderloin-drugs/