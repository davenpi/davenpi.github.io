---
layout: page
title: The rolling coin/Cyr wheel 
description: Path tracking with shape change
img: assets/img/rolling_coin.jpeg
importance: 2
category: work
---

## The project

The [Cyr Wheel](https://en.wikipedia.org/wiki/Cyr_wheel) is a big wheel that acrobats get inside and do complicated tricks.
Observations of acrobats in cyr wheels made us interested how difficult it is and how we might model the system from a
physical point of view.

To study the question we need to do three things.

### 1. Create a physical model
We need a set of equations describing the cyr and the forces exerted on it. 
That's the physics/dynamical system part. We got the physical model from [well known models](https://rotations.berkeley.edu/the-rolling-disk/) 
of rolling coins. We approximate the cyr wheel + acrobat as a rolling coin. I will present and describe the equations in more detail within the next few days.


### 2. Define what we can control and the performance objectives
Given the equations, what is it that we can control which corresponds to the acrobat moving around inside the wheel? We presume that
the athlete moves their body around so that the wheel becomes easier/harder to rotate in different directions. In other words we presume
that the athele inside the cyr wheel is effecitively changing the system's moment of inertia. Given the control, how can we change the
control over time so that the wheel follows a prescribed track along the ground? 

### 3. Simulate and analyze results
The equations which describe the wheel are too complicated to solve by hand. As a result we need to write software which
simulates the system. Once we have the physics simulated we need to combine that with optimization software to
develop control strategies which solve our task in the best way possible.


## Current status

The problem is formulated and we are working on getting the simulations set up. Expect to have the paper out before the end of May.

