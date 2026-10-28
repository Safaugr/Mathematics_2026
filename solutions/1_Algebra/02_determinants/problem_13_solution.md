# Exercise 13. Determinant by Elimination

The given matrix is

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}.
$$

## 1. Eliminate the first entry of row 2

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2 \\
\end{pmatrix}.
$$

Adding a multiple of another row preserves the determinant.

## 2. Eliminate the first entry of row 3

Apply

$$
R_3\leftarrow R_3-R_1.
$$

The result is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}.
$$

The determinant is unchanged.

## 3. Eliminate the second entry of row 3

Using the current second row, apply

$$
R_3\leftarrow R_3+2R_2.
$$

Since

$$
(0,-2,-1)+2(0,1,1)=(0,0,1),
$$

the resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

This operation also preserves the determinant.

## 4. Compute the determinant

The final matrix is upper triangular:

$$
\det A=1\cdot1\cdot1=1.
$$

No row swaps or row scalings were used,
so no correction factor is needed.

## Verification

Expanding the original determinant along the first row gives

$$
\det A
=1(10-0)-2(4-7)+3(0-5)
=10+6-15
=1.
$$

Both methods give the same result.