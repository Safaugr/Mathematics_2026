# Exercise 10. Inverse of a Diagonal Matrix

## Question

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},
\qquad
E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},
$$

without using Gauss–Jordan elimination, decide which
matrix is invertible.

For the invertible matrix, give the inverse and check
the result by multiplication.

## Solution

### 1. Invertibility of D

A diagonal matrix is invertible exactly when
all its diagonal entries are nonzero.

The diagonal entries of D are 2, -3, and 5.
They are all nonzero, so D is invertible.

Its inverse has the reciprocal diagonal entries:

$$
D^{-1}=
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15 \\
\end{pmatrix}.
$$

### 2. Verification by multiplication

Multiplying diagonal matrices multiplies
the corresponding diagonal entries:

$$
DD^{-1}=
\begin{pmatrix}
2\cdot\frac12 & 0 & 0 \\
0 & (-3)\left(-\frac13\right) & 0 \\
0 & 0 & 5\cdot\frac15 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
=I.
$$

The same calculation in the opposite order gives

$$
D^{-1}D=I.
$$

Thus, the proposed matrix satisfies the definition
of the inverse.

### 3. Invertibility of E

The second diagonal entry of E is zero.
Its determinant is therefore

$$
\det E=2\cdot0\cdot5=0.
$$

Hence, E is not invertible.

This can also be seen from the nonzero vector

$$
v=
\begin{pmatrix}
0 \\
1 \\
0 \\
\end{pmatrix}.
$$

Multiplying gives Ev=0.
If an inverse existed, multiplying by it would imply v=0,
contradicting the choice of v.

### 4. Conclusion

D is invertible, with the inverse given above.
E has no inverse because its zero diagonal entry
causes a loss of information.