# Exercise 2. Determinant of a 3-by-3 Matrix

The given matrix is

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}.
$$

## 1. Sarrus' rule

For a 3-by-3 matrix,

$$
\det\begin{pmatrix}
a & b & c \\
d & e & f \\
g & h & i \\
\end{pmatrix}
=aei+bfg+cdh-ceg-bdi-afh.
$$

The sum of the three positive terms is

$$
1\cdot3\cdot5+2\cdot4\cdot2+(-1)\cdot0\cdot1
=15+16+0=31.
$$

The sum of the three terms to subtract is

$$
(-1)\cdot3\cdot2+2\cdot0\cdot5+1\cdot4\cdot1
=-6+0+4=-2.
$$

Therefore,

$$
\det A=31-(-2)=33.
$$

## 2. Verification using row operations

Adding a multiple of another row to a row
does not change the determinant.

First apply

$$
R_3\leftarrow R_3-2R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}.
$$

Next apply

$$
R_3\leftarrow R_3+R_2.
$$

The resulting matrix is upper triangular:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & 0 & 11 \\
\end{pmatrix}.
$$

The determinant of a triangular matrix is the product
of its diagonal entries:

$$
\det A=1\cdot3\cdot11=33.
$$

This agrees with the result obtained using Sarrus' rule.