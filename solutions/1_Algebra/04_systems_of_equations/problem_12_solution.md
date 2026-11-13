# Exercise 12. Homogeneous System

## Question

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0. \\
\end{cases}
$$

Give all solutions in parametric form and explain
why (0,0,0) always satisfies a homogeneous system.

## Solution

### 1. Form the augmented matrix

Using the variable order x, y, z gives

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
2 & 4 & -2 & \mid & 0 \\
1 & -1 & 2 & \mid & 0 \\
\end{pmatrix}.
$$

### 2. Eliminate entries below the first pivot

Apply

$$
R_2\leftarrow R_2-2R_1,
\qquad
R_3\leftarrow R_3-R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}.
$$

Swap rows 2 and 3:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}.
$$

The final row adds no restriction.

### 3. Find all solutions

The second row gives

$$
-3y+3z=0,
\qquad
y=z.
$$

Substitute into the first equation:

$$
x+2z-z=0,
\qquad
x=-z.
$$

There is no pivot in the z column, so z is free.
Set z=t. All solutions are

$$
(x,y,z)=(-t,t,t),
\qquad t\in\mathbb{R}.
$$

Since t can be any real number, there are infinitely
many solutions.

### 4. Why the zero vector is always a solution

A homogeneous system has zero on the right-hand side
of every equation.

Setting every unknown to zero makes every linear
combination on the left equal to zero as well.
Therefore, the zero vector always satisfies the system.

Here, t=0 gives the solution (0,0,0).

### 5. Verification of the entire solution family

Substitute (-t,t,t) into the original equations:

$$
-t+2t-t=0,
$$

$$
2(-t)+4t-2t=0,
$$

$$
-t-t+2t=0.
$$

All three equations hold for every real t,
confirming the complete solution family.