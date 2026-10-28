# Exercise 11. Shortening the Calculation with Row Operations

The given matrix is

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}.
$$

## 1. Create zeros in the first column

Apply

$$
R_2\leftarrow R_2-R_1,
\qquad
R_3\leftarrow R_3-R_1.
$$

Adding a multiple of another row to a row
does not change the determinant.

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}.
$$

## 2. Obtain an upper triangular matrix

Using the current second row, apply

$$
R_3\leftarrow R_3-2R_2.
$$

This also preserves the determinant and gives

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

The determinant is the product of the diagonal entries:

$$
\det A=1\cdot1\cdot1=1.
$$

## 3. Verification

Expanding the original determinant along the first row gives

$$
\det A
=1(18-16)-2(6-4)+3(4-3)
=2-4+3
=1.
$$

Both methods give the same result.