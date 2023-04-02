---
layout: page
title: The glider
description: Modelling shape change during unpowered flight.
img: assets/img/GliderForces.png
importance: 1
category: work
---

{% include figure.html path="assets/img/GliderForces.png" title="Glider" class="img-fluid rounded z-depth-1" %}
Credit to [NASA](https://www.grc.nasa.gov/www/k-12/VirtualAero/BottleRocket/airplane/glider.html) for the cover photo. It helpfully
describes the forces acting on bodies in unpowered flight.

## The project

My interest in aviation led me to want to include some flight research into my PhD. Much of my work is related to the control of 
dynamical systems so coming up with a project wasn't too hard. This is what I came up with. 

Suppose we have a model of a gliding object (i.e. the object can create no thrust). Can we include a way for it's shape to change and 
use that shape change to try and land it at specific locations? That's the basic question. I thought this would be an interesting way 
to explore different kinds of flight methods and it has some natural inspiration since birds change their shape (wing angles etc.) all 
the time depending on what they want to accomplish. 

I do theoretical work so there's no need to build anything yet. To study the question I laid out we just need to do three things.

### 1. Create a physical model
We need a set of equations describing the glider and the forces exerted on it by gravity and the fluid it's moving in. 
That's the physics part (the dynamical system part). I got the physical model from previous work my advisor did on the [evolution of flight](https://softmath.seas.harvard.edu/publication/planar-controlled-gliding-tumbling-and-descent/). 
I will present and describe the equations in more detail within the next few days. Take a look at the referenced paper if you are eager 
to know more.  

### 2. Define what we can control and the performance objectives
Given the equations, what is it that we can control which corresponds to changing the glider's shape? We already mentioned that our
objective is gliding to a specific point, but do we want to do it in the least amount of time? With the least energy expenditure?
Some mixture of the two? This part of the problem is what I refer to as the control part.

### 3. Simulate and analyze results
The equations which describe the glider are too complicated to solve by hand. As a result we need to write software which
simulates the system. Once we have the physics simulated we need to combine that with optimization software to
develop control strategies which solve our task in the best way possible.

## Current status

We have the model and the control problem defined. I've written the software and produced some results. I just need to add in a few
suggestions from my advisor and write up the results. This paper should be out by May.
