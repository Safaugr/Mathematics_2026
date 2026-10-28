# Exercise 5. Row Operations

The given matrix is

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}.
$$

## Method

Adding a multiple of one row to another row does not
change the determinant.

We use these operations to obtain an upper triangular matrix,
then multiply its diagonal entries.

## 1. Eliminate the first entry of row 2

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

The new second row is

$$
(2,1,0)-2(1,2,3)=(0,-3,-6).
$$

This gives

$$
A_1=
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2 \\
\end{pmatrix}.
$$

The determinant is unchanged:

$$
\det A_1=\det A.
$$

## 2. Eliminate the first entry of row 3

Apply

$$
R_3\leftarrow R_3+R_1.
$$

The new third row is

$$
(-1,4,2)+(1,2,3)=(0,6,5).
$$

Therefore,

$$
A_2=
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5 \\
\end{pmatrix}.
$$

Again, the determinant is unchanged:

$$
\det A_2=\det A.
$$

## 3. Eliminate the second entry of row 3

Using the current second row, apply

$$
R_3\leftarrow R_3+2R_2.
$$

The new third row is

$$
(0,6,5)+2(0,-3,-6)=(0,0,-7).
$$

The resulting matrix is

$$
A_3=
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7 \\
\end{pmatrix}.
$$

This operation also preserves the determinant.

## 4. Compute the determinant

The final matrix is upper triangular, so

$$
\det A=\det A_3=1\cdot(-3)\cdot(-7)=21.
$$

No rows were swapped or multiplied by a scalar,
so no sign or scaling correction is needed.

## Verification by expansion

Expanding the original determinant along the first row gives

$$
\det A
=1(1\cdot2-0\cdot4)
-2(2\cdot2-0\cdot(-1))
+3(2\cdot4-1\cdot(-1))
=2-8+27
=21.
$$

Both methods give the same result.