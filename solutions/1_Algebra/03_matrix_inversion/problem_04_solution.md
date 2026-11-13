# Exercise 4. Gauss–Jordan

## Question

Find the inverse using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}.
$$

Show the augmented matrix after successive operations
and explain why obtaining I on the left gives
the inverse on the right.

## Solution

### 1. Form the augmented matrix

Place the identity matrix beside A:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}.
$$

Every row operation must be applied to both sides.

### 2. Eliminate the first entry of row 2

Apply

$$
R_2\leftarrow R_2-3R_1.
$$

This gives

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}.
$$

### 3. Make the second pivot equal to 1

Apply

$$
R_2\leftarrow -R_2.
$$

The resulting matrix is

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}.
$$

### 4. Eliminate the entry above the second pivot

Apply

$$
R_1\leftarrow R_1-2R_2.
$$

This gives

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}.
$$

The left side is now I, so

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}.
$$

### 5. Why the method works

Each elementary row operation is equivalent to
multiplying on the left by an invertible elementary matrix.

Let E represent the product of these elementary matrices.
The operations transform the left side into EA=I.
Thus, E is the inverse of A.

Applying the same operations to the right side
transforms I into EI=E, which is the required inverse.

### 6. Verification

Direct multiplication gives

$$
AA^{-1}=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}
=\begin{pmatrix}
-5+6 & 2-2 \\
-15+15 & 6-5 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

This confirms the result.