# Exercise 5. Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix},
$$

determine the number of solutions and write them
in parametric form. Explain how you know how many
variables may be chosen freely.

## Solution

Using the variable order x, y, z, the matrix represents

$$
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0. \\
\end{cases}
$$

There are pivots in the x and y columns, but no pivot
in the z column. There is no contradictory row,
so the system is consistent.

There are three variables and two pivots,
leaving one free variable. Set z=t, where t is any real number.

From the second equation,

$$
y=1-2t.
$$

Substitute this into the first equation:

$$
x+2(1-2t)-t=3,
\qquad
x=1+5t.
$$

Therefore, all solutions are

$$
(x,y,z)=(1+5t,1-2t,t),
\qquad t\in\mathbb{R}.
$$

Every real value of t gives a distinct solution,
so the system has infinitely many solutions.

### Verification

Substituting the parametric expressions gives

$$
(1+5t)+2(1-2t)-t=3,
$$

$$
(1-2t)+2t=1.
$$

Both nonzero rows are satisfied for every real t.
The final row is always 0=0, confirming the solution family.