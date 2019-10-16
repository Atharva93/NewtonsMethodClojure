# The Newton's method in Clojure

In this assignment, you will be programming in Clojure and experiment with the basics of functional programming by implementing the Newton's method for solving roots of polynomials.

Newton's method is a very simple numerical algorithm to solve for the roots of polynomials.  Namely, it is a method that tries to solve the equations of the form:

$$ ax^3 + bx^2 + cx + d = 0 $$

We can rewrite the equation as:

$$ f(x) = 0 $$
where

- $f(x) = ax^3 + bx^2 + cx + d$, and
- the first derivative is $f'(x) = 3ax^2 + 2bx + c$.

Newton's method is an algorithm that attempts to find a solution to
$f(x) = 0$ by an iterative method.

It works as follows:

- Pick an initial guess $x_0$.
- It refines the guess using the following update rule:
  $$ x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)} $$

Given the _right_ condition, we can show that:

$$ \lim_{n\to\infty} f(x_n) = 0 $$

So, for large enough $n$, $x_n$ is a good approximation to the solution.

# Assignment

In this assignment, you are asked to implement and evaluate Newton's method in Python and Clojure.
For this assignment, you are required to use the Jupyter notebook work environment.

See worksheet_python.ipynb for details in the Python implementation.

See worksheet_clojure.ipynb for the Clojure implementation.
