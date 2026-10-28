# Exercise 6. Parameter and Invertibility

The given matrix is

$$
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t \\
\end{pmatrix}.
$$

## 1. Compute the determinant

For a 2-by-2 matrix, the determinant is ad-bc.
Therefore,

$$
\det A(t)=t\cdot t-1\cdot2=t^2-2.
$$

## 2. Find when the inverse does not exist

A square matrix is not invertible exactly when
its determinant is zero.

Thus,

$$
t^2-2=0.
$$

Solving gives

$$
t^2=2,
\qquad
t=\pm\sqrt{2}.
$$

Therefore, A(t) is not invertible at the two values

$$
t=\sqrt{2},\qquad t=-\sqrt{2}.
$$

## 3. Verification using row dependence

For either exceptional value, t^2=2, so

$$
t(t,1)=(t^2,t)=(2,t).
$$

The second row is therefore t times the first row.
The rows are linearly dependent, confirming that
the matrix is not invertible.

For all other real values of t, the determinant is nonzero,
so the matrix is invertible.

## Conclusion

$$
A(t)\ \mathrm{is\ not\ invertible}
\quad\Longleftrightarrow\quad
t=\pm\sqrt{2}.
$$