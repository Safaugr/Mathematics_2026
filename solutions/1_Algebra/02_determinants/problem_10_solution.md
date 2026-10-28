# Exercise 10. Detecting Dependence

The given matrix is

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}.
$$

## Row dependence

The second row is twice the first:

$$
R_2=2R_1.
$$

Therefore, the rows are linearly dependent.
A square matrix with linearly dependent rows has determinant zero:

$$
\det A=0.
$$

Consequently, A is not invertible.

## Verification using a row operation

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

Adding a multiple of another row does not change the determinant.
The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5 \\
\end{pmatrix}.
$$

A matrix with a zero row has determinant zero,
confirming the result without a full determinant calculation.