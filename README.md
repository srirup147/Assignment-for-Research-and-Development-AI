# Assignment for Research and Development/AI
Parametric Curve Fitting Solution
==================================

Problem:
--------
Given parametric equations:
    x=\left(t*\cos(\theta)-e^{M\left|t\right|}\cdot\sin(0.3t)\sin(\theta)\ +X \right )
    y = \left (42 + t*\sin(\theta)+e^{M\left|t\right|}\cdot\sin(0.3t)\cos(\theta)\right)

Where:
  0 \deg<\theta<50 \deg \\
  -0.05<M<0.05 \\
  0<X<100\\

Objective:
----------
Finding the values of unknown variables in the given parametric equation of a curve and 
minimize the L1 distance between uniformly sampled points on the curve and data points.

Approach
---------
---> Step 1: Understanding the Problem:
I have to find θ,M,X that best align the predicted parametric curve with the given (x, y) data. I am treating this as a nonlinear optimization problem , so I will minimize the L1 distance between predicted and observed data points.
Step 2: Methodology:
