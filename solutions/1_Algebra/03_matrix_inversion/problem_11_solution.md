# Exercise 11. Parameter and Invertibility

## Question

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix},
$$

find all t for which the matrix is invertible,
and then give a formula for its inverse.

Explain what happens to this formula at the excluded values.

## Solution

### 1. Compute the determinant

Using the 2-by-2 determinant formula,

$$
\det A(t)=1\cdot1-t\cdot t=1-t^2.
$$

The matrix is invertible exactly when

$$
1-t^2\ne0.
$$

Since $1-t^2=(1-t)(1+t)$, the excluded values are

$$
t=1,\qquad t=-1.
$$

Thus, A(t) is invertible for every real t except 1 and -1.

### 2. Formula for the inverse

Apply the 2-by-2 inverse formula:

$$
A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix},
\qquad t\ne\pm1.
$$

### 3. What happens at the excluded values?

At t=1 or t=-1, the denominator is zero,
so the inverse formula is undefined.

At t=1, the matrix is

$$
A(1)=
\begin{pmatrix}
1 & 1 \\
1 & 1 \\
\end{pmatrix}.
$$

Its rows are identical, so it is not invertible.

At t=-1, the matrix is

$$
A(-1)=
\begin{pmatrix}
1 & -1 \\
-1 & 1 \\
\end{pmatrix}.
$$

Its second row is the negative of its first row,
so it is also not invertible.

These are genuine failures of invertibility,
rather than merely limitations of the formula.

### 4. Verification

For t different from 1 and -1,

$$
A(t)A(t)^{-1}
=\frac{1}{1-t^2}
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}
=\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & -t+t \\
t-t & 1-t^2 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

Multiplying in the opposite order gives the same identity matrix.
This confirms the inverse for every allowed value of t.