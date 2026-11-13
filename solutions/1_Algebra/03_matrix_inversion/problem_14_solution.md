# Exercise 14. A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix A satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a 2-by-2 matrix different
from I and -I that satisfies this condition,
and verify it by multiplication.

## Solution

### 1. Use the definition of the inverse

The condition A^2=I means

$$
AA=I.
$$

A matrix B is the inverse of A if AB=BA=I.

Taking B=A satisfies both equalities, since both
products are AA. Therefore, A is invertible and

$$
A^{-1}=A.
$$

### 2. Construct an example

Choose

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

This matrix is different from both I and -I:
its diagonal entries are zero and its off-diagonal
entries are one.

### 3. Verification by multiplication

$$
A^2=
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0 \\
\end{pmatrix}
=\begin{pmatrix}
0\cdot0+1\cdot1 & 0\cdot1+1\cdot0 \\
1\cdot0+0\cdot1 & 1\cdot1+0\cdot0 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

Thus, the example satisfies A^2=I and is its own inverse.

### 4. Interpretation

The matrix swaps the two coordinates of a vector:

$$
A
\begin{pmatrix}
x \\
y \\
\end{pmatrix}
=\begin{pmatrix}
y \\
x \\
\end{pmatrix}.
$$

Applying the same transformation again restores
the original vector. This explains geometrically
why the transformation is its own inverse.