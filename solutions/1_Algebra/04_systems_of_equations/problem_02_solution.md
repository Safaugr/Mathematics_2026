# Exercise 2. Gaussian Elimination — One Solution

## Question

Solve using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2. \\
\end{cases}
$$

After solving, substitute the result into all equations
and check consistency.

## Solution

### 1. Form the augmented matrix

Using the variable order x, y, z gives

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}.
$$

Elementary row operations preserve the solution set.

### 2. Eliminate x from the second and third rows

Apply

$$
R_2\leftarrow R_2-2R_1,
\qquad
R_3\leftarrow R_3-R_1.
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}.
$$

### 3. Swap rows to obtain a convenient pivot

Interchange rows 2 and 3:

$$
R_2\leftrightarrow R_3.
$$

This gives

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}.
$$

### 4. Eliminate y from the third row

Apply

$$
R_3\leftarrow R_3+3R_2.
$$

The matrix becomes upper triangular:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}.
$$

### 5. Back-substitution

The third row gives

$$
-7z=-21,
\qquad
z=3.
$$

The second row gives

$$
y-2z=-4,
\qquad
y-6=-4,
\qquad
y=2.
$$

The first row gives

$$
x+y+z=6,
\qquad
x+2+3=6,
\qquad
x=1.
$$

Thus,

$$
(x,y,z)=(1,2,3).
$$

There is a nonzero pivot for every variable,
so the solution is unique.

### 6. Verification in the original equations

First equation:

$$
1+2+3=6.
$$

Second equation:

$$
2\cdot1-2+3=3.
$$

Third equation:

$$
1+2\cdot2-3=2.
$$

All three original equations are satisfied,
confirming the solution.