# Exercise 9. Area and the Determinant

The given vectors are

$$
u=
\begin{pmatrix}
3 \\
1 \\
\end{pmatrix},
\qquad
v=
\begin{pmatrix}
1 \\
4 \\
\end{pmatrix}.
$$

## 1. Area of the parallelogram

Place the vectors in the columns of a matrix:

$$
M=
\begin{pmatrix}
3 & 1 \\
1 & 4 \\
\end{pmatrix}.
$$

Its determinant is

$$
\det M=3\cdot4-1\cdot1=11.
$$

The area is the absolute value of the determinant:

$$
S=|\det M|=11.
$$

Therefore, the parallelogram has area 11 square units.

## 2. Reversing the order of the vectors

Reversing the vectors swaps the columns:

$$
N=
\begin{pmatrix}
1 & 3 \\
4 & 1 \\
\end{pmatrix}.
$$

Its determinant is

$$
\det N=1\cdot1-3\cdot4=-11.
$$

The determinant changes sign, but the area remains

$$
|\det N|=|-11|=11.
$$

The sign records orientation. Swapping the vectors
reverses orientation without changing the parallelogram's area.

## 3. Verification

Treat the vectors as three-dimensional vectors
with zero third coordinate. Their cross product is

$$
(3,1,0)\times(1,4,0)=(0,0,11).
$$

Its length is 11, confirming the area.