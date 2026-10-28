# Exercise 4. Matrix Multiplication and Noncommutativity

The given matrices are

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

## Method

Both matrices have size $2\times2$, so both products are defined.

Each entry of a product is calculated by multiplying
corresponding entries of a row of the first matrix
and a column of the second, then adding the results.

## 1. Computing AB

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1 \\
\end{pmatrix}
=\begin{pmatrix}
8 & 2 \\
3 & 1 \\
\end{pmatrix}.
$$

## 2. Computing BA

$$
BA=
\begin{pmatrix}
2\cdot1+0\cdot0 & 2\cdot2+0\cdot1 \\
3\cdot1+1\cdot0 & 3\cdot2+1\cdot1 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 4 \\
3 & 7 \\
\end{pmatrix}.
$$

## 3. Comparison

The top-left entry of AB is 8, while the top-left entry of BA is 2.
Therefore,

$$
AB\ne BA.
$$

Matrix multiplication is not commutative in general:
changing the order of the factors can change the result.

## Verification

Use the vector

$$
x=
\begin{pmatrix}
1 \\
0 \\
\end{pmatrix}.
$$

Applying B first and then A gives

$$
A(Bx)=
A
\begin{pmatrix}
2 \\
3 \\
\end{pmatrix}
=\begin{pmatrix}
8 \\
3 \\
\end{pmatrix}
=(AB)x.
$$

Applying A first and then B gives

$$
B(Ax)=
B
\begin{pmatrix}
1 \\
0 \\
\end{pmatrix}
=\begin{pmatrix}
2 \\
3 \\
\end{pmatrix}
=(BA)x.
$$

These calculations check the first column of each product.
The different results also confirm that AB and BA are different.