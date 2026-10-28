# Exercise 1. Determinant of a 2-by-2 Matrix

For a 2-by-2 matrix, the determinant is

$$
\det\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
=ad-bc.
$$

## 1. First matrix

Let

$$
A=
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix}.
$$

Its determinant is

$$
\det A=3\cdot4-(-2)\cdot5=12+10=22.
$$

Since the determinant is nonzero, A is invertible.

## 2. Second matrix

Let

$$
B=
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}.
$$

Its determinant is

$$
\det B=1\cdot14-7\cdot2=14-14=0.
$$

Since the determinant is zero, B is not invertible.

## 3. Verification

For A, the inverse formula gives

$$
A^{-1}=\frac{1}{22}
\begin{pmatrix}
4 & 2 \\
-5 & 3 \\
\end{pmatrix}.
$$

Multiplication confirms the result:

$$
AA^{-1}=\frac{1}{22}
\begin{pmatrix}
12+10 & 6-6 \\
20-20 & 10+12 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

For B, the second row is twice the first row.
The rows are linearly dependent, confirming that
the determinant is zero and the matrix is not invertible.

## Conclusion

Only the first matrix is invertible:
its determinant is 22, while the second determinant is 0.