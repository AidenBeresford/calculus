# OpenStax Calculus Vol. I

## Chapter 2, Section 1
## A Preview of Calculus

Rate of change is the measure of the change in y based on the change in x of a function.
In a function f(x) = 1/2x, for every 1 x, y will change by 1/2.
That applies to linear functions, but what about nonlinear functions?

Nonlinear functions don't have a rate of change that can be measured by a constant.
Instead, we can determine the rate of change of a function between two points by taking two points on the function,
drawing a line between them, and finding the slope of that line (known as a secant line).
These secant lines approach the tanget line, which measures the rate of change at the point.
This value also represents the functions derivative, f'(x).

As our second point moves closer to our first point, our slope gradually becomes the tangent slope.
Letting our point approach the other is known as taking a limit.

The other section of Calculus involves finding area under a curve.
The first step is to approximate the area by getting the area of several
small rectangles that roughly follow the slope of our curve.
As the rectangle widths approach zero, the measurement becomes more and more accurate.

Limits are the basis of Calculus.

## Chapter 2, Section 2
## The Limit of a Function

Let's say we have a function that's undefined when x = 2. We would define the limit as
f(x) = ? when x approaches 2, with ? being the closest y to x = 2.
Essentially, a limit is the value that is approached as x gets a close as possible to to an undefinition.
Limits can be estimated by looking a graphs or tables for a function.

For a limit to exist, the function must approach a singular real number value.

Limits can also be one-sided, meaning the limit approaches different values from different sides.
For example, you coud have a limit that approaches -1 from the negative side, and 1 from the positive,
even if both limits are approaching 0.

Infinite limits are limits that approach infinity. Think division over x.

## Chapter 2, Section 3
## The Limit Laws

If the limit of f(x) = a and so on, then the limit of f(x) divided by g(x) is equal to
the limit of f(x) divided by the limit of g(x). 
This holds true for all primitive operations (addition, subtraction, multiplication, etc.)

When calculating a limit with the indeterminate form 0/0, we can do one of three things.
If f(x) and g(x) are polynomials, we can factor the functions and cancel common factors.
If the numerator or denominator contains a difference involving a square roots,
we can multiply the numerator and denominator by the conjugate.
If f(x)/g(x) is complex, we can simplify it.

Squeeze theorem allows you calculate the limits of trigonometric functions.
This theorem squeezes a difficult function between two easier functions,
one function is >= the difficult function, and the other one is <= it, being == at x=a.

## Chapter 2, Section 4
## Continuity

Many graphs can be traced without lifting pencil from paper, this is a property known as
continuity. A function can be discontinuous if at some point it has a break.

Breaks can occur for a number of reasons.
A function can break for point a because f(a) is undefined.
A function can break if f(a) has a nonexistent limit.
A function can break because the limit of f(a) does not equal f(a).

This means that a function is continuous if f(a) is defined, it has an existing limit,
and that limit is equal to f(a).

There are three kinds of discontinuities.
A removable discontinuity occurs when the limit exists.
A jump discontinuity occurs when the limit does not exist.
An infinite discontinuity occurs when either limit approaches either +inf or -inf.

Continuity can also be checked for over an interval of a function instead of a function.
If every point in the function is continuous, then the interval is continuous.

Functions continuous over the interval [a, b] exhibhit Intermediate Value Theorem.
This theorem states that any real number between f(a) and f(b) has a value c between a and b
that satisfies f(c) = z.

## Chapter 2, Section 5
## The Precise Definition of a Limit

Before starting, we need to declare a few things.
|f(x) - L| < epsilon means "The distance between f(X) and L is less than epsilon."
0 < |x-a| < delta means "The distance between x and a is less than delta."
|f(x) - L| < epsilon is equivalent to L - epsilon < f(x) < L + epsilon.
0 < |x-a| < delta is equivalent to a - delta < x < a + delta and a != x.

The epsilon-delta definition of a limit is as follows:
For all x != a over an interval containing a, letting L be a real number,
the limit of f(x) approaching a equals L if, for every epsilon > 0, there exists
a delta > 0, such that if 0 < |x-a| < delta, then |f(x) - L| < epsilon.

Broken down, this means that:
For every positive distance epsilon to L, there is a positive distance delta from a, meaning that
if x is closer than delta to a, and x != a, then f(x) is closer to epsilon than it is to L.

If we wanted to get the epsilon-delta definition of a one-sided limit, we would do the same thing,
chaning the |x-a| for a +- (x-a) depending on the side of the limit.
