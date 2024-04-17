# OpenStax Calculus Vol. I

## Chapter 3, Section 1
## Defining the Derivative

Secant lines can be used to estimate rate of change in a function. 
We can get this secant line by taking two nearby points on a function and drawing a line between them.
To accomplish this, we can use the formula
f(x) - f(a) / x - a, replacing x with a+h (h being a constant approaching zero).
The tangent line of a function at any point a, is the secant line passing through point a.

That function is known as the derivative, and the process of finding it is differentiation.

## Chapter 3, Section 2
## The Derivative as a Function

Using the method from the last section, we can find the derivative at a specific point in x.
If we needed to find the derivative at each point in a domain, we can use the derivative as a function.

A function is differentiable on S if you can differentiate any point in set S.
A function is differentiable at a if you can get a derivative at point a.

To find the derivative of a function, simply:
Substitute the function into your derivative formula
Simplify it
And evaluate the limit.

We can use several different notations to represent the derivative of f(x).
Defining y as equal to f(x), the derivative of f(x) is:
f'(x)
dy/dx
y'
or d/dx * (f(x))
And in place of f'(a), we can use
dy/dx|x=a

A point must be continuous to be differentiable, but a continuous point may not be differentiable.
For example, a function like |x| would be undifferentiable at 0 because it's limit changes depending on the approaching direction.
Another situation would be the cube root of x, where the tangent line at 0 is perfectly vertical.
And there are also numerous weird edge cases where a function can't be differentiable.

Since the derivative of a function is a derivative, we can find the derivative of that derivative.
This is known as a higher order derivative.

## Chapter 3, Section 3
## Differentiation Rules

The derivative of a constant function is always 0.
The derivative of x<sup>n</sup> is nx<sup>n-1</sup>.
The derivative of f(x) + g(x) is equal to the derivative of f(x) + the derivative of g(x).
The derivative of kf(x) is equal to k * the derivative of f(x).
The derivative of f(x) * g(x) is equal to the derivative of f(x), times g(x), + the derivative of g(x), times f(x).
The derivative of f(x) / g(x) is equal to the derivative of f(x) * g(x) / (g(x))<sup>2</sup>.

## Chapter 3, Section 4
## Derivatives as Rates of Change

If we have a function defined over an interval of [a, a+h] the amount of change would be measured as f(a+h) - f(a).
The average rate of change for this formula would be f(a+h) - f(a) / h. Instantaneous would be that formula with h approaching 0.
If we have f' and we know h is small enough, we can use the formula f(a+h) ~= f(a) = f'(a)h to estimate f(a+h).

Derivatives as rates of change can be used to analyze acceleration, population growth, and marginal cost.

## Chapter 3, Section 5
## Derivatives of Trigonometric Functions

The derivative of sine is cosine, and the derivative of cosine is -sine #mindblown.
The derivatives of tangent and cotangent are secant<sup>2</sup> and cosecant<sup>2</sup>.
The derivatives of secant and cosecant are secant * tangent and -cosecant * cotangent.

## Chapter 3, Section 6
## The Chain Rule

The chain rule states that the derivative of a composite function is the derivative of the outer function
evaluated at the inner function times the derivative of the inner function.
i.e. d/dx | sin(x<sup>3</sup>) = cos(x<sup>3</sup> * 3x<sup>2</sup>).

## Chapter 3, Section 7
## The Derivative of an Inverse Function

If a function is both invertible and differentiable, its inverse is also differentiable.
If f<sup>-1</sup> is differentiable at a, then it's derivative is equal to 1 / f'(f<sup>-1</sup>(a)).

The derivatives of inverse trigonometric functions are as follows:
The derivative of inverse sine is 1 / sqrt(1 - (x)<sup>2</sup>).
The derivative of inverse cosine is -1 * the derivative of inverse sine.
The derivative of inverse tangent is 1 / 1 + (x)<sup>2</sup>.
The derivative of inverse cotangent is -1 * the derivative of inverse tangent.
The derivative of inverse secant is 1 / |x|sqrt((x)<sup>2</sup> - 1).
The derivative of inverse cosecant is -1 * the derivative of inverse secant.

## Chapter 3, Section 8
## Implicit Differentiation

An implicit function would be a function defined from an equation where y is not clearly expressed by x.
For example, the equation y - x<sup>2</sup> = 1 would implicitly define y = x<sup>2</sup> + 1.

Implicit differentiation is used to find the slopes of tangents to non-functions.
To perform implicit differentiation, follow these steps:
Derive both sides of the equation.
Factor out dy/dx.
Solve for dy/dx by dividing both sides of the equation with an expression.

## Chapter 3, Section 9
## Derivatives of Exponential and Logarithmic Functions
