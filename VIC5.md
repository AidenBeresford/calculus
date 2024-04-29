# OpenStax Calculus Vol. I

## Chapter 5, Section 1
## Approximating Areas

Sigma notation is a notation involving the Greek letter Σ, which represents summation. We can use Σ to express
a long sum of values in a compacted form. If we wanted to write the sum expression of integers 1 through 20, we
would have to write a very long expression, or we could write 
$$\sum_{i=1}^{20} i$$

To approximate the area under the curve of a graph, we divide the region into small shapes with known area formulas.
Those areas are then summed up to obtain an estimate of the total area. Taking two positions on the x-axis a and b,
we can divide that interval into n subintervals of width (b-a)/n, imagine rectangles.
This division of intervals is called a partition (my computer science background coming in handy), 
and if they have the same width, a regular partition. 

To approximate the entire interval, the formulas are 
$$\sum_{i=1}^n f(x_{i-1}) * \Delta x$$
for left-endpoint approximation, and
$$\sum_{i=1}^n f(x_i) * \Delta x$$
for right-endpoint approximation.

As the width of each subinterval gets smaller, or as the number of subintervals increases,
the approximation gets more accurate. Essentially, the area of the curve equals the formula as
the number of subsections approaches infinity.

Instead of using an endpoint we could use something called a Riemann Sum, which uses the formula
$$\sum_{i=1}^n f(x_{i}^{*}) * \Delta x$$
to represent the height of the rectangle.

We can choose to under or overestimate the area by making a lower or upper sum. To do this, we have our $x_{i}^{*}$ equal
whichever x on our subinterval has the lowest or highest y value, giving us a lower or upper sum. 
