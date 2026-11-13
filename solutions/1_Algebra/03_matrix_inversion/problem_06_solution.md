# Exercise 6. Solving a System Using the Inverse

## Question

Solve

$$
Ax=b,
$$

where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$. Then substitute the resulting vector
back into the equation and check the result.

## Solution

### 1. Check invertibility

The determinant is

$$
\det A=2\cdot3-1\cdot1=5.
$$

Since the determinant is nonzero, A is invertible
and the system has exactly one solution.

### 2. Find the inverse

Using the formula for a 2-by-2 matrix,

$$
A^{-1}=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

### 3. Compute the solution vector

Multiplying Ax=b on the left by the inverse gives
$x=A^{-1}b$. Therefore,

$$
x=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
=\frac15
\begin{pmatrix}
15-7 \\
-5+14 \\
\end{pmatrix}
=\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}.
$$

### 4. Verification by substitution

Substitute the solution into the original equation:

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}
=\begin{pmatrix}
\frac{16}{5}+\frac95 \\
\frac85+\frac{27}{5} \\
\end{pmatrix}
=\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}
=b.
$$

Both equations are satisfied, confirming the solution.