# Exercise 15. Two Methods for Solving the Same System

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix},
$$

solve Ax=b in two ways:

1. Using the inverse: $x=A^{-1}b$.
2. Using Gaussian elimination.

Compare both solutions and the number of essential steps.
State which method was simpler in this example.

## Solution

### 1. Solve using the inverse

First compute the determinant:

$$
\det A=2\cdot3-1\cdot1=5.
$$

Since it is nonzero, the inverse exists:

$$
A^{-1}=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

Then

$$
x=A^{-1}b=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
=\frac15
\begin{pmatrix}
21-8 \\
-7+16 \\
\end{pmatrix}
=\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}.
$$

### 2. Solve using Gaussian elimination

The system is

$$
\begin{cases}
2x_1+x_2=7, \\
x_1+3x_2=8. \\
\end{cases}
$$

Its augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}.
$$

Eliminate the first entry of the second row:

$$
R_2\leftarrow R_2-\frac12R_1.
$$

This gives

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
0 & \frac52 & \mid & \frac92 \\
\end{pmatrix}.
$$

The second equation gives

$$
\frac52x_2=\frac92,
\qquad
x_2=\frac95.
$$

Substitute into the first equation:

$$
2x_1+\frac95=7,
\qquad
2x_1=\frac{26}{5},
\qquad
x_1=\frac{13}{5}.
$$

Thus, Gaussian elimination gives the same solution:

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}.
$$

### 3. Compare the methods

The inverse method required three main stages:

1. Calculate the determinant.
2. Construct the inverse matrix.
3. Multiply the inverse by b.

Gaussian elimination required one elimination row operation,
followed by solving for x_2 and back-substituting for x_1.

For this single system, elimination was simpler:
it found the required vector directly without constructing
the entire inverse matrix.

If the inverse were already known, using it would be convenient.
It could also be reused for other right-hand sides.

### 4. Verification

Substitute the solution into both original equations:

$$
2\left(\frac{13}{5}\right)+\frac95
=\frac{35}{5}
=7,
$$

$$
\frac{13}{5}+3\left(\frac95\right)
=\frac{40}{5}
=8.
$$

Both equations are satisfied, confirming the result.