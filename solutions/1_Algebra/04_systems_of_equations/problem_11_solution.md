# Exercise 11. A Parameter in a System of Three Equations

## Question

Analyze the number of solutions depending on t:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3. \\
\end{cases}
$$

Use elimination and separately analyze the parameter values
for which a standard calculation step ceases to be valid.

## Solution

### 1. Eliminate x from the last two equations

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}.
$$

Apply

$$
R_2\leftarrow R_2-R_1,
\qquad
R_3\leftarrow R_3-R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}.
$$

Solving the last two rows requires division by t-1.
Therefore, t=1 must be considered separately.

### 2. Case t different from 1

When t is not 1, both lower pivots are nonzero.
The last two equations give

$$
y=\frac{1}{t-1},
\qquad
z=\frac{2}{t-1}.
$$

Substituting into the first equation gives

$$
x=1-y-z
=1-\frac{3}{t-1}
=\frac{t-4}{t-1}.
$$

Thus, there is exactly one solution:

$$
(x,y,z)=
\left(
\frac{t-4}{t-1},
\frac{1}{t-1},
\frac{2}{t-1}
\right),
\qquad t\ne1.
$$

### 3. Case t=1

The eliminated matrix becomes

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & 0 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 2 \\
\end{pmatrix}.
$$

The second row requires 0=1, which is impossible.
Therefore, the system has no solution.

In the original system, t=1 makes all three
left-hand sides equal to x+y+z, while the right-hand
sides are 1, 2, and 3. These conditions cannot hold together.

### 4. Verification for t different from 1

The first equation is satisfied because

$$
x+y+z
=\frac{t-4+1+2}{t-1}
=1.
$$

For the second equation,

$$
x+ty+z
=\frac{t-4+t+2}{t-1}
=\frac{2t-2}{t-1}
=2.
$$

For the third equation,

$$
x+y+tz
=\frac{t-4+1+2t}{t-1}
=\frac{3t-3}{t-1}
=3.
$$

All three equations are satisfied for every allowed t.

### 5. Conclusion

- For t different from 1, there is exactly one solution.
- For t=1, there is no solution.
- No value of t gives infinitely many solutions.