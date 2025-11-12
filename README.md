# Assignment for Research and Development/AI
Parametric Curve Fitting Solution
=================================

Objective:
----------
Finding the values of unknown variables in the given parametric equation of a curve and 
minimize the L1 distance between uniformly sampled points on the curve and data points.

Approach
---------
Step 1: 
-------
Understanding the Problem:
--------------------------

I have to find θ,M,X that best align the predicted parametric curve with the given (x, y) data. I am treating this as a nonlinear optimization problem , so I will minimize the L1 distance between predicted and observed data points.

Step 2: 
-------
Methodology:
-----------

1) I have imported the dataset xy_data.csv.
2) Then i have defined the coordinates of the parametric curve.
3) Then i have Defined the objective function (L1 distance), where i have used the same number of samples as data points for fair comparison &  For each data point, i have found the minimum L1 distance to any curve point.
4) Then i have set up  optimization constraints and bounds.
5) After that i have # Defined multiple initial guesses to explore the parameter space.
6) Next I have Tried each initial guess & ran L-BFGS-B optimization & Kept track of the best result.
7) Then i have extracted the best parameters.
8) After that i have validated the result by numerical and visual methods.

