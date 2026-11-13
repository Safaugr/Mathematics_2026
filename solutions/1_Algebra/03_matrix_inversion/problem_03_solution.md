# Exercise 3. When Does the Inverse Not Exist?

## Question

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix},
$$

explain in two ways why the inverse does not exist:
using the determinant and using dependence between the rows.

## Solution

### 1. Using the determinant

For a 2-by-2 matrix, the determinant is ad-bc:

$$
\det A=2\cdot2-4\cdot1=4-4=0.
$$

A square matrix is invertible if and only if
its determinant is nonzero.

Since the determinant is zero, A has no inverse.

### 2. Using row dependence

The first row is twice the second row:

$$
(2,4)=2(1,2).
$$

Therefore, the rows are linearly dependent.
One row repeats the information contained in the other,
so the matrix is not invertible.

### 3. Verification using a nonzero vector

Take

$$
v=
\begin{pmatrix}
-2 \\
1 \\
\end{pmatrix}.
$$

Then

$$
Av=
\begin{pmatrix}
2(-2)+4\cdot1 \\
1(-2)+2\cdot1 \\
\end{pmatrix}
=\begin{pmatrix}
0 \\
0 \\
\end{pmatrix}.
$$

If an inverse existed, multiplying this equation by it
would give v=0. But v is nonzero, which is a contradiction.

Thus, both the zero determinant and the dependent rows
correctly show that A has no inverse.