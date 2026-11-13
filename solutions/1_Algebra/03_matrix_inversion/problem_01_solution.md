# Exercise 1. Definition of the Inverse

## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix},
$$

check, without using a formula, whether $B=A^{-1}$.
Compute AB and BA and relate the result to the definition
of the inverse.

## Solution

### 1. Definition

A matrix B is the inverse of A if

$$
AB=BA=I,
$$

where I is the identity matrix of the same size.

Both given matrices have size $2\times2$,
so both products are defined.

### 2. Computing AB

Using row-by-column multiplication,

$$
AB=
\begin{pmatrix}
2\cdot1+1(-1) & 2(-1)+1\cdot2 \\
1\cdot1+1(-1) & 1(-1)+1\cdot2 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

### 3. Computing BA

Similarly,

$$
BA=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
(-1)\cdot2+2\cdot1 & (-1)\cdot1+2\cdot1 \\
\end{pmatrix}
=\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
=I.
$$

### 4. Conclusion

Both products equal the identity matrix.
Therefore, B satisfies the definition of the inverse of A:

$$
B=A^{-1}.
$$

The two explicit multiplications verify the result
without using an inverse formula.