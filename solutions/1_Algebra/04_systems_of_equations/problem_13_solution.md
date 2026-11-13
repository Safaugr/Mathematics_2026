# Exercise 13. Does Every Equation Add New Information?

## Question

Consider the system

$$
x_1+x_2=10,\qquad
x_2+x_3=8,\qquad
x_1-x_3=2.
$$

Solve it and check whether all three equations
are independently necessary to describe the solution set.
If one follows from the others, show this by calculation.

## Solution

### 1. Identify the redundant equation

Subtract the second equation from the first:

$$
(x_1+x_2)-(x_2+x_3)=10-8.
$$

This simplifies to

$$
x_1-x_3=2,
$$

which is exactly the third equation.

Therefore, the third equation follows from the first two
and adds no new restriction.

### 2. Find all solutions

Choose x_2=t as the free variable.

The first equation gives

$$
x_1=10-t.
$$

The second equation gives

$$
x_3=8-t.
$$

Thus, all solutions are

$$
(x_1,x_2,x_3)=(10-t,t,8-t),
\qquad t\in\mathbb{R}.
$$

There are infinitely many solutions because t is arbitrary.

### 3. Confirm the redundancy by elimination

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}.
$$

Apply

$$
R_3\leftarrow R_3-R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & -1 & -1 & \mid & -8 \\
\end{pmatrix}.
$$

Next apply

$$
R_3\leftarrow R_3+R_2.
$$

The third row becomes entirely zero.
It represents 0=0, confirming that the third equation
adds no independent information.

### 4. Verification

Substitute the solution family into all three equations:

$$
(10-t)+t=10,
$$

$$
t+(8-t)=8,
$$

$$
(10-t)-(8-t)=2.
$$

All three equations hold for every real t.

### Conclusion

Only two independent equations are needed.
The third is the difference of the first two,
so removing it does not change the solution set.