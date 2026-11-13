# Exercise 7. Inverse of a Product

## Question

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix},
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$.
Check that the results are the same and explain
the meaning of the reversed order.

## Solution

### 1. Compute AB

Using row-by-column multiplication,

$$
AB=
\begin{pmatrix}
1\cdot2+1\cdot0 & 1\cdot0+1\cdot3 \\
0\cdot2+1\cdot0 & 0\cdot0+1\cdot3 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}.
$$

Its determinant is

$$
\det(AB)=2\cdot3-3\cdot0=6.
$$

Therefore, AB is invertible.

### 2. Find the inverse of AB directly

Using the 2-by-2 inverse formula,

$$
(AB)^{-1}=\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}
=\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
$$

### 3. Compute the individual inverses

The determinant of A is 1, so

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

B is diagonal with nonzero diagonal entries.
Its inverse has the reciprocal diagonal entries:

$$
B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}.
$$

Multiplying in reversed order gives

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
$$

The two calculations give the same result:

$$
(AB)^{-1}=B^{-1}A^{-1}.
$$

### 4. Explain the reversed order

The transformation AB applies B first and then A.

To undo the combined transformation, first undo A
and then undo B. Since the rightmost matrix acts first,
this inverse transformation is written as B^{-1}A^{-1}.

Algebraically, the reversed order places each inverse
next to its corresponding matrix:

$$
(AB)(B^{-1}A^{-1})
=A(BB^{-1})A^{-1}
=AA^{-1}
=I.
$$

Similarly,

$$
(B^{-1}A^{-1})(AB)
=B^{-1}(A^{-1}A)B
=B^{-1}B
=I.
$$

### 5. Numerical verification

Using the computed matrices,

$$
(AB)(AB)^{-1}=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}
=\begin{pmatrix}
1 & -1+1 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

This confirms the inverse.