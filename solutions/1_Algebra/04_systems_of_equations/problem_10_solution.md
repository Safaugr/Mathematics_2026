# Exercise 10. A Polynomial Through Three Points

## Question

Find a polynomial

$$
p(x)=ax^2+bx+c
$$

whose graph passes through (0,1), (1,3), and (2,9).

Reduce the problem to a system of equations
and check the result by substituting all three points.

## Solution

### 1. Translate the points into equations

Passing through (0,1) means

$$
p(0)=1,
\qquad
c=1.
$$

Passing through (1,3) means

$$
p(1)=3,
\qquad
a+b+c=3.
$$

Passing through (2,9) means

$$
p(2)=9,
\qquad
4a+2b+c=9.
$$

Thus, the coefficients satisfy the linear system

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9. \\
\end{cases}
$$

Although p is quadratic in x, the system is linear
in the unknown coefficients a, b, and c.

### 2. Solve the system

Substitute c=1 into the remaining equations:

$$
\begin{cases}
a+b=2, \\
4a+2b=8. \\
\end{cases}
$$

Subtract twice the first equation from the second:

$$
(4a+2b)-2(a+b)=8-4,
$$

$$
2a=4,
\qquad
a=2.
$$

Then

$$
b=2-a=0.
$$

Therefore,

$$
a=2,\qquad b=0,\qquad c=1.
$$

The required polynomial is

$$
p(x)=2x^2+1.
$$

The equations determine each coefficient uniquely.

### 3. Verification at all three points

For x=0,

$$
p(0)=2\cdot0^2+1=1.
$$

For x=1,

$$
p(1)=2\cdot1^2+1=3.
$$

For x=2,

$$
p(2)=2\cdot2^2+1=9.
$$

Thus, the graph passes through all three given points.