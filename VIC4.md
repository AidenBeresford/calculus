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

