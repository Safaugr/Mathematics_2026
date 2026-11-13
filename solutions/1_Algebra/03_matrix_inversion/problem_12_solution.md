# Exercise 12. Finding Inverses Without Starting from Scratch

## Question

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

Without finding A, compute the inverses of 3A,
the transpose of A, and the square of A:

$$
(3A)^{-1},\qquad (A^T)^{-1},\qquad (A^2)^{-1}.
$$

Justify each result using the appropriate property.

## Solution

### 1. Inverse of 3A

For a nonzero scalar k,

$$
(kA)^{-1}=\frac{1}{k}A^{-1}.
$$

Therefore,

$$
(3A)^{-1}=\frac13
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
=\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23 \\
\end{pmatrix}.
$$

The reciprocal scalar cancels the factor 3
when the matrices are multiplied.

### 2. Inverse of the transpose

Taking a transpose and taking an inverse satisfy

$$
(A^T)^{-1}=(A^{-1})^T.
$$

Transposing the given inverse gives

$$
(A^T)^{-1}=
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}.
$$

### 3. Inverse of the square

The inverse-of-a-product rule gives

$$
(A^2)^{-1}=(AA)^{-1}=A^{-1}A^{-1}.
$$

Thus,

$$
(A^2)^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
=\begin{pmatrix}
4+3 & -2-2 \\
-6-6 & 3+4 \\
\end{pmatrix}
=\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}.
$$

### 4. Verification of the properties

For the scalar multiple,

$$
(3A)\left(\frac13A^{-1}\right)=AA^{-1}=I.
$$

For the transpose, transpose the identity A^{-1}A=I:

$$
A^T(A^{-1})^T=(A^{-1}A)^T=I.
$$

For the square,

$$
A^2(A^{-1}A^{-1})
=A(AA^{-1})A^{-1}
=AA^{-1}
=I.
$$

Each proposed inverse therefore produces the identity,
without requiring the entries of A.