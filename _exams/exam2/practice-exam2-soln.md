---
layout: page
title: Practice Exam 2 Solutions
permalink: /exams/practice-exam2-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1

In Fall 2022, the average GPA of Electrical Engineering (EE) majors in lower-division courses at CSUF was $$2.4$$ and the standard deviation was $$0.4$$.
Assume that GPA's satisfy a normal distribution.
Use Simpson's Rule with $$n=6$$ to approximate the probability that a randomly selected EE student's GPA was at least a B-, (ie. between $$3.0$$ and $$4.0$$).

**Solution:**

We use the probability density function

$$f(x) = \frac{1}{0.5\sqrt{2\pi}}e^{-\frac{(x-2.4)^2}{2(0.4)^2}}.$$

Using Simpson's rule with $$n=6$$

$$\begin{align}
P(3\leq x\leq 4)
  & \int_3^4 f(x)dx\\
  & \frac{1}{3}\Delta x\left(f(x_0)+4f(x_1)+2f(x_2)+4f(x_3)+2f(x_4)+4f(x_5)+f(x_6)\right)\\
  & \frac{1}{3}\frac{1}{6}\left(f(18/6)+4f(19/6)+2f(20/6)+4f(21/6)+2f(22/6)+4f(23/6)+f(24/6)\right)\\
  & \frac{1}{3}\frac{1}{6}(0.323794+0.158904+0.0655547+0.0227339+0.00662744+0.000162412+0.000334576)\\
  & = 0.579573023888
\end{align}$$

## Problem 2

* (a) A $$50$$ kg object is shot from a cannon straight up with an initial velocity of $$10$$ m/s off a bridge that is $$100$$ meters above the ground.  As it moves through the air, it is slowed down by friction caused by air resistence.  Assuming the friction force is proportional to $$-v$$ (with proportionality constant $$k$$), set up a differential equation describing the velocity as a function of time.

* (b) Find a solution of the initial value problem

$$y' = e^{y-t}\sec(y),\ \ y(0) = 0.$$

**Solution:**

* (a) The key to this problem is to use the Newton's equation $$F=ma$$, for $$m$$ the mass and $$a=\frac{dv}{dt}$$ the acceleration.

The total forces present are the force of gravity $$-mg$$ and the force of air drag $$-kv$$.
Inserting this into Newton's equation, we get the differential equation

$$-mg -kv = m\frac{dv}{dt}.$$

Here $$g=9.81$$ is the acceleration due to gravity and $$m=50$$ is the mass, so

$$\frac{dv}{dt}= -9.81-\frac{k}{50}v.$$

* (b) We separate and integrate

$$\int e^{-y}\cos(y)dy = \int e^{-t}dt$$

The left integral is done using integration by parts.  This gives

$$\frac{1}{2}\left(e^{-y}\sin(y)-e^{-y}\cos(y)\right) = -e^{-t} + C.$$

Inserting the special value $$y(0) = 0$$ gives

$$\frac{1}{2}\left(0-1\right) = -1 + C.$$

This gives us $$C=1/2$$ and our final answer is

$$\frac{1}{2}\left(e^{-y}\sin(y)-e^{-y}\cos(y)\right) = -e^{-t} + \frac{1}{2}.$$

## Problem 3

Consider the following set of parametric equations

$$\left\lbrace\begin{array}{c}
x(t) = \csc(t)\\
y(t) = \cot(t)\\
\end{array}\right.\quad\text{for}\quad 0 < t <  \pi$$

* (a) Create a plot of the parametric curve above.

* (b) Find the slope of the tangent line to the curve at the point $$(\sqrt{2},1)$$.

**Solution:**

* (a) Omitted

* (b) 

$$\frac{dy}{dx} = \frac{dy/dt}{dx/dt} = \frac{-\csc^2(t)}{-\csc(t)\cot(t)} = \sec(t).$$

We want this when $$(x,y) = (\sqrt{2},1)$$, ie. when $$t=\pi/4$$.
This gives us a slope of $$\sec(\pi/4) = \sqrt{2}$$.


## Problem 4

Find the area of the region which lies inside both the curve $$r=2\cos(\theta)$$ and the curve $$r=2\sin(\theta)$$.

**Solution:**

By symmetry, it is twice the region between the angles $$\theta=0$$ and $$\theta=\pi/4$$.  Therefore the area is

$$A = 2\int_{0}^{\pi/4}\frac{1}{2}(2\sin(\theta))^2d\theta = 4\int_0^{\pi/4}\sin^2(\theta)d\theta = \frac{\pi}{2}-1.$$

## Problem 5

* (a)  Determine the limit of the sequence, if it exists.  If it is divergent, then write DIVERGENT.

$$a_n = \left(1 + \frac{2}{n}\right)^n.$$


* (b) Find the value of the sum

$$\sum_{n=1}^\infty \frac{12}{n(n+3)}$$


* (c) Express the decimal expression

$$0.123123123123\dots$$

as a fraction of two whole numbers.

**Solution:**

* (a) The well-known limit expression for an exponential!  $$e^2$$

* (b) Telescoping series!

$$\sum_{n=1}^\infty \frac{12}{n(n+3)} = \sum_{n=1}^\infty \frac{4}{n}-\frac{4}{n+3} = 4 + 2 + \frac{4}{3}.$$

* (c) 

$$0.123123123123\dots = \sum_{n=1}^\infty 123\cdot (0.001)^n = \frac{0.123}{1-0.001} = \frac{0.123}{0.999} = \frac{123}{999}.$$



