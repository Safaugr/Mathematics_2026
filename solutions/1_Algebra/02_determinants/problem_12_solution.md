# Exercise 12. A Parameter Revealed by a Row Operation

The given matrix is

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}.
$$

## 1. Apply the suggested row operation

Apply

$$
R_2\leftarrow R_2-2R_1.
$$

The new second row is

$$
(2,4,t)-2(1,2,3)=(0,0,t-6).
$$

This operation preserves the determinant, giving

$$
\det A(t)=
\det\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}.
$$

## 2. Compute the determinant

Expand along the first column:

$$
\det A(t)
=1\bigl(0\cdot1-(t-6)\cdot1\bigr)
=6-t.
$$

The matrix is not invertible exactly when its determinant is zero:

$$
6-t=0,
\qquad
t=6.
$$

For every other real value of t, the determinant is nonzero,
so the matrix is invertible.

## 3. Row dependence at the exceptional value

When t=6, the original second row is

$$
(2,4,6)=2(1,2,3).
$$

Thus, the second row is twice the first row.
The rows are linearly dependent, and the suggested
row operation produces a zero row.

This confirms that A(6) is not invertible.

## Verification

Expanding the original determinant along the first row gives

$$
\det A(t)
=1(4-t)-2(2)+3(2)
=4-t-4+6
=6-t.
$$

This agrees with the row-operation calculation.