# OpenStax Calculus Vol. I

## Chapter 4, Section 1
## Related Rates

Related rates are when to related quantities change with respect to a common variable.
For example, take a balloon with volume V and radius r. The balloon is filling with air over time.
As the volume fills, both V and r are increasing over time. dV/dt and dr/dt are related.

To solve a related rates problem, do the following:
Assign symbols to all variables.
State the givens and the rate to be determined.
Find a relating equation.
Differentiate both sides using chain rule.
Substitute into the equation, then solve for rate of change.

## Chapter 4, Section 2
## Linear Approximations and Differentials

Differentiation also allows us the ability to approximate parts of functions with linear functions.
With a function f differentiable at a, the tangent line is y = f(a) + f'(a)(x-a).
That linear function can give us a good approximation of values near a.

Differentials allow us to estimate change in output over a small change in input.
The differential dy is the dependent variable, and dx is the independent.
A function to define this relationship is dy = f'(x)dx. where f(x) is differentiable.
Simplifying that gives us the formula dy/dx = f'(x), which denotes a derivative.

Consider dx as delta x, the change in x. This means the change in y is equal to f(a+dx) - f(a).
Instead of calculating an exact change, you can use a linear approximation.
This means that if dx is small enough, you can use an approximation to calculate dy.

Let's say we have a function f(a). The exact value is a, but we have the measured value a+dx.
The error here is with dx, and since it's an input, the error manifests in the output.
This is called a propagated error.

If we don't know a, we can approximate the propagated error delta y as dy.
We can approximate dy to f'(a + dx)dx.

In those cases, dx and dy are absolute errors. The relative error is dn/n where n is x or y.

## Chapter 4, Section 3
## Maxima and Minima

Two properties of functions are the absolute maximums and minimums. The absolute extremum.
These are the highest and lowest outputs a function can give. 
If a function approaches + or - infinity, it has no maximum or minimum respectively.

Let's say we have a graph with two peaks, one is higher than the other. The higher peak is the
absolute maximum, the other peak is a local maximum, although both are local maximums. Any dips
would be considered local minimums. It is important to note that if an absolute extremum occurs
at an endpoint, it is NOT a local extremum.

If we don't have a graph of a function, we can find the extrema of a function with Fermat's theorem.
If function f has a local extremum at a point, the derivative of f at that point is either 0 or undefined.
That point is known a critical point of f. Fermat's theorem states that any differentiable local extremum
on a function has a derivative equal to 0. Any absolute extremum that isn't a local extremum must be an endpoint.

## Chapter 4, Section 4
## The Mean Value Theorem

Rolle's theorem states that if the two endpoints of a continuous, differentiable function are equivalent, 
there's at least one point where the derivative equals 0.
Rolle's theorem is a case of Mean Value Theorem which states that if two endpoints are continuous and differentiable, 
the slope of those two points is the derivative at c.

We know that in an interval, if the derivative at all points is 0, that interval is constant.
Constant Difference Theorem states that is two functions have the same derivative across all points, they
are parallel functions. An additional corollary is that if the derivative for all points of a function interval
is more than 0, that interval is increasing, and if it's less than 0, the interval is decreasing.

## Chapter 4, Section 5
## Derivatives and the Shape of a Graph

A continuous function has a local maximum at point c if that function switches from increasing to decreasing at c.
Similarly, a continuous function has a local minimum at c if it switches from decreasing to increasing at c.
Note that not all critical points are local extrema, but all local extrema are at critical points.

Concavity is the property that determines whether the curve of a function curves upwards or downwards.
Over a function f, if f' is decreasing, the function is concave down. If f' is increasing
the function is concave up. Functions can switch concavity as point x where f''(x) is 0 or undefined.
Points where a function changes concavity are called inflection points.

Using the second derivative test, we can find out if a critical point is a local minimum or maximum.
Assuming c is a critical point, if f''(c) > 0, f has a local minimum at c.
If f''(c) < 0, f has a local maximum at c. Otherwise, the test is inconclusive.

## Chapter 4, Section 6
## Limits at Infinity and Asymptotes

If f(x) becomes close to L as x increases to infinity, f has a limit at infinity equal to L. 
This also means that y = L is a horizontal asymptote of f.
The behavior as x approaches +- infinity is known as end behavior.

