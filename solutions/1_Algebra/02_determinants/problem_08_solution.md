# Exercise 8. Determinant of a Product

Given:

$$
\det A=3,\qquad \det B=-5.
$$

## 1. Computing the determinants

The determinant of a product is the product of the determinants:

$$
\det(AB)=\det A\cdot\det B=3(-5)=-15.
$$

Similarly,

$$
\det(BA)=\det B\cdot\det A=(-5)3=-15.
$$

Since $\det A=3\ne0$, the inverse of A exists, and

$$
\det(A^{-1})=\frac{1}{\det A}=\frac{1}{3}.
$$

Therefore,

$$
\det(A^{-1}B)=\frac{1}{3}(-5)=-\frac{5}{3}.
$$

## 2. Why the first two results are equal

The determinants are numbers, so their multiplication
is commutative: $3(-5)=(-5)3$.

This explains why AB and BA have equal determinants,
even though the matrices AB and BA need not be equal.

## 3. Verification

Since $A(A^{-1}B)=B$, the calculated determinants must satisfy

$$
\det A\cdot\det(A^{-1}B)=\det B.
$$

Indeed,

$$
3\left(-\frac{5}{3}\right)=-5.
$$