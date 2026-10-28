# Exercise 6. Transpose

The given matrices are

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}.
$$

## 1. Transposes

Transposition turns each row into the corresponding column.

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix},
\qquad
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}.
$$

A has size $2\times3$, so its transpose has size $3\times2$.
B has size $3\times2$, so its transpose has size $2\times3$.

## 2. Computing AB

Multiply each row of A by each column of B:

$$
AB=
\begin{pmatrix}
1\cdot1+2\cdot2+3(-1) & 1\cdot0+2\cdot1+3\cdot3 \\
4\cdot1+5\cdot2+6(-1) & 4\cdot0+5\cdot1+6\cdot3 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 11 \\
8 & 23 \\
\end{pmatrix}.
$$

Therefore,

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}.
$$

## 3. Computing the product of the transposes

$$
B^TA^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6 \\
\end{pmatrix}
=\begin{pmatrix}
1+4-3 & 4+10-6 \\
0+2+9 & 0+5+18 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 8 \\
11 & 23 \\
\end{pmatrix}.
$$

## Verification and Explanation

Both calculations give exactly the same matrix, so

$$
(AB)^T=B^TA^T.
$$

The order reverses because transposition exchanges rows
and columns. The entry in row i, column j of AB becomes
the entry in row j, column i of its transpose.

In index notation,

$$
\bigl((AB)^T\bigr)_{ij}
=(AB)_{ji}
=\sum_{k=1}^{3}a_{jk}b_{ki}
=\sum_{k=1}^{3}b_{ki}a_{jk}
=(B^TA^T)_{ij}.
$$