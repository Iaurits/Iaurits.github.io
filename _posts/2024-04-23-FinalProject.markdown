---
layout: post
title:  "Crash Course  "
date:   2024-04-23 09:47:40 +0100
categories: homework
---

It is no secrete that driving a car, can at times be dangerous, what is unclear is which kind of car brand is more safe. With advertising, a plethera of websites claming to an emperical safety rating of every car, it can be hard to navigate the world of car safety. Therfore we intend to figure out which kind of car is the safest car to drive, we are going to limit our search to New York City, since there is a lot of great open data accesible in NYC. We will also only consider the top five most frequently bought cars in the USA. These five are Ford, Toyota, Chevrolet, Honda and Nissan [https://www.statista.com/statistics/264362/leading-car-brands-in-the-us-based-on-vehicle-sales/]. We choose to restrict our selves to these brands as car brands that occour less frequently will be more subject to outlier in the data set, compared to the most frequent car types, where we expect the wisdom of the crowds to be in effect. We also have too much data to take everything into account.

A simple analisys would look at the total amout of accidents, that the different car types have been in and then conclude that the car type, which have been in the most accidents is the most dangerous. However, we need to factor in the amount of cars of that specific make that are so that we can find the relative amount of crashes that a car type is in, the following plot shows that concept.     


<iframe src="/figures/Ratio_car_brand.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

It might also be interesting to see whether there are any temporal patterns in the amount of crashes for these five brands. This is important in order for us to take into account any temporal trends are patterns which would go unnoticed in the first plot, but also to notice any differences in how data was collected at different points in time.

<iframe src="/figures/bokeh(1).html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

However, the percentage of crashes might not be sufficient when rating car safety. This is due to the fact that it might be impossible to ever design a car which never crashes since humans drives cars and human behavior is unpredictable. Therefore car manufactures might be more interested in reducing the bodily harm that occurs as a result of crashing, rather then reducing the actual risk of a crash. To account for this we have also created a plot which shows the occurrance of complaints per car brand. 



<iframe src="/figures/Car_brand.html"
    sandbox="allow-same-origin allow-scripts"
    width="150%"
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

The crash test video helps to highlight not another important factor in the crash is also the point of impact. Depending on where the car is hit, different injuries or a higher probability of injury might occur. To highlight this we have taken the safest car brand according to out first plot and colored the different points of impact based on the probability of death/injury.

<iframe src="/figures/car.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

_figure: A vizualazation of how frequents different acidents ocour and theire lethality/injury rate

From this visualization it can be seen that the center front end, center back end, right front bumper and left front bumper all have the highest probability of killing/injuring the car occupants as points of impact. This is also evident from the crash test video as when the ford is hit from the front, the occupants are flung significantly more around then when hit from the side.

While we had hoped to find that one car brand was significantly safter that the others, this is not the case. Only in the introductory plot did we see much difference in car brands. If we sould give a recomendation it will be based on that, and therefore a Ford should be safest. However it is a very small difference from the other brand, and other factors when buying a car might be more important. We have compared our safety results with the web site iSeeCars.com, which is a web site that helps people find good deals on cars and also has a lot of reaserach articles. On their site the have rated some SUV from each of the five brand that we also look at. When averageing the score for each brand, the brands are sorted in the same way as in the first plot we showed. That is Ford has the safest cars then Chevrolet, Honda, Nissan and lastly Toyota. 
