# Exercise 13. Undoing a Composite Transformation

## Question

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},
\qquad
H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear.

For T=HS, find the inverse in two ways:

1. First compute T, then its inverse.
2. Use the identity $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute H^{-1}S^{-1}
and verify that the incorrect order gives a different matrix.

Explain the rule: when undoing a composition of operations,
we undo them from the end.

## Solution

### 1. Compute T and find its inverse directly

Multiplying gives

$$
T=HS=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Its determinant is

$$
\det T=2\cdot1-1\cdot0=2.
$$

Using the 2-by-2 inverse formula,

$$
T^{-1}=\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}
=\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}.
$$

### 2. Use the inverse-of-a-product rule

The individual inverses are

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix},
\qquad
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

Therefore,

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}.
$$

Both methods give the same inverse.

### 3. Compare with the incorrect order

Reversing these inverse factors gives

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

Its upper-right entry is -1 instead of -1/2,
so it differs from the inverse of T.

Indeed,

$$
T(H^{-1}S^{-1})=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
\ne I.
$$

### 4. Geometric explanation

T=HS applies S first and then H.

To undo this transformation, first undo H
and then undo S. Because the rightmost matrix acts first,
the inverse is written as S^{-1}H^{-1}.

Thus, reversing a composition requires undoing
the operations in reverse order.

### 5. Verification of the correct inverse

$$
TT^{-1}=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}
=\begin{pmatrix}
1 & -1+1 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

Multiplying in the opposite order also gives

$$
T^{-1}T=
\begin{pmatrix}
1 & \frac12-\frac12 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

This confirms the result.