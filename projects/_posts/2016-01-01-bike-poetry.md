---
title: "Bike Speed Poetry Generator"
subtitle: ""
layout: post
category: [projects-featured, projects]
featured: true
img: test.png
permalink: /projects/bike-speed-poetry-generator

---
<!-- 
{final product video} -->

This was built using an <a target="_blank" href="http://amzn.to/1UxYccn">Arduino Leonardo</a> and a few supplies from the hardware store. The idea is that whenever the magnet gets close to the hall effect sensor, it reads a value which is translated through the arduino to turn on a light. The faster the tire is rotating the faster the light blinks.

The LED originally was in the center of the handle bars, facing the rider so he can receive visual feedback of how fast he is moving. Upon further consideration, I’ve decided to wire in two LED’s that extend to the ends of each handle bar. Doing this would make the LED light visible to drivers and thus make the cyclist more noticeable. It would also allow drivers to see a change in speed.



While experimenting with measuring speed, I also created a very archaic poetry generator. Using a random pattern & word picking algorithm, users would see lines of poetry displayed at the push of a button. 

The decision to merge these two creations came pretty naturally. Innovation happens in three ways: transfer, combination, recombination. 

The random pattern algorithm was replaced with the value indicator the speed generator produces. In other words, the speed of your bike wheel determines the ridiculousness of the poetry.

There is some method to the madness. Words with less syllables were categorized inside of their original categorization (noun, verb, adjective, prnoun, ect.) at the bikes slowest point, it delivers 1 syllable words, at it's fastest the most syllables possible. It may have made sense to do it the other way around. You can say 1 syllable words much faster than you can multiple syllable words. But I liked the idea of approaching increasing complexity and absurdity the faster you go.