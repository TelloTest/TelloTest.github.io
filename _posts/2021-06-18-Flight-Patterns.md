---
title: 'Sine on the Wavy Line'
date: 2021-06-23
permalink: /posts/2021/06/FlightPatterns/
header:
  teaser: "/../../images/archimedes.png"
tags:
  - unity
  - 'Neon Cloud'
  - devlog
  - show
page.comments: true
---

## The Thin Line Between Fun and Hate
Predictability is the thin line between enjoying a game and loathing it. It is delicately drawn in the sand between stimulating the ego and belittling intelligence. 

On one side of the line, gaining an intuition for a well veiled pattern gives us a feeling of reward, accomplishment or even superiority over those who remain out of the loop. On the other hand, predictability can seem pandering, lazy or perhaps commit the biggest crime in gaming...

...**being boring**

![High Treason: Boring Gameplay](/../../images/boring.gif)

---

## The shortest distance between two points

Back when scientific discoveries could be made while sitting in a hot bath or by simply looking at something for an extended period of time, Archimedes made the claim: 
>"The shortest distance between two points is a straight line."
>
>![ArchimedeezNutz](/../../images/archimedes.png)
>
>**Side Note:**
>I'm not convinced he actually said any of this.

---

Linearity is predictability in its purest mathematical form. There is absolutely nothing more predictable than a straight line and humans have a keen sense for predicting patterns, especially linear trajectories. The interpolation of a moving object is actually a built-in default function of the human brain. This ability goes far beyond simple straight lines too. This means that in order to provide a stimulating challenge to players, games too must evolve beyond straight lines.

![CominRightForUs!](/../../images/cominrightforus.gif)

>
>See [this](https://news.mit.edu/2018/study-reveals-how-brain-tracks-objects-motion-0306) article from MIT if you're interested in this topic.

---

Take for example, this prototype version of some enemies in flight in my game Neon Cloud:

![Absolute unpredictable mayhem!](/../../images/linearmayhem.gif)

Well that's just a hoot'n a half... To be honest I'm bored of this game just from watching this gif.

---

## [Straight Lines, Sealed, Delivered, I'm Bored](https://youtu.be/inXC_lab-34)
Ideally, we want our games to grow exponentially in fun and logarithmically in boredom. Static one-note linear flight patterns as obstacles would result in the reverse of this ideal outcome. A fair but evolving challenge is what I am aiming for in this game. There needs to be patterns a player can begin to tune into over time, but at the same time not be so repetitive as to be painfully obvious.

To solve this, I created an object type in Unity I've called a FlightPattern. A flight pattern is a tuneable asset that can be dropped into any moving object in the game at any time to alter said objects movement behavior. Not only will this help the game escape the exponential boredom problem, it will also allow some progressive challenges that can't as easily be predicted.

I can then use these patterns to assemble scenarios of challenges. Placing a fine tuned set of patterns on a set of enemies can allow me to create some very dynamic challenges that a player can learn over time, but on the surface seem random to a newcomer. I think this will allow my game to grow in fun exponentially as previously mentioned. At the very least I want to stave off the growth of boredom.


## [Sine, Sine Everywhere a Sine](https://www.youtube.com/watch?v=c9lh7lqZojc)

With the new pattern system I've created, linear movement is still an option. However, the game is open for the addition of any new flight logic a designer can come up with. I've implemented patterns that work on sin, cos, square and sawtooth patterns so far. With a few more fundamental functions, I will be able to allow a designer to create truly endless challenges to offer the player.

The following example is a series sine-based flight patterns tuned to varying degrees. Combining these, or other flight pattern objects, you can see how a challenge can be tuned and evolved over the course of the game.

![Sine1](/../../images/SinePattern001.gif)

![Sine2](/../../images/SinePattern002.gif)

![Sine3](/../../images/SinePattern003.gif)

>**Note:**  The last example is a pattern being tuned while the game is running.

---

## Cos For Concern
An endless runner can only be endless if people want to keep playing. If a game like this is too one-note, you can expect players to give it only one chance. I have come up with some more innovative challenges to the traditional endless runner archetype that I will display in future blog posts.

I will also be posting a more technical write-up of the process that went into the creation of flight patterns in a future blog post. Please keep an eye out for that.

:: Tello-

---

>Thank you for taking the time to read this far. I also humbly ask for you to check out some of my other media outlets. I post frequently to [twitter](https://twitter.com/tellovis) as well as my [youtube](https://www.youtube.com/channel/UC-FFrKPac98eL4zfAU1CW9g) channel where you will find devlogs, streams (attempts) and snippets of varying states of my game throughout its development. Likes and subscribes mean a lot to me and may help me more than you realize. Every subscriber helps me get closer to my personal end of summer goals as well as help me get past some subscriber count walls put in place by youtube. Thank you in advance! :)

---

>Lastly, I kindly ask you email me with any feedback of my work, site, inconsistencies or spelling atrocities

<!-- travis override -->
{% if page.comments == true %}
{% include comments.html %}
{% endif %}
<!-- end override -->