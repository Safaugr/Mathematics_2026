# Exercise 7. Using Properties Instead of Recomputing

The matrix A has size $3\times3$, and

$$
\det A=-4.
$$

## 1. Determinant of 2A

For an n-by-n matrix, multiplying every entry by a scalar k
multiplies the determinant by k^n.
Each of the n rows contributes one factor of k.

Since A has three rows,

$$
\det(2A)=2^3\det A=8(-4)=-32.
$$

## 2. Determinant of the transpose

Transposition does not change the determinant:

$$
\det(A^T)=\det A=-4.
$$

## 3. Determinant of the square

The determinant of a product equals the product
of the determinants:

$$
\det(A^2)=\det(AA)=\det A\cdot\det A=(-4)^2=16.
$$

## 4. Determinant of -A

Multiplying all three rows by -1 gives

$$
\det(-A)=(-1)^3\det A=(-1)(-4)=4.
$$

## Summary

| Expression | Determinant |
|---|---:|
| 2A | -32 |
| A transpose | -4 |
| A squared | 16 |
| -A | 4 |

## Verification

Since $(-A)(-A)=A^2$, the product property requires

$$
\det(-A)\det(-A)=\det(A^2).
$$

The computed values satisfy this:

$$
4\cdot4=16.
$$

Also, transposing twice recovers A, consistent with
the determinant remaining unchanged.