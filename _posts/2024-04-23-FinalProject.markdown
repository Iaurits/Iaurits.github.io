---
layout: post
title:  "Crash Course  "
date:   2024-04-23 09:47:40 +0100
categories: homework
---

It is no secret that driving a car can, at times, be dangerous. What is unclear is which kind of car brand is safer. With advertising and a plethora of websites claiming to offer empirical safety ratings for every car, it can be hard to navigate the world of car safety. Therefore, we intend to figure out which kind of car is the safest to drive. We will limit our search to New York City since there is a lot of great open data accessible in NYC. We will also only consider the top five most frequently bought cars in the USA: Ford, Toyota, Chevrolet, Honda, and Nissan [1]. We choose to restrict ourselves to these brands as car brands that occur less frequently will be more subject to outliers in the dataset compared to the most frequent car types, where we expect the wisdom of the crowds to be in effect. Additionally, we have too much data to take everything into account.

A simple analysis would look at the total number of accidents involving different car types and then conclude that the car type with the most accidents is the most dangerous. However, we need to factor in the number of cars of each specific brand to find the relative frequency of crashes for each car brand. This is achieved by using the number of cars sold in the USA for those five brands. Ideally, we would use data only from NYC; however, we expect that data from the entire USA is somewhat representative for NYC as well. In the following plot, the brands are ranked from the brand with the fewest relative crashes.

<iframe src="/figures/Ratio_car_brand.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

_Figure 1: Ratio of crashes and cars sold for the five most popular car brands_


It can be seen from this plot that Ford has the lowest amount of crashes per car sold. While Toyota has the highest. This could indicate that the Ford brand is safer to drive. 
It might also be interesting to see whether there are any temporal patterns in the amount of crashes for these five brands. This is important in order for us to take into account any temporal trends or patterns which would go unnoticed in the first plot, but also to notice any differences in how data was collected at different points in time.

<iframe src="/figures/bokeh(1).html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

_Figure 2: Here is can be seen how the number of crashes for each car brand has evoled thorugh the past decade_


Notice that all car brands follow the same trend and that data after 2016 rises shapely. This is due to the way data was recorded was changed. We also notice a sharp decline after 2020 which might be due to corona virus and the resulting lockdown.
However, the percentage of crashes might not be sufficient when rating car safety. This is due to the fact that it might be impossible to ever design a car which never crashes since humans drives cars and human behavior is unpredictable. Therefore car manufactures might be more interested in reducing the bodily harm that occurs as a result of crashing, rather then reducing the actual risk of a crash itself. To account for this we have also created a plot which shows the occurrance of complaints per car brand. 



<iframe src="/figures/Car_brand.html"
    sandbox="allow-same-origin allow-scripts"
    width="150%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

_Figure 3: This plot shows a heatmap where each column corropsonds to a car brand, and the color of each square represents the procentage of this injury per car brand._


We notice that the neck and head are the most common places to be injured, no matter which car brand you drive. 

To further validate this hypothesis we can look at the complaints. 
On the left heatmap, we can tell that whiplash and minor bleeding are the most common injuries. The high number in whiplash is also evident in the right heatmap where we can see that head and neck are the most common places to be injured. However it does not explain the minor bleading. This however can simply be explained by the fact that a car accident is in general traumatic and therefore the odds that a person involved in a car crash will bleed is just fairly large in general. The Youtube video below proves the point, as we see in the colission the dummys are thrown arround, glass and metal shards are flying everywhere, so it is no suprise that those two complaints seems to be the bigger ones. We also notice that each car brand have mostly the same distributions of injuries, and we can therefore from this plot not conclude that one brand is better than the other. However we will now look closer at Ford since this was the brand with the lowest ratio from figure 1.

On the left heatmap, we can tell that our hunch is consistent between the two plots, since a whiplash is primarily stressfull for the back and neck. 

<iframe width="420" height="315"
src="https://www.youtube.com/embed/PICLnx1rfuA">
</iframe>

_Video 1: This video illustrated how the human body is moved during and accident_


The crash test video helps to highlight that another important factor in the crash is also the point of impact. Depending on where the car is hit, different injuries or a higher probability of injury might occur. To highlight this we have taken the safest car brand according to the first plot and colored the different points of impact based on the probability of death/injury.

<iframe src="/figures/car.html"
    sandbox="allow-same-origin allow-scripts"
    width="125%"
    height="650"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

_Figure 4: A vizualazation of how frequents different acidents ocour and theire lethality/injury rate_

From this visualization it can be seen that the center front end, center back end, right front bumper and left front bumper all have the highest probability of killing/injuring the car occupants as points of impact. This is also evident from the crash test video as when the ford is hit from the front, the occupants are flung significantly more around then when hit from the side.

While we had hoped to find that one car brand was significantly safer that the others, this is not the case. Only in the introductory plot did we see much difference in car brands. If we sould give a recomendation it will be based on that, and therefore a Ford should be safest. However it is a very small difference from the other brand, and other factors when buying a car might be more important. We have compared our safety results with the web site iSeeCars.com, which is a web site that helps people find good deals on cars and also has a lot of reaserach articles. On their site the have rated some SUV from each of the five brand that we also look at. When averageing the score for each brand, the brands are sorted in the same way as in the first plot we showed. That is Ford has the safest cars then Chevrolet, Honda, Nissan and lastly Toyota. 

[1]: https://www.statista.com/statistics/264362/leading-car-brands-in-the-us-based-on-vehicle-sales/
