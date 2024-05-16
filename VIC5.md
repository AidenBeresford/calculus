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

## Chapter 5, Section 2
## The Definite Integral

The definite integral over an interval [a,b] is defined as
$$\int_{a}^{b} f(x)dx = \lim_{n\to\infty} f(x_{i}^{*}) * \Delta x$$
If this limit exists, the function is integrable over [a,b].

Variables a and b are the limits of integration, a the lower limit and b the upper.
The function f(x) is called the integrand, and dx indicated f(x) as a function with respect to x, 
with x being the variable of integration. The variable of integration is a dummy variable and doesn't
impact computation of the integral, so it can be safely ignored or replaced with another symbol.

If f(x) is continuous on [a,b] then f is integrable on [a,b]. Note that this relationship is not
inversible, as an integrable function g could be noncontinuous over [a,b] for example with a finite number 
of jump discontinuities.

So far we've been doing Riemann sums with regular partitions, but a Riemann could be done with any partitions.
The difference is that with irregular partitions, the limit must be changed from $n\to\infty$ to the width of the biggest subinterval approaching 0.

Instead of doing the Riemann sum, you can also use geometric formulas. 
If you wanted to integrate a linear function, you could use the triangle formula for example.

If you're integrating a partially negative function, you would get the area under the curve for the positive sections. For the negative sections, the
area above the curve. The net signed area is $A_{+}-A_{-}$.

There are a few properties of the definite integral to memorize:
If the a and b are the same, the integral contains no area.
If the a and b are reversed, put a negative sign before the integral sign.
The integral of a sum is the sum of each operands integral.
The integral of a difference is the difference of each operands integral.
$$\int_{a}^{b} f(x)dx = \int_{a}^{c} f(x)dx + \int_{c}^{b}$$

Comparison theorem can be used to tell us that:
If f(x) >= 0 for a <= x <= b, then
$$\int_{a}^{b} f(x)dx \geq 0$$
If f(x) >= g(x) for a <= x <= b, then
$$\int_{a}^{b} f(x)dx \geq \int_{a}^{b} g(x)dx$$
If m and M are constants such that m <= f(x) <= M for a <= x <= b, then
$$m(b-a) \leq \int_{a}^{b} f(x)dx \leq M(b-a)$$

To get the average of a definite integral, use the formula:
$${1 \over b-a} \lim_{n\to\infty} \sum_{i=1}^{n} f(x_{i})\Delta x = {1 \over b-a} \int_{a}^{b} f(x)dx$$

## Chapter 5, Section 3
## The Fundamental Theorem of Calculus

The only way we have to integrate as of now is Riemann sums and geometry, which are annoying to use.
Here are some more powerful techniques.

The Mean Value Theorem for Integrals says that a continuous function on a closed interval is it's average at some point on the interval.
Formulaically, this can be represented as these two formulas
$$f(c) = {1 \over b-a} \int_{a}^{b} f(x)dx$$
$$\int_{a}^{b} f(x)dx = f(c)(b-a)$$

The Fundamental Theorem of Calculus is broken into two parts.
The first part states that if f(x) is continuous over [a,b], and
$$F(x) = \int_{a}^{x} f(t)dt$$
then F'(x) = f(x) over [a,b].
This is confusing at first, because definite integrals are supposed to be numbers, but F(x) returns a number for all x, so it still works.

Part 2 of the theorem states the following, if f is continuous over the interval [a,b] and F(x) is any antiderivative of f(x), then
$$\int_{a}^{b} f(x)dx = F(b)-F(a)$$
Esentially, if we have the antiderivative we can evaluate the definite integral.

## Chapter 5, Section 4
## Integration Formulas and the Net Change Theorem

Definite and indefinite integrals are similar, but they have key differences that are important to consider while integrating.
A definite integral is either a number or a single function (when the limits of integration are variables).
An indefinite integral is a family of functions differing by a constant. 

Net change theorem considers the integral of a rate of change. When a quantity changes, the new value is the initial value plus the integral of the rate of change of that quantity.
The formula for this is either:
$$F(b) = F(a) + \int_{a}^{b} F'(x)dx$$
or
$$\int_{a}^{b} F'(x)dx = F(b) - F(a)$$

Net change theorem can be applied to area, distance, volume, and more.

## Chapter 5, Section 5
## Substitution

With the Fundamental Theorem, we can find integrals without Riemann sums, but to use it we must be able to find an antiderivative. The substitution technique helps us
find antiderivatives when the integrand is a victim of the notorious chain-rule.
A chain ruled integrand is going to follow the form f(g(x)) g'(x) dx.
In substitution, we substitute the x in dx with a u, which allows us to work with the integral easier.
For example, the substitution of an indefinite integral would be:
$$\int f(g(x)) g'(x) dx = \int f(u)du = F(u) + C = F(g(x)) + C$$

To preform substitution, do these steps:
1. Set u equal to g(x), selecting g(x) such that the integrand has g'(x)
2. Substitute u = g(x) and du = g'(x) into the integral
3. Evaluate the integral with respect to u, if impossible, select a different expression for u.
4. Write the result in terms of x.:wq

Sometimes if the derivative of g(x) and the supposed g'(x) in the integral are different, you need to alter the integrand.
Say we have the integral
$$\int z(z^{2}-5)^{1/2}$$
We know that du is supposed to be 2zdz, but the integrand only contains 1zdz.
To solve this, operate on the integral with 2zdz as du, and then divide it by 2 afterwards.

We can use u-Substitution to manipulate slightly more complicated integrals. Take
$$\int x / \sqrt{x-1} dx$$
In this situation, u is x-1, but the x in the numerator is just x. In this situation, you can set the x to u+1.
