# Exercise 4. Triangular Matrix

The given matrix is

$$
A=
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}.
$$

## Method

A is upper triangular because all entries below
the main diagonal are zero.

The determinant of any square upper or lower triangular
matrix is the product of its diagonal entries:

$$
\det A=\prod_{i=1}^{n}a_{ii}.
$$

## Calculation

The diagonal entries are 2, -3, and 7. Therefore,

$$
\det A=2\cdot(-3)\cdot7=-42.
$$

## Explanation

In the determinant formula, each term selects one entry
from every row and every column.

For an upper triangular matrix, any term that selects
an entry below the diagonal is zero. The only potentially
nonzero term is the product of the diagonal entries.

The same reasoning applies to a lower triangular matrix.

Thus, the entries 4, 1, and 5 above the diagonal
do not affect this determinant.

## Verification

The diagonal entries have absolute values 2, 3, and 7,
whose product is 42. Exactly one diagonal entry is negative,
so the determinant is negative, consistent with -42.