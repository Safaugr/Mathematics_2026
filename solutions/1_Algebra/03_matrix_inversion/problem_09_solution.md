# Exercise 9. Matrix Equation

## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix},
$$

solve the equation AX=B for X.

Before calculating, decide on which side of the equation
the inverse of A must be used.
Then check the result by computing AX.

## Solution

### 1. Choose the multiplication side

Since A multiplies X on the left, multiply both sides
of AX=B on the left by the inverse of A:

$$
A^{-1}(AX)=A^{-1}B.
$$

Associativity gives

$$
(A^{-1}A)X=IX=X.
$$

Therefore,

$$
X=A^{-1}B.
$$

Multiplying on the right would not place the inverse
next to A and would not isolate X directly.

### 2. Find the inverse of A

The determinant is

$$
\det A=1\cdot1-2\cdot0=1.
$$

Using the 2-by-2 inverse formula,

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$

### 3. Compute X

$$
X=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
=\begin{pmatrix}
3-4 & 1-8 \\
2 & 4 \\
\end{pmatrix}
=\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
$$

### 4. Verification

Substitute X into the original equation:

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}
=\begin{pmatrix}
-1+4 & -7+8 \\
2 & 4 \\
\end{pmatrix}
=\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}
=B.
$$

Thus, the computed X satisfies the equation.
Since A is invertible, this solution is unique.