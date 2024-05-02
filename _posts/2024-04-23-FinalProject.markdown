---
layout: post
title:  "Crash Course  "
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

<iframe src="/figures/Car_brand.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>


We notice that the neck seems to be the most injurde body part in almost every type of accident that occours, with back following as a close second. To further validate this hypothesis we can look at the complaints. 

From looking at the heatmap, we can tell that our hunch is consistent between the two plots, since a whiplash is primarily stressfull the the back and neck. However it does not explain the minor bleading. This however can simply be explained by the fact that a car accident is in general traumatic and therfore the odds that a person involved in a car crash will bleed is just fairly large in general. The Youtube video below proves the point, as we see in the colission the dummys are thrown arround, glass and metal shards are flying everywhere, so it is no suprise that those two complaints seems to be the bigger ones.

<iframe width="420" height="315"
src="https://www.youtube.com/embed/PICLnx1rfuA">
</iframe>

<iframe src="/figures/car.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

_figure: A vizualazation of how frequents different acidents ocour and theire lethality/injury rate