# Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1, \\
\end{cases}
$$

and

$$
\begin{cases}
2x+y=1, \\
x-y=4. \\
\end{cases}
$$

Compare the successive elimination steps.
Which part of the calculation is the same in both cases,
and why?

## Solution

### 1. First system

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1 \\
\end{pmatrix}.
$$

Swap the rows to obtain a first pivot equal to 1:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5 \\
\end{pmatrix}.
$$

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

This gives

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3 \\
\end{pmatrix}.
$$

The second row gives y=1.
Back-substitution into x-y=1 gives x=2.

Thus, the first solution is

$$
(x,y)=(2,1).
$$

### 2. Second system

The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4 \\
\end{pmatrix}.
$$

Swap the rows:

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1 \\
\end{pmatrix}.
$$

Apply the same elimination operation:

$$
R_2\leftarrow R_2-2R_1.
$$

This gives

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7 \\
\end{pmatrix}.
$$

The second row gives

$$
y=-\frac73.
$$

Back-substitution into x-y=4 gives

$$
x=4+y=4-\frac73=\frac53.
$$

Thus, the second solution is

$$
(x,y)=\left(\frac53,-\frac73\right).
$$

### 3. Comparison

Both systems have the same coefficient matrix:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & -1 \\
\end{pmatrix}.
$$

Therefore, the same row swap and elimination operation
produce the same triangular coefficient matrix:

$$
\begin{pmatrix}
1 & -1 \\
0 & 3 \\
\end{pmatrix}.
$$

Only the right-hand sides differ.
The row operations must also be applied to those
right-hand sides, producing different solution vectors.

The elimination of the coefficient matrix can be reused
because the required operations depend on A,
not on the right-hand side.

Both triangular systems have nonzero pivots
for both variables, so each solution is unique.

### 4. Verification

For the first solution,

$$
2\cdot2+1=5,
\qquad
2-1=1.
$$

For the second solution,

$$
2\left(\frac53\right)-\frac73=1,
$$

$$
\frac53-\left(-\frac73\right)=4.
$$

Both solutions satisfy their respective original systems.