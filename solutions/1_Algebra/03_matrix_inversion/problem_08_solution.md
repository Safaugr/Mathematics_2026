# Exercise 8. Inverse of a Transformation

## Question

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$

describes a scaling of the plane.
Find the inverse and explain geometrically
what the inverse transformation does.

Check the action of the pair S and its inverse
on one simple vector.

## Solution

### 1. Find the inverse

A diagonal matrix with nonzero diagonal entries
is inverted by taking the reciprocal of each diagonal entry.

Therefore,

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}.
$$

### 2. Geometric interpretation

The original transformation sends a vector (x,y) to

$$
S
\begin{pmatrix}
x \\
y \\
\end{pmatrix}
=\begin{pmatrix}
2x \\
\frac12y \\
\end{pmatrix}.
$$

It doubles the horizontal coordinate and halves
the vertical coordinate.

The inverse transformation halves the horizontal coordinate
and doubles the vertical coordinate.
It reverses the scaling performed by S.

### 3. Check using a vector

Choose

$$
v=
\begin{pmatrix}
2 \\
4 \\
\end{pmatrix}.
$$

First apply S:

$$
Sv=
\begin{pmatrix}
2\cdot2 \\
\frac12\cdot4 \\
\end{pmatrix}
=\begin{pmatrix}
4 \\
2 \\
\end{pmatrix}.
$$

Then apply the inverse:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac12\cdot4 \\
2\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
2 \\
4 \\
\end{pmatrix}
=v.
$$

The original vector is recovered.

### 4. Verification by matrix multiplication

$$
SS^{-1}=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

Multiplying in the other order also gives I,
because both matrices are diagonal and their
corresponding diagonal entries are reciprocals.