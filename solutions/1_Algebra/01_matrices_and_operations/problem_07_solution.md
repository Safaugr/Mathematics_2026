# Exercise 7. Identity Matrix, Zero Matrix, and Powers

The given matrix is

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}.
$$

The identity and zero matrices of the same size are

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix},
\qquad
0=
\begin{pmatrix}
0 & 0 \\
0 & 0 \\
\end{pmatrix}.
$$

## 1. Multiplication by the identity matrix

$$
AI=
\begin{pmatrix}
2\cdot1+1\cdot0 & 2\cdot0+1\cdot1 \\
0\cdot1+2\cdot0 & 0\cdot0+2\cdot1 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
=A.
$$

Similarly,

$$
IA=
\begin{pmatrix}
1\cdot2+0\cdot0 & 1\cdot1+0\cdot2 \\
0\cdot2+1\cdot0 & 0\cdot1+1\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
=A.
$$

The identity matrix is the neutral element for matrix multiplication.

## 2. Addition of the zero matrix

$$
A+0=
\begin{pmatrix}
2+0 & 1+0 \\
0+0 & 2+0 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
=A.
$$

The zero matrix is the neutral element for matrix addition.

## 3. Computing the square

A matrix power uses matrix multiplication, not entry-by-entry powers.

$$
A^2=AA=
\begin{pmatrix}
2\cdot2+1\cdot0 & 2\cdot1+1\cdot2 \\
0\cdot2+2\cdot0 & 0\cdot1+2\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
4 & 4 \\
0 & 4 \\
\end{pmatrix}.
$$

## 4. Computing the cube

$$
A^3=A^2A=
\begin{pmatrix}
4\cdot2+4\cdot0 & 4\cdot1+4\cdot2 \\
0\cdot2+4\cdot0 & 0\cdot1+4\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
8 & 12 \\
0 & 8 \\
\end{pmatrix}.
$$

## 5. Pattern in successive powers

The diagonal entries are $2,4,8$, and the lower-left entry remains zero.
The upper-right entries are $1,4,12$.

These results suggest that, for every integer $n\ge1$,

$$
A^n=
\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n \\
\end{pmatrix}.
$$

## Verification of the pattern

For $n=1$, the formula gives A.

Assume that the formula holds for some integer $n\ge1$.
Multiplying by A gives

$$
A^{n+1}=
\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
=\begin{pmatrix}
2^{n+1} & 2^n+n2^n \\
0 & 2^{n+1} \\
\end{pmatrix}
=\begin{pmatrix}
2^{n+1} & (n+1)2^n \\
0 & 2^{n+1} \\
\end{pmatrix}.
$$

This is the stated formula with n replaced by n+1,
so the pattern holds by mathematical induction.