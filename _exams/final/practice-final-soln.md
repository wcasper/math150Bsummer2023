---
layout: page
title: Practice Final Exam Solutions
permalink: /exams/practice-final-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1

Consider the region of the plane bounded by the curves $$y=0$$, $$y=x^2+1$$, $$x=0$$ and $$x=1$$.

* (a) Set up, but do not evaluate an integral representing the volume of the solid of revolution obtained by rotating the region around the $$x$$-axis.

$$\int_0^1 \pi (x^2+1)^2dx$$

* (b) Set up, but do not evaluate an integral representing the volume of the solid of revolution obtained by rotating the region around the line $$y=2$$.

$$\int_0^1 \pi [(2-0)^2-(2-(x^2+1))^2]dx$$

* (c) Set up, but do not evaluate an integral representing the volume of the solid of revolution obtained by rotating the region around the line $$x=1$$ using the Shell Method.

$$\int_0^1 2\pi (1-x)(x^2+1)dx$$

## Problem 2

A spherical tank with a radius of $$5$$ meters is half filled with water.  How much work is required to pump the water out of a whole at the top of the tank?  [Remember: the density of water is $$1000$$ kg/m$$^3$$ and gravitational acceleration is $$9.8$$ m/s$$^2$$.

$$\int_{-5}^0 1000(9.8)(5-y)\pi (5^2-y^2) dy $$

## Problem 3

Set up, but do not solve, an integral obtaining the arc length of one petal of the four-leaf clover $$r=\cos(2\theta)$$.

$$\int_{\pi/4}^{3\pi/4} \sqrt{\cos^2(2\theta)+4\sin^2(2\theta)}d\theta$$

## Problem 4

Find the surface area of the shape obtained by rotating the curve

$$y=x^3,\ \ 0\leq x\leq 2$$

around the $$x$$-axis.

$$\int_0^22\pi x^3\sqrt{1 + 9x^4}dx = \left.\frac{1}{27}\pi(1+9x^4)^{3/2}\right\rvert_0^2 = \frac{1}{27}\pi(145^{3/2}-1)$$

## Problem 5

Calculate each of the following integrals

* (a) $$\int (\ln(x))^2dx$$

$$x\ln(x)^2-2x\ln(x)+2x+C$$

* (b) $$\int\frac{1}{x^2\sqrt{4x^2+1}}dx$$

$$-x^{-1}\sqrt{1+4x^2}+C$$

* (c) $$\int \frac{x^2-2x-1}{(x-1)^2(x^2+1)}$$

$$-\frac{1}{2}\ln(1+x^2) + \frac{1}{x-1} + \ln(x-1) + \tan^{-1}(x) + C$$


## Problem 6

Determine carefully the limit of each of the following sequences.

* (a) $$\lim_{n\rightarrow\infty} n\sin(2/n)$$

$$2$$

* (b) $$\lim_{n\rightarrow\infty} \frac{2^n}{n!}$$

$$0$$

* (c) How many terms must we add up in the series $$\sum_{n=1}^\infty \frac{1}{n^5}$$ in order to get the value up to $$5$$ decimal places?

$$R_n\leq \int_n^\infty \frac{1}{x^5}dx = \frac{1}{4n^4}.$$

We want $$\frac{1}{4n^4}\leq 10^{-6}$$ 

so we should sum $$n=23$$ terms.

## Problem 7

Determine if each of the following series are absolutely convergent, continuously convergent, or divergent.

* (a) $$\sum_{n=1}^\infty \frac{n+4^n}{n^2+6^n}$$

Use the Limit Comparison Test with the convergent geometric series $$\sum_{n=1}^\infty (4/6)^n$$.
Since

$$\lim{n\rightarrow\infty}\frac{\frac{n+4^n}{n^2+6^n}}{(4/6)^n} = 1,$$

either both series converge or both sries diverge.
Thus both series converge.

* (b) $$\sum_{n=1}^\infty (-1)^n\cos(\pi/n)$$

The limit $$\lim_{n\rightarrow\infty}(-1)^n\cos(\pi/n)$$ does not exist.
The test for divergence implies that the series diverges.

## Problem 8

Determine if each of the following series are absolutely convergent, continuously convergent, or divergent.

* (a) $$\sum_{n=1}^\infty \frac{n+5}{\sqrt[3]{n^7+n^2}}$$

The Limit Comparison Test with the $$p$$-series $$\sum_{n=1}^\infty \frac{1}{n^{4/3}}$$ implies that both series converge absolutely.

* (b) $$\sum_{n=1}^\infty \frac{\ln(n)}{n^3}$$

The Limit Comparison Test with the $$p$$-series $$\sum_{n=1}^\infty \frac{1}{n^{2}}$$ implies that both series converge.

* (c) $$\sum_{n=1}^\infty (-1)^n\frac{10^n}{(n+1)4^{2n+1}}$$

The Ratio Test shows that the series converges.

## Problem 9

Find the radius of convergence and the interval of convergence of the series

$$\sum_{n=1}^\infty (-1)^n\frac{x^n}{n^25^n}.$$

The radius of convergence is $$R=5$$.

The interval of convergence is $$[-5,5]$$

## Problem 10

* (a) Calculate the Taylor polynomial $$T_8(x)$$ of the function $$f(x)=\sin(2x)$$ based at $$x=0$$.

$$T_8(x) = \sum_{n=0}^3 \frac{(-1)^n}{(2n+1)!}2^{2n+1}x^{2n+1}$$

or equivalently

$$T_8(x) = 2x - \frac{2^3}{3!}x^3 + \frac{2^5}{5!}x^5 - \frac{2^7}{7!}x^7 .$$

* (b) Use Taylor's Estimate to bound the error $$\lvert T_8(x)-f(x)\rvert $$ in the interval $$[-0.1,0.1]$$.

The $$9$$'th derivative of $$f(x)$$ is $$2^9\cos(2x)$$.  The maximum value of this on the interval $$[-0.1,0.1]$$ is $$2^9$$.
Therefore Taylor's Estimate says

$$\lvert T_8(x)-f(x)\rvert \leq \frac{2^9x^9}{9!}.$$



