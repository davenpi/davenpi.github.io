---
layout: page
title: Kiiking
description: modeling an Estonian pasttime
img: assets/img/Kiiking.jpeg
importance: 1
category: work
---


{% include figure.html path="assets/img/Kiiking.jpeg" title="Kiiking" class="img-fluid rounded z-depth-1" %}
Cover photo from [Wikipedia](https://en.wikipedia.org/wiki/Kiiking#/media/File:Kiiking_12.JPG)
## The project

Kiiking is a past time/sport invented in Estonia. People compete to see who can make a full rotation on the longest swing. It's 
kind of wild. [Check out this video](https://www.youtube.com/watch?v=TWbcsEDrmFE) My advisor was interested in the question 
of how to make complete rotation in the least possible time and posed the question to another grad student and I. As I mentioned 
most of my work involves the control of dynamical systems so this kind of thing, as strange as it may seem, is right up my alley.

To study the question we just need to do three things.

### 1. Create a physical model
We need to create a physical model of the combined athlete/swing system. That part is easy and we just modeled it as
a pendulum of variable length. We added in some extra bells and whistles related
to the fact that a person has a limited amount power they can produce.

### 2. Define what we can control and the performance objectives
Given the equations describing the system we need to decide exactly how we will model the athlete doing their thing. We
also need to decide on a performance objective. In our case it's just the time it takes to make a swing up to 180 degrees.

### 3. Simulate and analyze results
Even though the physical model is simple, the equations are still to complex to solve by hand so we need to simulate the 
system. Once we write the software to simulate the dynamics we need to combine that with some optimization software to find
strategies which solve the task optimally. 

## My contributions and current status

I did some video analysis of real Kiiking to give some experimental weight to the project. I also developed control
strategies using techniques from Deep Reinforcement Learning. The Kiiking problem is simple enough to solve without
the need for something as complex as Deep Reinforcement Learning (my colleague developed a solution using more traditional
methods), but we wanted to use it for a two main reasons. First it allowed us to develop a feedback based control.
Second, since we can solve it with traditional means, we got a chance to compare new methods and their performance to old
ones. 

All the work for this project is done and it is written up. It should be out in the coming week or so.