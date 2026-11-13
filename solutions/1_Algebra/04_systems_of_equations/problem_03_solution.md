# Exercise 3. Inconsistent System

## Question

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7. \\
\end{cases}
$$

Show how the contradiction appears in the matrix
after elimination and interpret it in terms of equations.

## Solution

### 1. Form the augmented matrix

Using the variable order x, y gives

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}.
$$

### 2. Eliminate the second row's first entry

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}.
$$

The second row represents

$$
0x+0y=1,
$$

which simplifies to the contradiction

$$
0=1.
$$

Therefore, the system is inconsistent and has no solution.

### 3. Interpretation in terms of equations

Doubling the first original equation gives

$$
2x+4y=6.
$$

However, the second original equation requires

$$
2x+4y=7.
$$

The same expression cannot equal both 6 and 7.
This is exactly the contradiction exposed by elimination.

### 4. Geometric interpretation

The equations can be written as

$$
y=-\frac12x+\frac32,
$$

$$
y=-\frac12x+\frac74.
$$

They describe distinct parallel lines:
their slopes are equal, but their intercepts differ.

The lines do not intersect, confirming that
there is no solution.