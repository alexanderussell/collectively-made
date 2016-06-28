---
title: "Bike Speed Poetry Generator"
subtitle: "Experimenting with madness"
layout: post
category: projects
tag: Physical Computing
permalink: /projects/bike-speed-poetry-generator
img: bike.png
featured: true
thumb-bg: "background-color: #eed100;"
header-id: header-bike
jewel: bike-exploded-diagram.png
---

<div class="wrapper case-study" markdown="1">

<figure class="img-left">
<img src="/img/projects/OpenBack.JPG" />
<figcaption>A light switch socket retrofitted to house the Arduino.</figcaption>
</figure>

## The Original Project

<span class="drop-cap">I</span> set out to create some kind of system that allowed me to measure the speed of my bike, not with numbers or miles per hour, rather with some kind of senuous indicator. The first iteration used a small LED that was wired up to some sensors and a microprocessor. The original intent was to provide visual feedback to the cyclist, similar to how a car operator can view the spedometer. It began to feel unimportant to be able to view speed this way since you have a lot of other human senses giving you an idea of how fast you are moving while on a bike. 

Subsequent iterations move the blinking light to the ends of the drop-down handlebars in order for drivers to see the cyclist better and possibly be able to gauge the speed a cyclist is moving at. Eventually, I replaced the light entirely with a poetry generator. This new un-functional design direction was inspired by an experiment in innovation; recombining two ideas to create something new, perhaps more artistic than useful. I just couldn't escape the idea of recording speed with poetry.

This was built using an <a target="_blank" href="http://amzn.to/1UxYccn">Arduino Leonardo</a> and a few supplies from the hardware store. The idea is that whenever the magnet gets close to the hall effect sensor, it reads a value which is translated through the arduino to turn on a light. The faster the tire is rotating, the faster the light blinks.

</div>
<div class="wrapper-l">
<img src="/img/projects/wheelview.jpg" />
</div>

<div class="wrapper case-study" markdown="1">

The LED originally was in the center of the handle bars, facing the rider so she could receive visual feedback of how fast she is moving. Upon further consideration, I decided to wire in two LED’s that extend to the ends of each handle bar. Doing this would make the LED light visible to drivers and thus make the cyclist more noticeable. It would also allow drivers to see a change in speed. 

## Flirting With Multiple Ideas

While experimenting with measuring speed, I was also creating a very archaic poetry generator. Using a random pattern & word picking algorithm, users would see lines of poetry displayed at the push of a button. 

<img src="/img/projects/poetryGenerator.png" />

## The Mutation

The decision to merge these two creations came pretty naturally. The random pattern algorithm was replaced with the value indicator the speed generator produces. In other words, the speed of your bike wheel determines the ridiculousness of the poetry.

There is some method to the madness. Words with less syllables were categorized inside of their original categorization (noun, verb, adjective, pronoun, ect.) at the bikes slowest point, it delivers 1 syllable words, at it's fastest the most syllables possible. It may have made sense to do it the other way around. You can say 1 syllable words much faster than you can multiple syllable words. But I liked the idea of approaching increasing complexity and absurdity the faster you go.

</div>