---
layout: post
title:  "A data-viz story about the "
date:   2024-04-23 09:47:40 +0100
categories: homework
---

It is no secrete that driving a car, can at times be dangerous, what is unclear is which kind of car brand is more safe. With advertising, a plethera of websites claming to an emperical safety rating of every car, it can be hard to navigate the world of car safety. Therfore we intend to figure out which kind of car is the safest car to drive, we are going to limit our search to New York City, since there is a lot of great open data accesible in NYC.

To keep the story focused we will only be looking at the most frequent car types. This however is justifiable since car types that occour less frequently will be more subject to outlier in the data set, compared to the most frequent car types, where we expect the wisdom of the crowds to be in effect.

A simple analisys would look at the total amout of accidents, that the different car types have been in and then conclude that the car type, which have been in the most accidents is the most dangerous. However, we need to factor in the amount of cars of that specific make that are so that we can find the relative amount of crashes that a car type is in, the following plot shows that concept.     

<iframe src="/figures/Ratio_car_brand.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

From the plot we see that a Honda is more likely to be in an accident then other car brands, this however still leaves a lot of questions, such as, do people that drives a Honda and are in an accident, more in dangere than people who drive a Ford. To answer this we need to look at how people get injured when they are in a car crash. The following heatmap shows what kind of injuries people get, compared to the specific kind of crash.

<iframe src="/figures/ProInj.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

From the heatmap we notice a few things. We notice that the entire body is mainly injured when the car is either demolish or overturned. Further more  we notice that the neck seems to be the most injurde body part in almost every type of accident that occours, with back following as a close second. To further validate this hypothesis we can look at the complaints. 

<iframe src="/figures/Complaint_POI.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

From looking at the heatmap, we can tell that our hunch is consistent between the two plots, since a whiplash is primarily stressfull the the back and neck. However it does not explain the minor bleading. This however can simply be explained by the fact that a car accident is in general traumatic and therfore the odds that a person involved in a car crash will bleed is just fairly large in general.

<iframe width="420" height="315"
src="https://www.youtube.com/embed/MqRDoRvb8yI&t=15">
</iframe>