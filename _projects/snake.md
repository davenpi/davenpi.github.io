---
layout: page
title: The snake project
description: Video analysis and mathematical modeling of snakes.
img: assets/img/70cm_time_lapse.png
importance: 1
category: work
---


{% include figure.html path="assets/img/70cm_time_lapse.png" title="Snake" class="img-fluid rounded z-depth-1" %}

## The project

We have a collaborator, [Dr. Bruce Jayne](https://www.artsci.uc.edu/departments/biology/fac-staff/jayne.html),
who is very interested in snake locomotion. Bruce took some videos of snakes bridging vertical gaps like the one
pictured above and we advisor wondered if we could study the stability of the snakes from a mathematical/physics point of view. To
accomplish the task we wanted to first develop a quantitative understanding of the data, then develop a physical model of the snake, 
and then use the physical model to understand the stability properties of the snakes as they do their climbing tasks. 

### Quantitative understanding of the data

The data for this project is several dozen videos of snakes bridging gaps like the one in the picture above. We wanted
to extract the curvature along the snake as it progresses across the gap. In order
to do this I had to convert the videos into a sequence of images and then develop some image analysis software. This software
detects where the snake is in the image, finds it's front, and then calculates the curvature along the entire snake. I had 
never done something like that before and it was a fun challenge to figure that out. 

### Physical model

We decided to model the snake as an elastic filament and include the effect of it's muscles by adding in some extra
parameters to the typical equations of elasticity theory. In particular, we added in an active bending moment to 
supplement the tradition bending moment that filaments/rods create due to their stiffness. I will describe this part of the work
in more detail in the coming days.

### Understanding stability using the model

We use the model to formulate the following control theory question. What is the minimal amount of work the snake
must do to reach a given height?

## Current Progress

I finished the data analysis and am working through the control theory portion of the project. The heavy lift is over and the
aim is to have this paper out by May.