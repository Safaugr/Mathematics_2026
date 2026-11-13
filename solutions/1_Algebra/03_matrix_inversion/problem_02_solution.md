# Exercise 2. Formula for a 2-by-2 Matrix

## Question

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a 2-by-2 matrix.
At the end, check the result by computing one product with A.

## Solution

### 1. Check invertibility

The determinant is

$$
\det A=3\cdot4-2\cdot5=12-10=2.
$$

Since the determinant is nonzero, A is invertible.

### 2. Apply the inverse formula

For a 2-by-2 matrix with nonzero determinant,

$$
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}^{-1}
=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}.
$$

Swap the diagonal entries, change the signs of
the other two entries, and divide by the determinant:

$$
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}
=\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2} \\
\end{pmatrix}.
$$

### 3. Verification by multiplication

Multiply A by the proposed inverse:

$$
AA^{-1}=\frac{1}{2}
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}
=\frac{1}{2}
\begin{pmatrix}
12-10 & -6+6 \\
20-20 & -10+12 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

The product equals the identity matrix,
confirming the inverse.