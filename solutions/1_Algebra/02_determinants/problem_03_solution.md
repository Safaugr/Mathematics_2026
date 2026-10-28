# Exercise 3. Swapping Two Rows

The given matrix is

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1 \\
\end{pmatrix}.
$$

## 1. Computing the determinant of A

Expand along the first row, using the signs +, -, +:

$$
\det A
=1(3\cdot1-1\cdot1)-2(0\cdot1-1\cdot2)+0
=2-2(-2)
=6.
$$

## 2. Swapping the first two rows

The new matrix is

$$
B=
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1 \\
\end{pmatrix}.
$$

Swapping two rows changes the sign of the determinant.
Therefore, before calculating, we predict

$$
\det B=-\det A=-6.
$$

## 3. Verification by direct calculation

Expand B along its first row:

$$
\det B
=0-3(1\cdot1-0\cdot2)+1(1\cdot1-2\cdot2)
=-3+(1-4)
=-6.
$$

This agrees with the prediction.

## Conclusion

$$
\det A=6,\qquad \det B=-6.
$$

Interchanging two rows reverses the sign of the determinant
while preserving its absolute value.