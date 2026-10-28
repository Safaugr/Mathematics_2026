# Exercise 5. Matrix Times Vector

The given matrix and vector are

$$
A=
\begin{pmatrix}
2 & -1 \\
1 & 3 \\
\end{pmatrix},
\qquad
x=
\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

## 1. Computing Ax

The matrix has size $2\times2$ and the vector has size $2\times1$.
The product is therefore defined and has size $2\times1$.

Multiply each row of A by the column vector x:

$$
Ax=
\begin{pmatrix}
2\cdot4+(-1)\cdot2 \\
1\cdot4+3\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

## 2. Linear combination of the columns

The columns of A are

$$
a_1=
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix},
\qquad
a_2=
\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}.
$$

The entries of x give the coefficients of the linear combination:

$$
Ax=4a_1+2a_2.
$$

Hence,

$$
Ax=
4\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}
+2\begin{pmatrix}
-1 \\
3 \\
\end{pmatrix}
=\begin{pmatrix}
8 \\
4 \\
\end{pmatrix}
+\begin{pmatrix}
-2 \\
6 \\
\end{pmatrix}
=\begin{pmatrix}
6 \\
10 \\
\end{pmatrix}.
$$

## Verification and Interpretation

The row-by-column calculation and the linear combination
of the columns both give the same vector, $(6,10)$.

Matrix-vector multiplication combines the columns of A,
using the corresponding entries of x as coefficients.