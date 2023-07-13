---
layout: page
title: Practice Exam 1 Solutions
permalink: /exams/practice-exam1-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1

* (a) Draw a picture of the region bounded by the curve $$y=x^4-4x^2$$ and $$y=x^2-4$$

<p align="center"><img src="exam1/problem1graph.png"/></p>

* (b) Set up an integral whose value is the area of the region in part (a)

$$\int_{-2}^{-1} (x^2-4)-(x^4-4x^2)dx + \int_{-1}^1 (x^4-4x^2)-(x^2-4)dx + \int_1^2(x^2-4)-(x^4-4x^2)dx$$

* (c) Evaluate the definite integral from (b)

$$8$$

## Problem 2

Consider a tank of the shape featured in the image below.
The density of water is $$62.5\ \text{lb}/\text{ft}^3$$.

<p align="center"><img src="exam1/tank.png"/></p>

* (a) Set up the work required to drain the tank through the pipe at the top.

The bottom radius is $$3$$ and the top radius is $$6$$.
Since the radius increases linearly with the height, we get that the radius is 

$$r(y) = 3 + \frac{3}{8}y.$$

The work required is therefore

$$W = 62.5\int_0^8 \pi (8-y)\left(3 + \frac{3}{8}y\right)^2 dy$$


* (b) Evaluate the total work required.  Make sure to specify your units.

$$62.5\cdot 528$$


## Problem 3

Evaluate each of the following integrals.

* (a) $$\int_0^1 (x^2+1)e^{-x}$$

Using integration by parts twice, we get $$3-\frac{6}{e}$$

* (b) $$\int \frac{1}{\sqrt{x^2+2x+5}}dx$$

Using the trig substitution $$x+1=2\tan(\theta)$$, we get

$$\int \sec(\theta)d\theta = \ln|\sec(\theta) + \tan(\theta)| + C$$

Now by drawing a triangle, we get

$$\ln\left\lbrace \frac{\sqrt{(x+1)^2+2^2}}{2} + \frac{x+1}{2}\right\rbrace + C$$


## Problem 4

Use the specified method to find the volume of the solid of revolution.

* (a) $$y=x(x-1)^2$$ and $$y=0$$ rotated around the $$y$$-axis using the Shell Method

$$V = \int 2\pi rh dx = \int_0^1 2\pi x^2(x-1)^2dx = \frac{\pi}{15}.$$

* (b) $$y=e^{-x}$$, $$y=1$$, and $$x=2$$ rotated around $$y=2$$ using the Disk/Washer Method

$$V = \int \pi (r_{out}^2-r_{in}^2) dx = \pi \int_0^2 (2-e^{-x})^2-1 dx= \frac{5}{2} - \frac{1}{2}e^{-4} + 4e^{-2}.$$

## Problem 5

Evaluate each of the following integrals.

* (a) $$\int \sec^5(x)\tan^7(x)dx$$

$$\int \sec^4(x)(\sec^2(x)-1)^3 \sec(x)\tan(x)dx = \int u^4(u^2-1)^3du = \int u^{10}-3u^8+3u^6-u^4 du$$

This gives

$$\frac{1}{11}\sec^{11}(x)-\frac{3}{9}\sec^9(x) + \frac{3}{7}\sec^7(x) - \frac{1}{5}\sec^5(x) + C.$$

* (b) $$\int \frac{3x+2}{x(x^2+1)}dx$$

Using partial fractions, we get

$$\ln\left(\frac{x^2}{x^2+1}\right) + 3\tan^{-1}(x) + C.$$

