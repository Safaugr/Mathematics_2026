# Exercise 15. Combining Determinant Properties

A and B are invertible 2-by-2 matrices with

$$
\det A=-2,\qquad \det B=3.
$$

We need to compute

$$
\det(B^{-1}A^TB).
$$

## 1. Apply the product property

The determinant of a product is the product
of the determinants:

$$
\det(B^{-1}A^TB)
=\det(B^{-1})\det(A^T)\det B.
$$

## 2. Apply the inverse and transpose properties

Since B is invertible,

$$
\det(B^{-1})=\frac{1}{\det B}=\frac{1}{3}.
$$

Transposition preserves the determinant:

$$
\det(A^T)=\det A=-2.
$$

Therefore,

$$
\det(B^{-1}A^TB)
=\frac{1}{3}(-2)(3)
=-2.
$$

## 3. Why the B factors cancel

The factors involving B are scalar numbers and satisfy

$$
\det(B^{-1})\det B
=\frac{1}{\det B}\det B
=1.
$$

Thus, the expression reduces to the determinant of A.

This cancellation occurs among scalar determinants.
It does not require rearranging the matrix factors.

## Verification

Let

$$
M=B^{-1}A^TB.
$$

Multiplying on the left by B gives

$$
BM=A^TB.
$$

Taking determinants,

$$
\det B\cdot\det M=\det(A^T)\det B.
$$

Since the determinant of B is nonzero, division gives

$$
\det M=\det(A^T)=\det A=-2.
$$

This confirms the result.