# Exercise 2. Addition and Scalar Multiplication

## Method

Matrix addition and subtraction are performed entry by entry.
Scalar multiplication multiplies every entry by the scalar.

## 1. Addition

$$
A+B=
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5 \\
\end{pmatrix}
=
\begin{pmatrix}
5 & 0 \\
-1 & 8 \\
\end{pmatrix}.
$$

## 2. Subtraction

$$
A-B=
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5 \\
\end{pmatrix}
=
\begin{pmatrix}
-3 & 4 \\
-1 & -2 \\
\end{pmatrix}.
$$

## 3. Scalar multiplication and subtraction

First multiply each entry by the corresponding scalar:

$$
3A=
\begin{pmatrix}
3 & 6 \\
-3 & 9 \\
\end{pmatrix},
\qquad
2B=
\begin{pmatrix}
8 & -4 \\
0 & 10 \\
\end{pmatrix}.
$$

Therefore,

$$
3A-2B=
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10 \\
\end{pmatrix}
=
\begin{pmatrix}
-5 & 10 \\
-3 & -1 \\
\end{pmatrix}.
$$

## 4. Why the sizes must match

Matrix addition pairs entries in the same row and column.
The matrices must have the same number of rows and columns
so that every entry has a corresponding entry.
Here, both matrices have size $2\times2$.

## Verification

Adding B back to A-B gives A:

$$
(A-B)+B=
\begin{pmatrix}
-3+4 & 4+(-2) \\
-1+0 & -2+5 \\
\end{pmatrix}
=
\begin{pmatrix}
1 & 2 \\
-1 & 3 \\
\end{pmatrix}
=A.
$$