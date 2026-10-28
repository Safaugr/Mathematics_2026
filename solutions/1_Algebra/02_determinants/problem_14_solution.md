# Exercise 14. A System of Equations and the Determinant

The coefficient matrix is

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}.
$$

## 1. Exactly one solution for every right-hand side

The determinant is

$$
\det A=1\cdot4-2k=4-2k.
$$

The system Ax=b has exactly one solution for every b
if and only if A is invertible. Therefore,

$$
4-2k\ne0,
\qquad
k\ne2.
$$

## 2. The exceptional value

When k=2, write the unknown vector as $(x_1,x_2)^T$.
The system becomes

$$
\begin{cases}
x_1+2x_2=b_1, \\
2x_1+4x_2=b_2. \\
\end{cases}
$$

The second left-hand side is twice the first.
Thus, consistency requires

$$
b_2=2b_1.
$$

## 3. Example with infinitely many solutions

Choose

$$
b=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}.
$$

The equations are

$$
\begin{cases}
x_1+2x_2=1, \\
2x_1+4x_2=2. \\
\end{cases}
$$

The second equation repeats the first.
Setting x_2=s gives all solutions:

$$
x=
\begin{pmatrix}
1-2s \\
s \\
\end{pmatrix},
\qquad s\in\mathbb{R}.
$$

Substitution gives

$$
(1-2s)+2s=1,
$$

$$
2(1-2s)+4s=2.
$$

Therefore, every real value of s gives a solution.

## 4. Example with no solution

Choose

$$
b=
\begin{pmatrix}
1 \\
3 \\
\end{pmatrix}.
$$

The equations are

$$
\begin{cases}
x_1+2x_2=1, \\
2x_1+4x_2=3. \\
\end{cases}
$$

Subtracting twice the first equation from the second gives

$$
0=1.
$$

This contradiction proves that no solution exists.

## Conclusion

For $k\ne2$, there is exactly one solution for every b.

For $k=2$, there are infinitely many solutions when
$b_2=2b_1$, and no solution otherwise.