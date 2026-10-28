# Exercise 15. Associativity of Multiplication and Different Calculation Paths

The given matrices are

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},
\qquad
C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

## 1. Computing (AB)C

First compute AB:

$$
AB=
\begin{pmatrix}
1+4+0 & 0+2+0 \\
0+2-1 & 0+1+3 \\
\end{pmatrix}
=\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}.
$$

Then multiply by C:

$$
(AB)C=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}
=\begin{pmatrix}
10+0 & 5-2 \\
2+0 & 1-4 \\
\end{pmatrix}
=\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

## 2. Computing A(BC)

First compute BC:

$$
BC=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}
=\begin{pmatrix}
2+0 & 1+0 \\
4+0 & 2-1 \\
-2+0 & -1-3 \\
\end{pmatrix}
=\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}.
$$

Then multiply by A on the left:

$$
A(BC)=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}
=\begin{pmatrix}
2+8+0 & 1+2+0 \\
0+4-2 & 0+1-4 \\
\end{pmatrix}
=\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

## 3. Comparing the calculation paths

For standard row-by-column multiplication, multiplying
an m-by-n matrix by an n-by-p matrix requires mnp scalar
multiplications and mp(n-1) scalar additions.

The counts below include operations involving zero and one.

| Step | Scalar multiplications | Scalar additions |
|---|---:|---:|
| AB | 12 | 8 |
| (AB)C after computing AB | 8 | 4 |
| Total for (AB)C | 20 | 12 |
| BC | 12 | 6 |
| A(BC) after computing BC | 12 | 8 |
| Total for A(BC) | 24 | 14 |

The intermediate matrix AB has size $2\times2$,
whereas BC has size $3\times2$.

Under this counting method, computing AB first requires
fewer scalar operations.

## 4. Conclusion and verification

Both calculation paths give

$$
(AB)C=A(BC)=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

The independent calculations agree in every entry.

Associativity means that changing the grouping of compatible
matrix products does not change the result.
The order of the factors remains A, B, C in both calculations.

Although the result is unchanged, the grouping can affect
the intermediate matrix sizes and the computational effort.