# Exercise 4. Infinitely Many Solutions

## Question

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0. \\
\end{cases}
$$

Give the solution in parametric form, identify a free variable,
and check the solution for one chosen parameter value.

## Solution

Using the variable order x, y, z, the augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}.
$$

Apply the row operations

$$
R_2\leftarrow R_2-2R_1,
\qquad
R_3\leftarrow R_3-R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}.
$$

The third row gives y=1. Substituting into the first row gives

$$
x+1+z=2,
\qquad
x=1-z.
$$

The zero row adds no restriction. Therefore, z is a free variable.
Set z=t, where t is any real number. All solutions are

$$
(x,y,z)=(1-t,1,t),
\qquad t\in\mathbb{R}.
$$

There are infinitely many solutions because t can be any real number.

### Verification

Choose t=2, giving the point (-1,1,2).
Substituting into all three original equations gives

$$
-1+1+2=2,
$$

$$
2(-1)+2(1)+2(2)=4,
$$

$$
-1-1+2=0.
$$

All three equations are satisfied, confirming the example.