End behavior gets complicated when involving rational functions. To evaluate the limits of
a rational function, divide the numerator and denominator by the highest term in the equation.

Functions like sin and cos don't approach any specific value as x approaches infinity, therefore
they don't approach a finite limit.

## Chapter 4, Section 7
## Applied Optimization Problems

When optimizing something, we have some quantity we want to maximize or minimize while meeting some
condition.

To solve optimization problems, do the following:
Introduce all variables
Determine the target quantity
Write a formula
Write any related equations
Identify the domain
Locate the maximum or minimum value

## Chapter 4, Section 8
## L’Hôpital’s Rule

Let's say you want to evaluate limits involving the quotient of two functions.
Take the limit of f(x)/g(x). Say the limit of f(x) is L<sub>1</sub> and g(x) L<sub>2</sub>.
The limit of f(x)/g(x) would equal L<sub>1</sub> / L<sub>2</sub>.
If both lim f(x) and lim g(x) equal zero, it's considered an indeterminate form.

L’Hôpital’s Rule gives us a way to evaluate these weird limits. 
Consider two differentiable functions where the limit at x-\>a of f = 0 = the limit at x-\>a of g, 
and g'(a) != 0, we can write f(x) ~= f(a) + f'(a)(x-a), and g(x) ~= g(a) + g'(a)(x-a), meaning
f(x)/g(x) ~= f(a) + f'(a)(x-a) / g(a) + g'(a)(x-a).

L’Hôpital’s Rule can also be used to evaluate limits of the form +-infinity / +-infinity.
In this case, the limit of f(x)/g(x) is equal to the limit of f'(x)/g(x) as x approaches a.
It is important to note that L’Hôpital’s Rule ONLY APPLIES to limits of indeterminate form.

There are some other indeterminate forms like 0 * infinity. To use L’Hôpital’s Rule, simply rewrite
these functions as quotients.

Taking two functions, x<sup>2</sup> and x<sup>3</sup>, both functions approach infinities, but x<sup>3</sup> 
does so much faster. This is demonstrated with:
The limit of x<sup>3</sup> / x<sup>2</sup> as x approaches infinity equals infinity, while x<sup>2</sup> / x<sup>3</sup> equals 0.
Therefore, if the limit of one function over another approaching infinity is infinity, the top function is growing more rapidly, and vice versa.

If we have a function like x<sup>2</sup> / 3x<sup>2</sup> + 4x + 1, and we get the limit of that approaching infinity, each value is
roughly 3 times more, so the limit evaluates to 1/3.
These two functions are considered to be growing at the same rate.

## Chapter 4, Section 9
## Newton's Method

To find the roots of any function is difficult, if not impossible. However, using Newton's Method, we can approximate
the roots of functions. Establishing f as a function with root a, the tangent line as x approaches a will always
intersect the x-axis closer and closer to the root. This means that you can do an approximation f(x<sub>0</sub>), and then
take the x-intercept of that tangent line (x<sub>1</sub>) and do f(x<sub>1</sub>) repeating the process ad infinitum.

Newton's method is not foolproof however, it can fail in certain circumstances. For example, Newton's method can fail when:
The tangent line of f(x<sub>n</sub>) does not intersect the x-axis.
If the approximations are approaching a different root than the one we're looking for.
If the approximations fail to approach a root.

## Chapter 4, Section 10
## Antiderivatives

We know how to find a derivative of a function, but how do we find the function of a derivative? 
A reason we would want that for example, could be constructing velocity from acceleration.
This function constructed from the derivative is called an antiderivative.

Let's say we have function 2x. We know the antiderivative of 2x is x<sup>2</sup> because the derivative of it is 2x.
2x + C where C is any constant is also an antiderivative of 2x, since the derivative of a constant is 0.

The formal notation for representing antiderivatives is
∫f(x)dx = F(x) + C
∫f(x)dx is called the indefinite integral of f.
Finding the antiderivative is called integrating.

The collection of all functions F(x) + C are the antiderivative family of f.

Evaluating indefinite integrals usually applies the same properties of derivatives, for example,
∫x<sup>n</sup>dx = x<sup>n+1</sup> / n+1 + C which uses the power rule of derivatives.

